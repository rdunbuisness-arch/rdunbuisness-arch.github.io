# Deficit: sound effect ideas

Retro chiptune SFX made with the Web Audio API (no audio files). The table matches `sound-demo.html`.

## Guidance
- **Subtle:** peak gain 0.03–0.08, every sound under 0.8 s, soft 5 ms attack and exponential release (no clicks). Nothing should play over 2× per second; when +/- auto-repeats, play only every 3rd tick.
- **Mute toggle:** a 🔊/🔇 pixel button in the header plus a Settings switch, saved in localStorage (`deficit-sound`).
- **Default: OFF.** Calorie logging happens in public (meals, work), and browsers block audio until a user gesture anyway. Show a one-time hint "Turn on sounds?" after the first Finish day.
- Respect `prefers-reduced-motion` as a hint to keep celebratory sounds short. Never play the surplus sound as a punishment, only once per day when the day crosses into surplus.
- Create one shared `AudioContext` lazily on the first tap.

## Events
| Event | Description | Waveform | Notes (Hz) | Step / total |
|---|---|---|---|---|
| Add calories (+100) | Short soft upward blip on each tap. | square | 660 → 880 | 40 ms / ~80 ms |
| Remove calories (−100) | Same blip, inverted downward. | square | 880 → 660 | 40 ms / ~80 ms |
| Quick-add chip (+50/+250/+500) | Coin pickup; bigger chips add a third note. | square | 988 → 1319 | 60 ms / ~120 ms |
| Finish / lock day | Satisfying "save point" chime, rising arpeggio. | triangle | 523 → 659 → 784 → 1047 | 90 ms / ~360 ms |
| Pound crossed (+1 lb) | Classic 1-up: quick 6-note rising run. | square | 659 → 784 → 1319 → 1047 → 1175 → 1568 | 70 ms / ~420 ms |
| Goal milestone (every 10%) | Mini fanfare: two held chords, triangle. | triangle | 523 → 659 → 784 → rest → 659 → 784 → 1047 | 120 ms / ~840 ms |
| Streak extended | Two bright sparkle pings. | sine | 1568 → 2093 | 80 ms / ~160 ms |
| Surplus warning (day goes negative) | Gentle low two-note "uh-oh", never harsh. | triangle | 392 → 311 | 140 ms / ~280 ms |
| Nav / date change | Tiny tick, barely there. | square | 1200 | 25 ms / ~25 ms |
| Error / invalid input | Low buzzy double bonk. | sawtooth | 147 → rest → 147 | 70 ms / ~210 ms |

Each note: oscillator → gain envelope (0 → peak in 5 ms, exponential decay to 0.0001 over 1.2× step). Peak gain per event: add 0.05, remove 0.05, chip 0.05, finish 0.08, pound 0.06, goal 0.08, streak 0.06, surplus 0.07, nav 0.03, error 0.05.

## Copy-paste for Grok Build
```
Add optional retro chiptune sound effects to Deficit using only the Web Audio API (no audio files).
- Create src/lib/deficit/sfx.ts exporting play(event) and setMuted(bool). Lazily create one AudioContext on first user gesture.
- Sound is OFF by default. Add a 🔊/🔇 pixel toggle in the header and a switch in Settings; persist in localStorage key "deficit-sound".
- Keep it subtle: peak gain ≤ 0.08, 5 ms attack, exponential release, every sound < 0.8 s. When +/- auto-repeats, sound only every 3rd tick.
- Play the surplus warning at most once per day, only when the open day's deficit crosses from ≥0 to <0.
- Events (wave; notes in Hz; ms per note; peak gain):
  add: square; 660,880; 40ms; 0.05   (Add calories (+100))
  remove: square; 880,660; 40ms; 0.05   (Remove calories (−100))
  chip: square; 988,1319; 60ms; 0.05   (Quick-add chip (+50/+250/+500))
  finish: triangle; 523,659,784,1047; 90ms; 0.08   (Finish / lock day)
  pound: square; 659,784,1319,1047,1175,1568; 70ms; 0.06   (Pound crossed (+1 lb))
  goal: triangle; 523,659,784,rest,659,784,1047; 120ms; 0.08   (Goal milestone (every 10%))
  streak: sine; 1568,2093; 80ms; 0.06   (Streak extended)
  surplus: triangle; 392,311; 140ms; 0.07   (Surplus warning (day goes negative))
  nav: square; 1200; 25ms; 0.03   (Nav / date change)
  error: sawtooth; 147,rest,147; 70ms; 0.05   (Error / invalid input)
- Implementation:
function tone(ctx,wave,f,t,d,g){if(!f)return;const o=ctx.createOscillator(),a=ctx.createGain();o.type=wave;o.frequency.value=f;a.gain.setValueAtTime(0,t);a.gain.linearRampToValueAtTime(g,t+0.005);a.gain.exponentialRampToValueAtTime(0.0001,t+d/1000);o.connect(a).connect(ctx.destination);o.start(t);o.stop(t+d/1000+0.02);}
function playSfx(ctx,s){const t0=ctx.currentTime+0.01;s.notes.forEach((f,i)=>tone(ctx,s.wave,f,t0+i*s.step/1000,s.step*1.2,s.gain));}
  where a sound is {wave, notes, step, gain}.
```
