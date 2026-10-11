# Cozy adventure — mechanics framework v1 (story-agnostic)
Target: 20–30 min, one sitting, no fail state. Hero: the traveler (8-dir walk).

## Core loop
Explore an area -> talk to residents -> learn a need or a clue -> find or earn a tool -> use the tool to open the next area -> repeat 4 times -> climax.

## Systems (World Engineer can build these now; content comes from the story outline)
1. Interaction: a "!" prompt appears near NPCs and objects; E/Space/tap to interact.
2. Dialogue: a text box on the 9-slice panel, with portrait slot, typewriter text (skip on press), and 2–3 choice replies. Data-driven from dialogue.json (nodes, conditions on flags/items, effects that set flags or give/take items).
3. Inventory: up to 8 key items, an I/Tab grid, and item descriptions. Using an item works in context: interact with a target while holding the right item. No crafting.
4. Clue journal: auto-logs clues and current goal; J opens it; HUD shows a one-line "current goal".
5. Gates: data-driven blockers (brambles need shears, a gap needs a plank, a dark cave needs the lantern, a locked gate needs a key, a stream needs stepping stones). Each gate shows a hint line when you bump it.
6. Puzzles, 3 types, reusable: (a) push-block or stepping-stone placement on the tile grid; (b) order/sequence (ring bells or light lamps in an order hinted by clues); (c) fetch/trade chain between NPCs.
7. Save: a hearth/bench save point that autosaves to localStorage (position, flags, items), plus an autosave on area change; Continue on the title screen.
8. Areas: 5 small connected maps (about 20x15 tiles each) with fade transitions; camera follows.
9. Climax framework: a scripted sequence system (move NPCs, camera pans, timed dialogue, a screen tint), used for the finale and 1–2 earlier beats.
10. Ending: credits roll plus a stats card (time, secrets found out of 5, creatures helped) and share text.

## Pacing template (the story fills it)
Act 1 (5 min): home or village, learn the problem, get tool 1.
Act 2 (15 min): areas 2–4, each with one resident, one tool, one puzzle and one optional secret.
Act 3 (5–8 min): the final area uses all the tools, then the climax sequence and the ending.
