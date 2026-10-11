# Spore Run — design v1

## Pitch
Spore Run is a 2–3 minute top-down forest dash built on our existing walking mushroom heroes. You play the traveler racing to plant spores on 10 bare dirt patches before nightfall, while a hungry Robin hops toward you whenever you stand still. Every planted patch sprouts a tiny mushroom and adds 5 seconds to the clock; picking up a glowing dewdrop gives a short speed burst. Your score is patches planted plus seconds left, shown on a one-tap share screen ("I planted 10 in 1:42 — beat me"), so friends can trade times tonight. One map, one enemy, one pickup, tight and polished.

## Controls
Arrow keys / WASD to move (touch: drag anywhere). Planting is automatic when you step on a patch. R to restart.

## Core loop
Move -> plant patch (+5s, sprout pop) -> grab dewdrop (speed) -> dodge Robin (hit = lose 3s, short knockback) -> plant all 10 or timer hits 0 -> score screen -> restart.

## Art assets (32x32 world tiles (map scaled to 32px); small sprites at listed sizes, PNG, transparent bg)
1. Player = the traveler (existing art); old fly agaric/robin sprites retired
2. Robin hop cycle (4 frames) + peck frame — Animation
3. Grass ground tile (2 variants)
4. Bare dirt patch tile
5. Sprouted baby mushroom (2-frame pop)
6. Tree / bush border obstacle (32x32)
7. Rock obstacle
8. Glowing dewdrop pickup (2-frame shimmer)
9. Spore puff effect (3 frames)
10. Title/score panel frame (9-slice, 48x48) and small clock icon

## Build tasks (World Engineer, first pass, placeholders OK)
1. Single 20x15 tile map in /workspace/studio/world, border of trees, scattered rocks, 10 dirt patches.
2. Player movement with collision; auto-plant on patch, +5s, counter.
3. 90s countdown timer HUD; dusk tint as time runs out.
4. Robin AI: hops toward player, faster when player idle; hit = -3s + knockback + brief invulnerability.
5. Dewdrops: 3 spawns, 2s speed boost.
6. Win/lose score screen with copyable share text and R to restart.
7. Swap placeholders for studio art as it lands in assets/.
Note: tiles 32x32 per Director; Branch 2 does tiles/tree/bush/rock, Branch 3 does items 3,6,7,8. Enemy (Robin) art TBD, placeholder for now.
