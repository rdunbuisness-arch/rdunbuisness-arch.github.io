# Grok Build brief: Deficit, "Soft Pastel Pixel" restyle + fixes

Copy-paste everything below into Grok Build.

---

Restyle the Deficit app (calorie deficit tracker) to a **soft pastel pixel-art** look, and apply the bug fixes and UX changes below. Keep it simple: one main screen, big readable numbers, same data model and localStorage key (`deficit-tracker`). Do not change the deficit formula (deficit = TDEE + extra burn − eaten; 3500 kcal = 1 lb; Mifflin-St Jeor TDEE).

## Style
- **Fonts (Google Fonts):** `Silkscreen` (400) for labels, buttons, headings (uppercase, letter-spacing 1px, 10–12px). `VT323` for all numbers and body text (20px body; hero number 56px; daily deficit 36px; eaten counter 52px). Use `font-variant-numeric: tabular-nums`.
- **Palette:**
  - Background `#FDF6EC` (cream), panels `#FFFFFF`
  - Ink / borders / text `#4A4063` (plum)
  - Hero deficit number `#FF8FAB` (pink)
  - Stat numbers / logo `#7C6FD6` (lavender)
  - Positive / deficit / primary button `#B9FBC0`, shadow `#72C97C`, positive text `#3F9A4F`
  - Negative / surplus `#FFB3C6`
  - Secondary buttons `#CDEFFD`, shadow `#A2D2FF`; goal bar `#A2D2FF`
  - Highlight / today / notice `#FFE5A3`; panel drop shadow `#CDB4DB`
- **Pixel borders:** no border-radius anywhere. Panels: `border:3px solid #4A4063; box-shadow:4px 4px 0 #CDB4DB`. Buttons: `border:3px solid #4A4063; box-shadow:3px 3px 0 <shadow color>`; on `:active` `transform:translate(2px,2px); box-shadow:none`. Set `image-rendering: pixelated`.
- **Progress bars (pound bar, goal bar):** 18px tall, 3px plum border, cream track; pound fill is a pixel-striped `repeating-linear-gradient(90deg,#FF8FAB 0 8px,#FFB3C6 8px 12px)`; goal fill solid `#A2D2FF`. Fill width snaps in 4% steps for a chunky look.
- **21-day bar chart:** deficit days are mint bars, surplus days pink bars, missing days a short grey stub `#EEE`, today is a dashed-border yellow bar. Each bar gets a 2px plum border. Add a hidden-text `aria-label` summary.
- Respect `prefers-reduced-motion`; keep the count-up and add a small 2-frame "+1 LB" pixel pop when a pound is crossed.

## Layout (mobile first, max-width 420px, single column)
1. Header: `DEFICIT` logo · `◀ MON 10/12 ▶` date nav · ⚙ settings. Show a yellow "TODAY" chip button when not on today.
2. Hero panel: label "TOTAL DEFICIT", big `+4,820 kcal`, line "1.4 lb banked · 2,180 kcal to next lb", pound bar, then "GOAL −30 LB · 5%" and goal bar.
3. Four stat tiles: STREAK `5d`, 7-DAY AVG `+803`, EST LB `208.6`, GOAL ETA `FEB 23`.
4. 21-day chart panel.
5. Today panel: "TODAY · OPEN/LOCKED" + day deficit; equation line `2,290 base + 250 burn − 1,600 eaten = +940`; EATEN tally (−100 / value / +100) plus +50 / +250 / +500 chips; EXTRA BURN small tally (−50 / value / +50); actions: big mint `FINISH DAY ✓` and `LOG` (renamed from "Ledger").

## Bug fixes (in `src/lib/deficit/model.ts`, `store.ts`, components)
1. **Data loss on reload:** setup (`setup-screen.tsx` ~L35) and settings (`settings-sheet.tsx` ~L46) accept goal weight ≤ 0 (e.g. 0 or −5), but `cleanSettings` (`model.ts` L399) rejects it on hydrate, so `merge` (`store.ts` ~L95) drops settings AND all logs. Validate goal > 0 in both forms, use one shared `validateSettings()` from model.ts, and in `merge` never discard logs when only settings fail; keep logs and send the user to setup.
2. **Fractional age/height pass the forms but fail on reload:** `cleanSettings` checks range before rounding (`model.ts` L400–402); age 100.4 or heightIn 11.6 get the whole backup rejected. Round first, then range-check (also clamp the import).
3. **Stats depend on the viewed date:** `project()` uses `end = timelineEnd(logs, date, today)` (`model.ts` L285) for streak (L357), the 7-day pace window (L286–290) and ETA (L294). Browsing 2 days ahead makes the streak 0; 7 days ahead makes the 7-day pace "—"; 30 days ahead pushes the ETA out a month. Compute streak/pace/ETA from `today`, not from the viewed date.
4. **Future days can be finished:** after "Finish day" the app jumps to tomorrow (`deficit-app.tsx` ~L72 and the initial-date logic ~L18), and nothing stops finishing tomorrow or any future day, which banks a full-TDEE "fast" in advance. Disable Finish on dates after today; after finishing, stay on today and show it as LOCKED.
5. **7-day pace ignores gaps:** `pace7` averages only the logged days in the window (`model.ts` L288); one logged day in 7 shows as that day's value. Show it as "avg of N logged days" or divide by 7, and say which.
6. **ETA shown during a surplus streak:** when `pace7 ≤ 0` the rate falls back to the all-time average (`model.ts` L292), so the ETA still shows a date while you're gaining. Show "Pace negative this week" instead of a date.
7. **Invalid dates accepted on import:** `DATE_RE` (`model.ts` L81) is format-only; `2026-13-45` imports and `addDays` rolls it to 2027-02-14. Validate a real calendar date (round-trip through `addDays(d,0) === d`).
8. **Extra burn input can't be cleared or typed naturally** (`day-screen.tsx` ~L194–199): it parses every keystroke and snaps to "0". Reuse the Tally draft/blur pattern.
9. Minor: the "high" activity multiplier is 1.465 (`model.ts` L6), which is non-standard (Mifflin-St Jeor tables use 1.55 moderate / 1.725 very active). Either relabel it or use 1.55. Keyboard +/- (`deficit-app.tsx`) steps 100 but doesn't trigger the haptic/"hot" feedback the buttons do. Fine to leave.

## UX / readability changes
1. Show the day's equation and the result together, in big type (`base + burn − eaten = deficit`), and color the result (mint deficit / pink surplus).
2. Rename and clarify: "Cumulative deficit" → "Total deficit", "Ledger" → "Log", "Est" → "Est. weight", "Left" → "lb to go", "Pending/Locked" → "Open/Locked".
3. Raise the contrast and size of tiny gray 12px uppercase labels: min 11px pixel font in plum on white.
4. Make the goal bar a real 18px pixel bar with % and lb to go. Today it's a 1px hairline.
5. Bars chart: color deficit vs surplus, mark today, add a legend ("■ deficit ■ surplus").
6. Finish day: confirm with a short toast "Day locked: +940 → 1.4 lb banked" and stay on today; never auto-jump to tomorrow.
7. Add a one-tap "+custom" chip that opens the number pad on the eaten input.
8. All tap targets ≥ 44px; visible focus ring (3px dashed plum).
