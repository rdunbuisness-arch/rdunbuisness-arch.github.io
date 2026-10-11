# Fox walk right v2 - fixes on Artist 3 frames

- Base: Artist 3 v1 frames /workspace/studio/branch3/fox_walk_right_f1..f8_v1.png: 512x512 exports of **32x32** native art (16x blocks), magenta #fa08fa background, facing right.
- Fix 1: all four legs redrawn in your leg style. Far legs are one shade darker (upper #884315 instead of #a64c10; socks stay #3a1818). Diagonal pairs: near front + far hind share a phase, near hind + far front are half a cycle later. Feet are planted for 5 frames and lifted 1px for 2 (swing). Paw outline on ground row y=26 when planted. Far legs are drawn behind the body, near legs in front.
- Fix 2: tail tip (x<=8, y<=9) moves 1px vertically one frame behind the body bob: body up on f3/f7 (your bob, kept), tail up on f4/f8.
- Fix 3: body, head and ears are your f1 pixels in every frame (shifted only vertically by the bob), so head x is locked. I could not find a sideways head shift in the v1 pixels themselves (f3/f7 heads match f1 shifted up 1px); the jitter you saw was most likely the tail outline changing width on f3/f7, which is now fixed as well.
- Each frame lists SET/CLEAR relative to YOUR v1 frame with the same number.
- Planning GIF: fox_walk_right_v2_preview.gif (8 fps).

Palette (key = hex), same as the v1 frames:
  . = #fa08fa
  a = #c4550c
  b = #3a2518
  c = #eec991
  d = #a64c10
  e = #f5b658
  f = #3a1818
  g = #884315
  h = #f0f0f0

## Frame 1: start from branch3/fox_walk_right_f1_v1.png, save as branch3/fox_walk_right_f1_v2.png

SET (62 px), grouped by colour:
#### #c4550c (key a) - 4 px
9,21 #c4550c
10,21 #c4550c
19,21 #c4550c
20,21 #c4550c
#### #3a2518 (key b) - 24 px
8,21 #3a2518
11,21 #3a2518
18,21 #3a2518
22,21 #3a2518
8,22 #3a2518
11,22 #3a2518
18,22 #3a2518
22,22 #3a2518
8,23 #3a2518
11,23 #3a2518
18,23 #3a2518
22,23 #3a2518
7,24 #3a2518
17,24 #3a2518
19,24 #3a2518
7,25 #3a2518
17,25 #3a2518
19,25 #3a2518
8,26 #3a2518
9,26 #3a2518
15,26 #3a2518
19,26 #3a2518
20,26 #3a2518
21,26 #3a2518
#### #3a1818 (key f) - 8 px
14,22 #3a1818
15,22 #3a1818
14,23 #3a1818
15,23 #3a1818
15,24 #3a1818
16,24 #3a1818
15,25 #3a1818
16,25 #3a1818
#### #884315 (key g) - 26 px
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
14,21 #884315
15,21 #884315
9,22 #884315
10,22 #884315
19,22 #884315
20,22 #884315
9,23 #884315
10,23 #884315
19,23 #884315
20,23 #884315
8,24 #884315
9,24 #884315
20,24 #884315
21,24 #884315
8,25 #884315
9,25 #884315
20,25 #884315
21,25 #884315

CLEAR back to magenta #fa08fa (31 px):
16,19 #fa08fa
12,21 #fa08fa
17,21 #fa08fa
23,21 #fa08fa
24,21 #fa08fa
12,22 #fa08fa
17,22 #fa08fa
23,22 #fa08fa
24,22 #fa08fa
12,23 #fa08fa
17,23 #fa08fa
23,23 #fa08fa
24,23 #fa08fa
11,24 #fa08fa
12,24 #fa08fa
13,24 #fa08fa
23,24 #fa08fa
24,24 #fa08fa
25,24 #fa08fa
11,25 #fa08fa
12,25 #fa08fa
13,25 #fa08fa
23,25 #fa08fa
24,25 #fa08fa
25,25 #fa08fa
11,26 #fa08fa
12,26 #fa08fa
13,26 #fa08fa
17,26 #fa08fa
23,26 #fa08fa
24,26 #fa08fa

Finished grid (row 0 first):
```
................................
................................
....................b.....b.....
....bbb............bab...bab....
...bcccb...........bacb.bcab....
..bcccccb..........baabbbaab....
.becccccb...........beeeeeeeb...
baacccccb..........baaaahfaaab..
baaacccb...........baaaaffaaafb.
baaaaab............bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
........baab.bggb.baabb.........
........bggb.bffb.bggbb.........
........bggb.bffb.bggbb.........
.......bggb...bffbbbggb.........
.......bggb...bffbbbggb.........
........bb.....bb..bbb..........
................................
................................
................................
................................
................................
```

## Frame 2: start from branch3/fox_walk_right_f2_v1.png, save as branch3/fox_walk_right_f2_v2.png

SET (52 px), grouped by colour:
#### #3a2518 (key b) - 19 px
8,22 #3a2518
11,22 #3a2518
15,22 #3a2518
17,22 #3a2518
22,22 #3a2518
8,23 #3a2518
11,23 #3a2518
18,23 #3a2518
22,23 #3a2518
8,24 #3a2518
11,24 #3a2518
18,24 #3a2518
22,24 #3a2518
9,25 #3a2518
16,25 #3a2518
14,26 #3a2518
15,26 #3a2518
19,26 #3a2518
20,26 #3a2518
#### #3a1818 (key f) - 8 px
14,22 #3a1818
21,22 #3a1818
14,23 #3a1818
15,23 #3a1818
14,24 #3a1818
15,24 #3a1818
14,25 #3a1818
15,25 #3a1818
#### #884315 (key g) - 25 px
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
13,21 #884315
14,21 #884315
21,21 #884315
22,21 #884315
9,22 #884315
10,22 #884315
19,22 #884315
9,23 #884315
10,23 #884315
19,23 #884315
20,23 #884315
9,24 #884315
10,24 #884315
19,24 #884315
20,24 #884315
19,25 #884315
20,25 #884315

CLEAR back to magenta #fa08fa (21 px):
16,19 #fa08fa
16,22 #fa08fa
23,22 #fa08fa
12,23 #fa08fa
17,23 #fa08fa
23,23 #fa08fa
24,23 #fa08fa
12,24 #fa08fa
17,24 #fa08fa
23,24 #fa08fa
24,24 #fa08fa
11,25 #fa08fa
12,25 #fa08fa
17,25 #fa08fa
22,25 #fa08fa
23,25 #fa08fa
24,25 #fa08fa
11,26 #fa08fa
12,26 #fa08fa
22,26 #fa08fa
23,26 #fa08fa

Finished grid (row 0 first):
```
................................
................................
....................b.....b.....
....bbb............bab...bab....
...bcccb...........bacb.bcab....
..bcccccb..........baabbbaab....
.becccccb...........beeeeeeeb...
baacccccb..........baaaahfaaab..
baaacccb...........baaaaffaaafb.
baaaaab............bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........baabggb.baabggb........
........bggbbffb.bggbfb.........
........bggb.bffb.bggbb.........
........bggb.bffb.bggbb.........
.........bb..bffb.bggb..........
..............bb...bb...........
................................
................................
................................
................................
................................
```

## Frame 3: start from branch3/fox_walk_right_f3_v1.png, save as branch3/fox_walk_right_f3_v2.png

SET (75 px), grouped by colour:
#### #c4550c (key a) - 2 px
18,21 #c4550c
19,21 #c4550c
#### #3a2518 (key b) - 31 px
4,3 #3a2518
5,3 #3a2518
6,3 #3a2518
3,4 #3a2518
7,4 #3a2518
2,5 #3a2518
1,6 #3a2518
8,6 #3a2518
8,7 #3a2518
7,8 #3a2518
10,22 #3a2518
13,22 #3a2518
21,22 #3a2518
24,22 #3a2518
10,23 #3a2518
13,23 #3a2518
21,23 #3a2518
24,23 #3a2518
10,24 #3a2518
15,24 #3a2518
17,24 #3a2518
21,24 #3a2518
24,24 #3a2518
11,25 #3a2518
15,25 #3a2518
17,25 #3a2518
22,25 #3a2518
13,26 #3a2518
14,26 #3a2518
18,26 #3a2518
19,26 #3a2518
#### #eec991 (key c) - 10 px
3,6 #eec991
7,6 #eec991
3,7 #eec991
4,7 #eec991
5,7 #eec991
6,7 #eec991
7,7 #eec991
4,8 #eec991
5,8 #eec991
6,8 #eec991
#### #f5b658 (key e) - 1 px
2,6 #f5b658
#### #3a1818 (key f) - 7 px
22,22 #3a1818
23,22 #3a1818
23,23 #3a1818
14,24 #3a1818
23,24 #3a1818
13,25 #3a1818
14,25 #3a1818
#### #884315 (key g) - 24 px
13,18 #884315
14,18 #884315
21,18 #884315
22,18 #884315
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
13,21 #884315
14,21 #884315
21,21 #884315
22,21 #884315
11,22 #884315
12,22 #884315
12,23 #884315
12,24 #884315
18,24 #884315
19,24 #884315
18,25 #884315
19,25 #884315

CLEAR back to magenta #fa08fa (29 px):
4,1 #fa08fa
5,1 #fa08fa
6,1 #fa08fa
3,2 #fa08fa
4,2 #fa08fa
5,2 #fa08fa
6,2 #fa08fa
7,2 #fa08fa
2,3 #fa08fa
3,3 #fa08fa
7,3 #fa08fa
8,3 #fa08fa
1,4 #fa08fa
2,4 #fa08fa
8,4 #fa08fa
0,5 #fa08fa
1,5 #fa08fa
0,6 #fa08fa
16,18 #fa08fa
9,22 #fa08fa
9,23 #fa08fa
9,24 #fa08fa
9,25 #fa08fa
10,25 #fa08fa
21,25 #fa08fa
10,26 #fa08fa
11,26 #fa08fa
21,26 #fa08fa
22,26 #fa08fa

Finished grid (row 0 first):
```
................................
....................b.....b.....
...................bab...bab....
....bbb............bacb.bcab....
...bcccb...........baabbbaab....
..bcccccb...........beeeeeeeb...
.becccccb..........baaaahfaaab..
baacccccb..........baaaaffaaafb.
baaacccb...........bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........baabggb.baabggb........
..........bggbfb.bggbbffb.......
..........bggbfb.bggbbffb.......
..........bggbfb.bggbbffb.......
...........bbffb.bggb.bb........
.............bb...bb............
................................
................................
................................
................................
................................
```

## Frame 4: start from branch3/fox_walk_right_f4_v1.png, save as branch3/fox_walk_right_f4_v2.png

SET (59 px), grouped by colour:
#### #c4550c (key a) - 1 px
12,21 #c4550c
#### #3a2518 (key b) - 24 px
10,21 #3a2518
13,21 #3a2518
21,21 #3a2518
24,21 #3a2518
10,22 #3a2518
15,22 #3a2518
17,22 #3a2518
20,22 #3a2518
24,22 #3a2518
10,23 #3a2518
14,23 #3a2518
19,23 #3a2518
24,23 #3a2518
14,24 #3a2518
19,24 #3a2518
25,24 #3a2518
16,25 #3a2518
25,25 #3a2518
12,26 #3a2518
13,26 #3a2518
17,26 #3a2518
18,26 #3a2518
23,26 #3a2518
24,26 #3a2518
#### #3a1818 (key f) - 8 px
22,22 #3a1818
23,22 #3a1818
22,23 #3a1818
23,23 #3a1818
23,24 #3a1818
24,24 #3a1818
23,25 #3a1818
24,25 #3a1818
#### #884315 (key g) - 26 px
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
14,21 #884315
22,21 #884315
23,21 #884315
11,22 #884315
12,22 #884315
18,22 #884315
11,23 #884315
12,23 #884315
17,23 #884315
18,23 #884315
12,24 #884315
13,24 #884315
17,24 #884315
18,24 #884315
12,25 #884315
13,25 #884315
17,25 #884315
18,25 #884315

CLEAR back to magenta #fa08fa (24 px):
16,19 #fa08fa
9,21 #fa08fa
9,22 #fa08fa
16,22 #fa08fa
8,23 #fa08fa
9,23 #fa08fa
15,23 #fa08fa
20,23 #fa08fa
8,24 #fa08fa
9,24 #fa08fa
10,24 #fa08fa
15,24 #fa08fa
20,24 #fa08fa
21,24 #fa08fa
8,25 #fa08fa
9,25 #fa08fa
10,25 #fa08fa
15,25 #fa08fa
20,25 #fa08fa
21,25 #fa08fa
9,26 #fa08fa
10,26 #fa08fa
20,26 #fa08fa
21,26 #fa08fa

Finished grid (row 0 first):
```
................................
................................
....bbb.............b.....b.....
...bcccb...........bab...bab....
..bcccccb..........bacb.bcab....
.becccccb..........baabbbaab....
baacccccb...........beeeeeeeb...
baaacccb...........baaaahfaaab..
baaaaab............baaaaffaaafb.
baaaaab............bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
..........baabgb.baabbggb.......
..........bggbfb.bggbbffb.......
..........bggbb.bggb.bffb.......
...........bggb.bggb..bffb......
...........bggb.bggb..bffb......
............bb...bb....bb.......
................................
................................
................................
................................
................................
```

## Frame 5: start from branch3/fox_walk_right_f5_v1.png, save as branch3/fox_walk_right_f5_v2.png

SET (62 px), grouped by colour:
#### #c4550c (key a) - 4 px
11,21 #c4550c
12,21 #c4550c
17,21 #c4550c
18,21 #c4550c
#### #3a2518 (key b) - 24 px
10,21 #3a2518
14,21 #3a2518
19,21 #3a2518
24,21 #3a2518
10,22 #3a2518
14,22 #3a2518
19,22 #3a2518
24,22 #3a2518
10,23 #3a2518
14,23 #3a2518
19,23 #3a2518
24,23 #3a2518
11,24 #3a2518
15,24 #3a2518
25,24 #3a2518
11,25 #3a2518
15,25 #3a2518
25,25 #3a2518
11,26 #3a2518
12,26 #3a2518
13,26 #3a2518
17,26 #3a2518
23,26 #3a2518
24,26 #3a2518
#### #3a1818 (key f) - 8 px
22,22 #3a1818
23,22 #3a1818
22,23 #3a1818
23,23 #3a1818
23,24 #3a1818
24,24 #3a1818
23,25 #3a1818
24,25 #3a1818
#### #884315 (key g) - 26 px
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
22,21 #884315
23,21 #884315
11,22 #884315
12,22 #884315
17,22 #884315
18,22 #884315
11,23 #884315
12,23 #884315
17,23 #884315
18,23 #884315
12,24 #884315
13,24 #884315
16,24 #884315
17,24 #884315
12,25 #884315
13,25 #884315
16,25 #884315
17,25 #884315

CLEAR back to magenta #fa08fa (31 px):
16,19 #fa08fa
8,21 #fa08fa
9,21 #fa08fa
15,21 #fa08fa
20,21 #fa08fa
8,22 #fa08fa
9,22 #fa08fa
15,22 #fa08fa
20,22 #fa08fa
8,23 #fa08fa
9,23 #fa08fa
15,23 #fa08fa
20,23 #fa08fa
7,24 #fa08fa
8,24 #fa08fa
9,24 #fa08fa
19,24 #fa08fa
20,24 #fa08fa
21,24 #fa08fa
7,25 #fa08fa
8,25 #fa08fa
9,25 #fa08fa
19,25 #fa08fa
20,25 #fa08fa
21,25 #fa08fa
8,26 #fa08fa
9,26 #fa08fa
15,26 #fa08fa
19,26 #fa08fa
20,26 #fa08fa
21,26 #fa08fa

Finished grid (row 0 first):
```
................................
................................
....................b.....b.....
....bbb............bab...bab....
...bcccb...........bacb.bcab....
..bcccccb..........baabbbaab....
.becccccb...........beeeeeeeb...
baacccccb..........baaaahfaaab..
baaacccb...........baaaaffaaafb.
baaaaab............bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
..........baabb.baab.bggb.......
..........bggbb.bggb.bffb.......
..........bggbb.bggb.bffb.......
..........bbggbbggb...bffb......
..........bbggbbggb...bffb......
...........bbb..bb.....bb.......
................................
................................
................................
................................
................................
```

## Frame 6: start from branch3/fox_walk_right_f6_v1.png, save as branch3/fox_walk_right_f6_v2.png

SET (52 px), grouped by colour:
#### #3a2518 (key b) - 19 px
9,22 #3a2518
14,22 #3a2518
16,22 #3a2518
19,22 #3a2518
23,22 #3a2518
10,23 #3a2518
14,23 #3a2518
19,23 #3a2518
24,23 #3a2518
10,24 #3a2518
14,24 #3a2518
19,24 #3a2518
24,24 #3a2518
17,25 #3a2518
24,25 #3a2518
11,26 #3a2518
12,26 #3a2518
22,26 #3a2518
23,26 #3a2518
#### #3a1818 (key f) - 8 px
13,22 #3a1818
22,22 #3a1818
22,23 #3a1818
23,23 #3a1818
22,24 #3a1818
23,24 #3a1818
22,25 #3a1818
23,25 #3a1818
#### #884315 (key g) - 25 px
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
13,21 #884315
14,21 #884315
21,21 #884315
22,21 #884315
11,22 #884315
17,22 #884315
18,22 #884315
11,23 #884315
12,23 #884315
17,23 #884315
18,23 #884315
11,24 #884315
12,24 #884315
17,24 #884315
18,24 #884315
11,25 #884315
12,25 #884315

CLEAR back to magenta #fa08fa (21 px):
16,19 #fa08fa
8,22 #fa08fa
15,22 #fa08fa
8,23 #fa08fa
9,23 #fa08fa
15,23 #fa08fa
20,23 #fa08fa
8,24 #fa08fa
9,24 #fa08fa
15,24 #fa08fa
20,24 #fa08fa
9,25 #fa08fa
14,25 #fa08fa
15,25 #fa08fa
16,25 #fa08fa
19,25 #fa08fa
20,25 #fa08fa
14,26 #fa08fa
15,26 #fa08fa
19,26 #fa08fa
20,26 #fa08fa

Finished grid (row 0 first):
```
................................
................................
....................b.....b.....
....bbb............bab...bab....
...bcccb...........bacb.bcab....
..bcccccb..........baabbbaab....
.becccccb...........beeeeeeeb...
baacccccb..........baaaahfaaab..
baaacccb...........baaaaffaaafb.
baaaaab............bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........bggbfb.bggbbffb........
..........bggbb.bggb.bffb.......
..........bggbb.bggb.bffb.......
..........bggb...bb..bffb.......
...........bb.........bb........
................................
................................
................................
................................
................................
```

## Frame 7: start from branch3/fox_walk_right_f7_v1.png, save as branch3/fox_walk_right_f7_v2.png

SET (54 px), grouped by colour:
#### #c4550c (key a) - 2 px
10,21 #c4550c
11,21 #c4550c
#### #3a2518 (key b) - 21 px
13,22 #3a2518
16,22 #3a2518
18,22 #3a2518
21,22 #3a2518
13,23 #3a2518
16,23 #3a2518
18,23 #3a2518
21,23 #3a2518
9,24 #3a2518
13,24 #3a2518
16,24 #3a2518
18,24 #3a2518
23,24 #3a2518
9,25 #3a2518
14,25 #3a2518
19,25 #3a2518
23,25 #3a2518
10,26 #3a2518
11,26 #3a2518
21,26 #3a2518
22,26 #3a2518
#### #3a1818 (key f) - 7 px
14,22 #3a1818
15,22 #3a1818
15,23 #3a1818
15,24 #3a1818
22,24 #3a1818
21,25 #3a1818
22,25 #3a1818
#### #884315 (key g) - 24 px
13,18 #884315
14,18 #884315
21,18 #884315
22,18 #884315
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
13,21 #884315
14,21 #884315
21,21 #884315
22,21 #884315
19,22 #884315
20,22 #884315
20,23 #884315
10,24 #884315
11,24 #884315
20,24 #884315
10,25 #884315
11,25 #884315

CLEAR back to magenta #fa08fa (11 px):
16,18 #fa08fa
17,22 #fa08fa
17,23 #fa08fa
17,24 #fa08fa
13,25 #fa08fa
17,25 #fa08fa
18,25 #fa08fa
13,26 #fa08fa
14,26 #fa08fa
18,26 #fa08fa
19,26 #fa08fa

Finished grid (row 0 first):
```
................................
....................b.....b.....
...................bab...bab....
....bbb............bacb.bcab....
...bcccb...........baabbbaab....
..bcccccb...........beeeeeeeb...
.becccccb..........baaaahfaaab..
baacccccb..........baaaaffaaafb.
baaacccb...........bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........bggbbffb.bggbfb........
.........bggbbffb.bggbfb........
.........bggbbffb.bggbfb........
.........bggb.bb...bbffb........
..........bb.........bb.........
................................
................................
................................
................................
................................
```

## Frame 8: start from branch3/fox_walk_right_f8_v1.png, save as branch3/fox_walk_right_f8_v2.png

SET (95 px), grouped by colour:
#### #c4550c (key a) - 11 px
1,6 #c4550c
2,6 #c4550c
1,7 #c4550c
2,7 #c4550c
3,7 #c4550c
3,8 #c4550c
4,8 #c4550c
5,8 #c4550c
4,9 #c4550c
5,9 #c4550c
20,21 #c4550c
#### #3a2518 (key b) - 39 px
4,2 #3a2518
5,2 #3a2518
6,2 #3a2518
3,3 #3a2518
7,3 #3a2518
2,4 #3a2518
8,4 #3a2518
1,5 #3a2518
8,5 #3a2518
0,6 #3a2518
0,7 #3a2518
7,7 #3a2518
6,8 #3a2518
6,9 #3a2518
13,21 #3a2518
16,21 #3a2518
18,21 #3a2518
21,21 #3a2518
9,22 #3a2518
12,22 #3a2518
16,22 #3a2518
18,22 #3a2518
23,22 #3a2518
8,23 #3a2518
11,23 #3a2518
18,23 #3a2518
22,23 #3a2518
8,24 #3a2518
11,24 #3a2518
17,24 #3a2518
22,24 #3a2518
8,25 #3a2518
17,25 #3a2518
9,26 #3a2518
10,26 #3a2518
15,26 #3a2518
16,26 #3a2518
20,26 #3a2518
21,26 #3a2518
#### #eec991 (key c) - 10 px
4,3 #eec991
5,3 #eec991
6,3 #eec991
3,4 #eec991
4,4 #eec991
5,4 #eec991
6,4 #eec991
7,4 #eec991
3,5 #eec991
7,5 #eec991
#### #f5b658 (key e) - 1 px
2,5 #f5b658
#### #3a1818 (key f) - 8 px
14,22 #3a1818
15,22 #3a1818
14,23 #3a1818
15,23 #3a1818
15,24 #3a1818
16,24 #3a1818
15,25 #3a1818
16,25 #3a1818
#### #884315 (key g) - 26 px
13,19 #884315
14,19 #884315
21,19 #884315
22,19 #884315
13,20 #884315
14,20 #884315
21,20 #884315
22,20 #884315
14,21 #884315
15,21 #884315
22,21 #884315
10,22 #884315
19,22 #884315
20,22 #884315
9,23 #884315
10,23 #884315
19,23 #884315
20,23 #884315
9,24 #884315
10,24 #884315
20,24 #884315
21,24 #884315
9,25 #884315
10,25 #884315
20,25 #884315
21,25 #884315

CLEAR back to magenta #fa08fa (25 px):
8,7 #fa08fa
7,8 #fa08fa
8,8 #fa08fa
7,9 #fa08fa
16,19 #fa08fa
17,21 #fa08fa
17,22 #fa08fa
24,22 #fa08fa
12,23 #fa08fa
17,23 #fa08fa
23,23 #fa08fa
24,23 #fa08fa
12,24 #fa08fa
13,24 #fa08fa
18,24 #fa08fa
23,24 #fa08fa
24,24 #fa08fa
12,25 #fa08fa
13,25 #fa08fa
18,25 #fa08fa
23,25 #fa08fa
12,26 #fa08fa
13,26 #fa08fa
17,26 #fa08fa
18,26 #fa08fa

Finished grid (row 0 first):
```
................................
................................
....bbb.............b.....b.....
...bcccb...........bab...bab....
..bcccccb..........bacb.bcab....
.becccccb..........baabbbaab....
baacccccb...........beeeeeeeb...
baaacccb...........baaaahfaaab..
baaaaab............baaaaffaaafb.
baaaaab............bacccaacccab.
baaaaab.bb.........baccccccccb..
baaaaabbeebbbbbbbbbbcaccccabb...
baaaaaaeeeeeeeeeeeeaccccbbb.....
baaaaaaaaaeeeeeeeeeeecccb.......
.baaaaaaaaaaaaaaaaaaacccb.......
..baaaaaaaaaaaaaaaaaacccb.......
...baaaaaaaaaaaaaaaaacccb.......
....bbbbbbdddddddddddcccb.......
.........baddddddddddccb........
.........baabggb.baabggb........
.........baabggb.baabggb........
.........baabbggb.baabgb........
.........bggbbffb.bggbfb........
........bggb.bffb.bggbb.........
........bggb..bffb.bggb.........
........bggb..bffb.bggb.........
.........bb....bb...bb..........
................................
................................
................................
................................
................................
```
