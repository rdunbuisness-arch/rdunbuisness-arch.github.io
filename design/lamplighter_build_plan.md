# The Lamplighter's Thread — build plan (from outline v1.1)
The systems come from adventure_mechanics.md. Everything is data-driven: areas/*.json, dialogue.json, items.json, flags.
Tool order: Shears -> Plank -> Lantern -> Key (+ Lantern Heart). No fail state, and hint lines appear on every gate.

## Milestone 1 — village + chapter 1 (playable first, about 5 min)
Area: Meadow / Bramblewick, about 30x20 tiles. It has Thistle's cottage (enterable 1-room interior with the save hearth), the festival stall, berry bushes, the dark lighthouse visible on the headland (blocked by a "path washed out — come back later" sign until the climax), and an east exit to the Pond blocked by brambles.
Flow:
1. Title screen, then the intro card: "The beacon is dark. Wren's boat is still out in the fog."
2. Inside the cottage: read Thistle's half-finished letter (a journal clue, the goal becomes "Find Thistle") and pick up the broken key handle (a story item). Touching the hearth saves.
3. Robin, near the stall: "I need a ribbon for my nest-lantern." Stall keeper (use the fox placeholder or a sign NPC): "Ribbons for berries!"
4. Pick 3 berries from the bushes (a "3/3" counter). Trade berries for the ribbon, then give the ribbon to the robin, who gives the Shears.
5. Use the shears on the brambles, then a fade transition to the Pond. End of milestone 1: a "Chapter 1 complete" card.
6. Secret 1: a festival pie behind the stall.
Done when: it plays start to finish in 4–6 min, saves and continues, and nothing soft-locks.

## Milestone 2 — Pond
Stepping-stone push puzzle (3 stones into a 3-gap row) to reach the deer on the islet. The deer gives the Plank. Secret: a journal page under the willow.

## Milestone 3 — Fly Agaric Wood
The plank bridges the gap. Mushroom sequence: 4 glowing mushrooms, with the order given by the journal riddle; a wrong press makes them all dim and reset, and the hint repeats. Reward: the Lantern. Secret: a journal page in a hollow log.

## Milestone 4 — Coast / Tide Cave
The lantern lights the dark cave (with a vision radius; without the lantern you only see a 1-tile circle and an "It's too dark" hint). Thistle hides with the fox guarding him. Help the fox (bring a fish from the tide pool), and you get the Key plus the Lantern Heart. A cutscene with Thistle reveals the Fogwyrm twist. Secret: a journal page in a tide pool.

## Milestone 5 — Lighthouse climax and epilogue
Storm tint with rain. Floor 1: shears on the vines over the door. Floor 2: the lantern on the dark stairs. Floor 3: the plank over the broken landing. Floor 4: the key opens the lamp room. Lamp sequence while the Fogwyrm circles. Then a choice ("Give the lantern" is the only way forward, and refusing loops gently). The Fogwyrm shrinks to a wisp, the beacon relights, Wren's boat arrives, and the epilogue festival plays, followed by credits and the stats card (time, secrets out of 5, friends helped). Secret: a golden acorn on the balcony.
