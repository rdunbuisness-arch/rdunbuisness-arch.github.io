# Fox walk right - click-in fixes (Artist 3)

- Base: /workspace/studio/branch1/fox_v2.png (512x512 export = **64x64** native at 8x). Base already **faces right**: no mirroring.
- Background: native #c5cded (key a) kept as in the base.
- Ground: paw row y=50, paw outline row y=51, same in every frame. Body/head x never changes (no drift).
- Output names: branch3/fox_walk_right_f<N>_v1.png (N=1..8). Loop f8 -> f1.
- Planning aid GIF: fox_walk_right_preview.gif (8 fps); per-frame previews fox_walk_right_f<N>_preview_8x.png.

## Frame 1 - full map

Palette (key = hex):
  a = #c5cded
  b = #c4550c
  c = #3a2518
  d = #a64c10
  e = #f5b658
  f = #eec991
  g = #3a1818
  h = #884315

Full grid, row 0 first:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbffffcaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaacccccccccccccaacbbbbbfffffcaaaaaaaaaaaaa
aaaaaaaacccccccccacccccceeeeeeeeeeeeeccbbbbbfffffccaaaaaaaaaaaaa
aaaacccceeeeeeeeecccceeeeeeeeeeeeeeeeeebbbbfffffccaaaaaaaaaaaaaa
aaacffffeeeeeeeeeeceeeeeeeeeeeeeeeeeeeeeeeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddcccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccacacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddddddddddddddddddcbbccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddddddddddddddddddcbbccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbcccccccccccccccccccbbcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbccaaaaaaaaaaaaaaaccbbcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbccaaaaaaaaaaaaaaaccbbcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbccaaaaaaaaaaaaaaacbbcaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaccbbcaaaaaaaaaaaaaaacbbcaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacggchhcaaaaaaaaaaaaachhcggcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacggcchhcaaaaaaaaaaaachhccggcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacgggchhhcaaaaaaaaaaachhhcgggcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacccacccaaaaaaaaaaaaacccacccaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Every pixel grouped by colour (x,y hex):
#### #c5cded (key a) - 3203 px
0,0 #c5cded
1,0 #c5cded
2,0 #c5cded
3,0 #c5cded
4,0 #c5cded
5,0 #c5cded
6,0 #c5cded
7,0 #c5cded
8,0 #c5cded
9,0 #c5cded
10,0 #c5cded
11,0 #c5cded
12,0 #c5cded
13,0 #c5cded
14,0 #c5cded
15,0 #c5cded
16,0 #c5cded
17,0 #c5cded
18,0 #c5cded
19,0 #c5cded
20,0 #c5cded
21,0 #c5cded
22,0 #c5cded
23,0 #c5cded
24,0 #c5cded
25,0 #c5cded
26,0 #c5cded
27,0 #c5cded
28,0 #c5cded
29,0 #c5cded
30,0 #c5cded
31,0 #c5cded
32,0 #c5cded
33,0 #c5cded
34,0 #c5cded
35,0 #c5cded
36,0 #c5cded
37,0 #c5cded
38,0 #c5cded
39,0 #c5cded
40,0 #c5cded
41,0 #c5cded
42,0 #c5cded
43,0 #c5cded
44,0 #c5cded
45,0 #c5cded
46,0 #c5cded
47,0 #c5cded
48,0 #c5cded
49,0 #c5cded
50,0 #c5cded
51,0 #c5cded
52,0 #c5cded
53,0 #c5cded
54,0 #c5cded
55,0 #c5cded
56,0 #c5cded
57,0 #c5cded
58,0 #c5cded
59,0 #c5cded
60,0 #c5cded
61,0 #c5cded
62,0 #c5cded
63,0 #c5cded
0,1 #c5cded
1,1 #c5cded
2,1 #c5cded
3,1 #c5cded
4,1 #c5cded
5,1 #c5cded
6,1 #c5cded
7,1 #c5cded
8,1 #c5cded
9,1 #c5cded
10,1 #c5cded
11,1 #c5cded
12,1 #c5cded
13,1 #c5cded
14,1 #c5cded
15,1 #c5cded
16,1 #c5cded
17,1 #c5cded
18,1 #c5cded
19,1 #c5cded
20,1 #c5cded
21,1 #c5cded
22,1 #c5cded
23,1 #c5cded
24,1 #c5cded
25,1 #c5cded
26,1 #c5cded
27,1 #c5cded
28,1 #c5cded
29,1 #c5cded
30,1 #c5cded
31,1 #c5cded
32,1 #c5cded
33,1 #c5cded
34,1 #c5cded
35,1 #c5cded
36,1 #c5cded
37,1 #c5cded
38,1 #c5cded
39,1 #c5cded
40,1 #c5cded
41,1 #c5cded
42,1 #c5cded
43,1 #c5cded
44,1 #c5cded
45,1 #c5cded
46,1 #c5cded
47,1 #c5cded
48,1 #c5cded
49,1 #c5cded
50,1 #c5cded
51,1 #c5cded
52,1 #c5cded
53,1 #c5cded
54,1 #c5cded
55,1 #c5cded
56,1 #c5cded
57,1 #c5cded
58,1 #c5cded
59,1 #c5cded
60,1 #c5cded
61,1 #c5cded
62,1 #c5cded
63,1 #c5cded
0,2 #c5cded
1,2 #c5cded
2,2 #c5cded
3,2 #c5cded
4,2 #c5cded
5,2 #c5cded
6,2 #c5cded
7,2 #c5cded
8,2 #c5cded
9,2 #c5cded
10,2 #c5cded
11,2 #c5cded
12,2 #c5cded
13,2 #c5cded
14,2 #c5cded
15,2 #c5cded
16,2 #c5cded
17,2 #c5cded
18,2 #c5cded
19,2 #c5cded
20,2 #c5cded
21,2 #c5cded
22,2 #c5cded
23,2 #c5cded
24,2 #c5cded
25,2 #c5cded
26,2 #c5cded
27,2 #c5cded
28,2 #c5cded
29,2 #c5cded
30,2 #c5cded
31,2 #c5cded
32,2 #c5cded
33,2 #c5cded
34,2 #c5cded
35,2 #c5cded
36,2 #c5cded
37,2 #c5cded
38,2 #c5cded
39,2 #c5cded
40,2 #c5cded
41,2 #c5cded
42,2 #c5cded
43,2 #c5cded
44,2 #c5cded
45,2 #c5cded
46,2 #c5cded
47,2 #c5cded
48,2 #c5cded
49,2 #c5cded
50,2 #c5cded
51,2 #c5cded
52,2 #c5cded
53,2 #c5cded
54,2 #c5cded
55,2 #c5cded
56,2 #c5cded
57,2 #c5cded
58,2 #c5cded
59,2 #c5cded
60,2 #c5cded
61,2 #c5cded
62,2 #c5cded
63,2 #c5cded
0,3 #c5cded
1,3 #c5cded
2,3 #c5cded
3,3 #c5cded
4,3 #c5cded
5,3 #c5cded
6,3 #c5cded
7,3 #c5cded
8,3 #c5cded
9,3 #c5cded
10,3 #c5cded
11,3 #c5cded
12,3 #c5cded
13,3 #c5cded
14,3 #c5cded
15,3 #c5cded
16,3 #c5cded
17,3 #c5cded
18,3 #c5cded
19,3 #c5cded
20,3 #c5cded
21,3 #c5cded
22,3 #c5cded
23,3 #c5cded
24,3 #c5cded
25,3 #c5cded
26,3 #c5cded
27,3 #c5cded
28,3 #c5cded
29,3 #c5cded
30,3 #c5cded
31,3 #c5cded
32,3 #c5cded
33,3 #c5cded
34,3 #c5cded
35,3 #c5cded
36,3 #c5cded
37,3 #c5cded
38,3 #c5cded
39,3 #c5cded
40,3 #c5cded
41,3 #c5cded
42,3 #c5cded
43,3 #c5cded
44,3 #c5cded
45,3 #c5cded
46,3 #c5cded
47,3 #c5cded
48,3 #c5cded
49,3 #c5cded
50,3 #c5cded
51,3 #c5cded
52,3 #c5cded
53,3 #c5cded
54,3 #c5cded
55,3 #c5cded
56,3 #c5cded
57,3 #c5cded
58,3 #c5cded
59,3 #c5cded
60,3 #c5cded
61,3 #c5cded
62,3 #c5cded
63,3 #c5cded
0,4 #c5cded
1,4 #c5cded
2,4 #c5cded
3,4 #c5cded
4,4 #c5cded
5,4 #c5cded
6,4 #c5cded
7,4 #c5cded
8,4 #c5cded
9,4 #c5cded
10,4 #c5cded
11,4 #c5cded
12,4 #c5cded
13,4 #c5cded
14,4 #c5cded
15,4 #c5cded
16,4 #c5cded
17,4 #c5cded
18,4 #c5cded
19,4 #c5cded
20,4 #c5cded
21,4 #c5cded
22,4 #c5cded
23,4 #c5cded
24,4 #c5cded
25,4 #c5cded
26,4 #c5cded
27,4 #c5cded
28,4 #c5cded
29,4 #c5cded
30,4 #c5cded
31,4 #c5cded
32,4 #c5cded
33,4 #c5cded
34,4 #c5cded
35,4 #c5cded
36,4 #c5cded
37,4 #c5cded
38,4 #c5cded
39,4 #c5cded
40,4 #c5cded
41,4 #c5cded
42,4 #c5cded
43,4 #c5cded
44,4 #c5cded
45,4 #c5cded
46,4 #c5cded
47,4 #c5cded
48,4 #c5cded
49,4 #c5cded
50,4 #c5cded
51,4 #c5cded
52,4 #c5cded
53,4 #c5cded
54,4 #c5cded
55,4 #c5cded
56,4 #c5cded
57,4 #c5cded
58,4 #c5cded
59,4 #c5cded
60,4 #c5cded
61,4 #c5cded
62,4 #c5cded
63,4 #c5cded
0,5 #c5cded
1,5 #c5cded
2,5 #c5cded
3,5 #c5cded
4,5 #c5cded
5,5 #c5cded
6,5 #c5cded
7,5 #c5cded
8,5 #c5cded
9,5 #c5cded
10,5 #c5cded
11,5 #c5cded
12,5 #c5cded
13,5 #c5cded
14,5 #c5cded
15,5 #c5cded
16,5 #c5cded
17,5 #c5cded
18,5 #c5cded
19,5 #c5cded
20,5 #c5cded
21,5 #c5cded
22,5 #c5cded
23,5 #c5cded
24,5 #c5cded
25,5 #c5cded
26,5 #c5cded
27,5 #c5cded
28,5 #c5cded
29,5 #c5cded
30,5 #c5cded
31,5 #c5cded
32,5 #c5cded
33,5 #c5cded
34,5 #c5cded
35,5 #c5cded
36,5 #c5cded
37,5 #c5cded
38,5 #c5cded
39,5 #c5cded
40,5 #c5cded
41,5 #c5cded
42,5 #c5cded
43,5 #c5cded
44,5 #c5cded
45,5 #c5cded
46,5 #c5cded
47,5 #c5cded
48,5 #c5cded
49,5 #c5cded
50,5 #c5cded
51,5 #c5cded
52,5 #c5cded
53,5 #c5cded
54,5 #c5cded
55,5 #c5cded
56,5 #c5cded
57,5 #c5cded
58,5 #c5cded
59,5 #c5cded
60,5 #c5cded
61,5 #c5cded
62,5 #c5cded
63,5 #c5cded
0,6 #c5cded
1,6 #c5cded
2,6 #c5cded
3,6 #c5cded
4,6 #c5cded
5,6 #c5cded
6,6 #c5cded
7,6 #c5cded
8,6 #c5cded
9,6 #c5cded
10,6 #c5cded
11,6 #c5cded
12,6 #c5cded
13,6 #c5cded
14,6 #c5cded
15,6 #c5cded
16,6 #c5cded
17,6 #c5cded
18,6 #c5cded
19,6 #c5cded
20,6 #c5cded
21,6 #c5cded
22,6 #c5cded
23,6 #c5cded
24,6 #c5cded
25,6 #c5cded
26,6 #c5cded
27,6 #c5cded
28,6 #c5cded
29,6 #c5cded
30,6 #c5cded
31,6 #c5cded
32,6 #c5cded
33,6 #c5cded
34,6 #c5cded
35,6 #c5cded
36,6 #c5cded
37,6 #c5cded
38,6 #c5cded
39,6 #c5cded
40,6 #c5cded
41,6 #c5cded
42,6 #c5cded
43,6 #c5cded
44,6 #c5cded
45,6 #c5cded
46,6 #c5cded
47,6 #c5cded
48,6 #c5cded
49,6 #c5cded
50,6 #c5cded
51,6 #c5cded
52,6 #c5cded
53,6 #c5cded
54,6 #c5cded
55,6 #c5cded
56,6 #c5cded
57,6 #c5cded
58,6 #c5cded
59,6 #c5cded
60,6 #c5cded
61,6 #c5cded
62,6 #c5cded
63,6 #c5cded
0,7 #c5cded
1,7 #c5cded
2,7 #c5cded
3,7 #c5cded
4,7 #c5cded
5,7 #c5cded
6,7 #c5cded
7,7 #c5cded
8,7 #c5cded
9,7 #c5cded
10,7 #c5cded
11,7 #c5cded
12,7 #c5cded
13,7 #c5cded
14,7 #c5cded
15,7 #c5cded
16,7 #c5cded
17,7 #c5cded
18,7 #c5cded
19,7 #c5cded
20,7 #c5cded
21,7 #c5cded
22,7 #c5cded
23,7 #c5cded
24,7 #c5cded
25,7 #c5cded
26,7 #c5cded
27,7 #c5cded
28,7 #c5cded
29,7 #c5cded
30,7 #c5cded
31,7 #c5cded
32,7 #c5cded
33,7 #c5cded
34,7 #c5cded
35,7 #c5cded
36,7 #c5cded
37,7 #c5cded
38,7 #c5cded
39,7 #c5cded
40,7 #c5cded
41,7 #c5cded
42,7 #c5cded
43,7 #c5cded
44,7 #c5cded
45,7 #c5cded
47,7 #c5cded
48,7 #c5cded
49,7 #c5cded
50,7 #c5cded
52,7 #c5cded
53,7 #c5cded
54,7 #c5cded
55,7 #c5cded
56,7 #c5cded
57,7 #c5cded
58,7 #c5cded
59,7 #c5cded
60,7 #c5cded
61,7 #c5cded
62,7 #c5cded
63,7 #c5cded
0,8 #c5cded
1,8 #c5cded
2,8 #c5cded
3,8 #c5cded
4,8 #c5cded
5,8 #c5cded
6,8 #c5cded
7,8 #c5cded
8,8 #c5cded
9,8 #c5cded
10,8 #c5cded
11,8 #c5cded
12,8 #c5cded
13,8 #c5cded
14,8 #c5cded
15,8 #c5cded
16,8 #c5cded
17,8 #c5cded
18,8 #c5cded
19,8 #c5cded
20,8 #c5cded
21,8 #c5cded
22,8 #c5cded
23,8 #c5cded
24,8 #c5cded
25,8 #c5cded
26,8 #c5cded
27,8 #c5cded
28,8 #c5cded
29,8 #c5cded
30,8 #c5cded
31,8 #c5cded
32,8 #c5cded
33,8 #c5cded
34,8 #c5cded
35,8 #c5cded
36,8 #c5cded
37,8 #c5cded
38,8 #c5cded
39,8 #c5cded
40,8 #c5cded
41,8 #c5cded
42,8 #c5cded
43,8 #c5cded
44,8 #c5cded
48,8 #c5cded
49,8 #c5cded
53,8 #c5cded
54,8 #c5cded
55,8 #c5cded
56,8 #c5cded
57,8 #c5cded
58,8 #c5cded
59,8 #c5cded
60,8 #c5cded
61,8 #c5cded
62,8 #c5cded
63,8 #c5cded
0,9 #c5cded
1,9 #c5cded
2,9 #c5cded
3,9 #c5cded
4,9 #c5cded
5,9 #c5cded
6,9 #c5cded
7,9 #c5cded
8,9 #c5cded
9,9 #c5cded
10,9 #c5cded
11,9 #c5cded
12,9 #c5cded
13,9 #c5cded
14,9 #c5cded
15,9 #c5cded
16,9 #c5cded
17,9 #c5cded
18,9 #c5cded
19,9 #c5cded
20,9 #c5cded
21,9 #c5cded
22,9 #c5cded
23,9 #c5cded
24,9 #c5cded
25,9 #c5cded
26,9 #c5cded
27,9 #c5cded
28,9 #c5cded
29,9 #c5cded
30,9 #c5cded
31,9 #c5cded
32,9 #c5cded
33,9 #c5cded
34,9 #c5cded
35,9 #c5cded
36,9 #c5cded
37,9 #c5cded
38,9 #c5cded
39,9 #c5cded
40,9 #c5cded
41,9 #c5cded
42,9 #c5cded
43,9 #c5cded
44,9 #c5cded
48,9 #c5cded
49,9 #c5cded
53,9 #c5cded
54,9 #c5cded
55,9 #c5cded
56,9 #c5cded
57,9 #c5cded
58,9 #c5cded
59,9 #c5cded
60,9 #c5cded
61,9 #c5cded
62,9 #c5cded
63,9 #c5cded
0,10 #c5cded
1,10 #c5cded
2,10 #c5cded
3,10 #c5cded
4,10 #c5cded
5,10 #c5cded
6,10 #c5cded
7,10 #c5cded
8,10 #c5cded
9,10 #c5cded
10,10 #c5cded
11,10 #c5cded
12,10 #c5cded
13,10 #c5cded
14,10 #c5cded
15,10 #c5cded
16,10 #c5cded
17,10 #c5cded
18,10 #c5cded
19,10 #c5cded
20,10 #c5cded
21,10 #c5cded
22,10 #c5cded
23,10 #c5cded
24,10 #c5cded
25,10 #c5cded
26,10 #c5cded
27,10 #c5cded
28,10 #c5cded
29,10 #c5cded
30,10 #c5cded
31,10 #c5cded
32,10 #c5cded
33,10 #c5cded
34,10 #c5cded
35,10 #c5cded
36,10 #c5cded
37,10 #c5cded
38,10 #c5cded
39,10 #c5cded
40,10 #c5cded
41,10 #c5cded
42,10 #c5cded
43,10 #c5cded
54,10 #c5cded
55,10 #c5cded
56,10 #c5cded
57,10 #c5cded
58,10 #c5cded
59,10 #c5cded
60,10 #c5cded
61,10 #c5cded
62,10 #c5cded
63,10 #c5cded
0,11 #c5cded
1,11 #c5cded
2,11 #c5cded
3,11 #c5cded
4,11 #c5cded
5,11 #c5cded
6,11 #c5cded
7,11 #c5cded
8,11 #c5cded
9,11 #c5cded
10,11 #c5cded
11,11 #c5cded
12,11 #c5cded
13,11 #c5cded
14,11 #c5cded
15,11 #c5cded
16,11 #c5cded
17,11 #c5cded
18,11 #c5cded
19,11 #c5cded
20,11 #c5cded
21,11 #c5cded
22,11 #c5cded
23,11 #c5cded
24,11 #c5cded
25,11 #c5cded
26,11 #c5cded
27,11 #c5cded
28,11 #c5cded
29,11 #c5cded
30,11 #c5cded
31,11 #c5cded
32,11 #c5cded
33,11 #c5cded
34,11 #c5cded
35,11 #c5cded
36,11 #c5cded
37,11 #c5cded
38,11 #c5cded
39,11 #c5cded
40,11 #c5cded
41,11 #c5cded
42,11 #c5cded
43,11 #c5cded
54,11 #c5cded
55,11 #c5cded
56,11 #c5cded
57,11 #c5cded
58,11 #c5cded
59,11 #c5cded
60,11 #c5cded
61,11 #c5cded
62,11 #c5cded
63,11 #c5cded
0,12 #c5cded
1,12 #c5cded
2,12 #c5cded
3,12 #c5cded
4,12 #c5cded
5,12 #c5cded
6,12 #c5cded
7,12 #c5cded
8,12 #c5cded
9,12 #c5cded
10,12 #c5cded
11,12 #c5cded
12,12 #c5cded
13,12 #c5cded
14,12 #c5cded
15,12 #c5cded
16,12 #c5cded
17,12 #c5cded
18,12 #c5cded
19,12 #c5cded
20,12 #c5cded
21,12 #c5cded
22,12 #c5cded
23,12 #c5cded
24,12 #c5cded
25,12 #c5cded
26,12 #c5cded
27,12 #c5cded
28,12 #c5cded
29,12 #c5cded
30,12 #c5cded
31,12 #c5cded
32,12 #c5cded
33,12 #c5cded
34,12 #c5cded
35,12 #c5cded
36,12 #c5cded
37,12 #c5cded
38,12 #c5cded
39,12 #c5cded
40,12 #c5cded
41,12 #c5cded
42,12 #c5cded
43,12 #c5cded
55,12 #c5cded
56,12 #c5cded
57,12 #c5cded
58,12 #c5cded
59,12 #c5cded
60,12 #c5cded
61,12 #c5cded
62,12 #c5cded
63,12 #c5cded
0,13 #c5cded
1,13 #c5cded
2,13 #c5cded
3,13 #c5cded
4,13 #c5cded
5,13 #c5cded
6,13 #c5cded
7,13 #c5cded
8,13 #c5cded
9,13 #c5cded
10,13 #c5cded
11,13 #c5cded
12,13 #c5cded
13,13 #c5cded
14,13 #c5cded
15,13 #c5cded
16,13 #c5cded
17,13 #c5cded
18,13 #c5cded
19,13 #c5cded
20,13 #c5cded
21,13 #c5cded
22,13 #c5cded
23,13 #c5cded
24,13 #c5cded
25,13 #c5cded
26,13 #c5cded
27,13 #c5cded
28,13 #c5cded
29,13 #c5cded
30,13 #c5cded
31,13 #c5cded
32,13 #c5cded
33,13 #c5cded
34,13 #c5cded
35,13 #c5cded
36,13 #c5cded
37,13 #c5cded
38,13 #c5cded
39,13 #c5cded
40,13 #c5cded
41,13 #c5cded
42,13 #c5cded
43,13 #c5cded
55,13 #c5cded
56,13 #c5cded
57,13 #c5cded
58,13 #c5cded
59,13 #c5cded
60,13 #c5cded
61,13 #c5cded
62,13 #c5cded
63,13 #c5cded
0,14 #c5cded
1,14 #c5cded
2,14 #c5cded
3,14 #c5cded
4,14 #c5cded
5,14 #c5cded
6,14 #c5cded
7,14 #c5cded
8,14 #c5cded
9,14 #c5cded
10,14 #c5cded
11,14 #c5cded
12,14 #c5cded
13,14 #c5cded
14,14 #c5cded
15,14 #c5cded
16,14 #c5cded
17,14 #c5cded
18,14 #c5cded
19,14 #c5cded
20,14 #c5cded
21,14 #c5cded
22,14 #c5cded
23,14 #c5cded
24,14 #c5cded
25,14 #c5cded
26,14 #c5cded
27,14 #c5cded
28,14 #c5cded
29,14 #c5cded
30,14 #c5cded
31,14 #c5cded
32,14 #c5cded
33,14 #c5cded
34,14 #c5cded
35,14 #c5cded
36,14 #c5cded
37,14 #c5cded
38,14 #c5cded
39,14 #c5cded
40,14 #c5cded
41,14 #c5cded
42,14 #c5cded
43,14 #c5cded
55,14 #c5cded
56,14 #c5cded
57,14 #c5cded
58,14 #c5cded
59,14 #c5cded
60,14 #c5cded
61,14 #c5cded
62,14 #c5cded
63,14 #c5cded
0,15 #c5cded
1,15 #c5cded
2,15 #c5cded
3,15 #c5cded
4,15 #c5cded
5,15 #c5cded
6,15 #c5cded
7,15 #c5cded
8,15 #c5cded
9,15 #c5cded
10,15 #c5cded
11,15 #c5cded
12,15 #c5cded
13,15 #c5cded
14,15 #c5cded
15,15 #c5cded
16,15 #c5cded
17,15 #c5cded
18,15 #c5cded
19,15 #c5cded
20,15 #c5cded
21,15 #c5cded
22,15 #c5cded
23,15 #c5cded
24,15 #c5cded
25,15 #c5cded
26,15 #c5cded
27,15 #c5cded
28,15 #c5cded
29,15 #c5cded
30,15 #c5cded
31,15 #c5cded
32,15 #c5cded
33,15 #c5cded
34,15 #c5cded
35,15 #c5cded
36,15 #c5cded
37,15 #c5cded
38,15 #c5cded
39,15 #c5cded
40,15 #c5cded
41,15 #c5cded
42,15 #c5cded
43,15 #c5cded
54,15 #c5cded
55,15 #c5cded
56,15 #c5cded
57,15 #c5cded
58,15 #c5cded
59,15 #c5cded
60,15 #c5cded
61,15 #c5cded
62,15 #c5cded
63,15 #c5cded
0,16 #c5cded
1,16 #c5cded
2,16 #c5cded
3,16 #c5cded
4,16 #c5cded
5,16 #c5cded
6,16 #c5cded
7,16 #c5cded
8,16 #c5cded
9,16 #c5cded
10,16 #c5cded
11,16 #c5cded
12,16 #c5cded
13,16 #c5cded
14,16 #c5cded
15,16 #c5cded
16,16 #c5cded
17,16 #c5cded
18,16 #c5cded
19,16 #c5cded
20,16 #c5cded
21,16 #c5cded
22,16 #c5cded
23,16 #c5cded
24,16 #c5cded
25,16 #c5cded
26,16 #c5cded
27,16 #c5cded
28,16 #c5cded
29,16 #c5cded
30,16 #c5cded
31,16 #c5cded
32,16 #c5cded
33,16 #c5cded
34,16 #c5cded
35,16 #c5cded
36,16 #c5cded
37,16 #c5cded
38,16 #c5cded
39,16 #c5cded
40,16 #c5cded
41,16 #c5cded
42,16 #c5cded
55,16 #c5cded
56,16 #c5cded
57,16 #c5cded
58,16 #c5cded
59,16 #c5cded
60,16 #c5cded
61,16 #c5cded
62,16 #c5cded
63,16 #c5cded
0,17 #c5cded
1,17 #c5cded
2,17 #c5cded
3,17 #c5cded
4,17 #c5cded
5,17 #c5cded
6,17 #c5cded
7,17 #c5cded
8,17 #c5cded
9,17 #c5cded
10,17 #c5cded
11,17 #c5cded
12,17 #c5cded
13,17 #c5cded
14,17 #c5cded
15,17 #c5cded
16,17 #c5cded
17,17 #c5cded
18,17 #c5cded
19,17 #c5cded
20,17 #c5cded
21,17 #c5cded
22,17 #c5cded
23,17 #c5cded
24,17 #c5cded
25,17 #c5cded
26,17 #c5cded
27,17 #c5cded
28,17 #c5cded
29,17 #c5cded
30,17 #c5cded
31,17 #c5cded
32,17 #c5cded
33,17 #c5cded
34,17 #c5cded
35,17 #c5cded
36,17 #c5cded
37,17 #c5cded
38,17 #c5cded
39,17 #c5cded
40,17 #c5cded
41,17 #c5cded
42,17 #c5cded
56,17 #c5cded
57,17 #c5cded
58,17 #c5cded
59,17 #c5cded
60,17 #c5cded
61,17 #c5cded
62,17 #c5cded
63,17 #c5cded
0,18 #c5cded
1,18 #c5cded
2,18 #c5cded
3,18 #c5cded
4,18 #c5cded
5,18 #c5cded
6,18 #c5cded
7,18 #c5cded
8,18 #c5cded
9,18 #c5cded
10,18 #c5cded
11,18 #c5cded
12,18 #c5cded
13,18 #c5cded
14,18 #c5cded
15,18 #c5cded
16,18 #c5cded
17,18 #c5cded
18,18 #c5cded
19,18 #c5cded
20,18 #c5cded
21,18 #c5cded
22,18 #c5cded
23,18 #c5cded
24,18 #c5cded
25,18 #c5cded
26,18 #c5cded
27,18 #c5cded
28,18 #c5cded
29,18 #c5cded
30,18 #c5cded
31,18 #c5cded
32,18 #c5cded
33,18 #c5cded
34,18 #c5cded
35,18 #c5cded
36,18 #c5cded
37,18 #c5cded
38,18 #c5cded
39,18 #c5cded
40,18 #c5cded
41,18 #c5cded
42,18 #c5cded
59,18 #c5cded
60,18 #c5cded
61,18 #c5cded
62,18 #c5cded
63,18 #c5cded
0,19 #c5cded
1,19 #c5cded
2,19 #c5cded
3,19 #c5cded
4,19 #c5cded
5,19 #c5cded
6,19 #c5cded
7,19 #c5cded
8,19 #c5cded
9,19 #c5cded
10,19 #c5cded
11,19 #c5cded
12,19 #c5cded
13,19 #c5cded
14,19 #c5cded
15,19 #c5cded
16,19 #c5cded
17,19 #c5cded
18,19 #c5cded
19,19 #c5cded
20,19 #c5cded
21,19 #c5cded
22,19 #c5cded
23,19 #c5cded
24,19 #c5cded
25,19 #c5cded
26,19 #c5cded
27,19 #c5cded
28,19 #c5cded
29,19 #c5cded
30,19 #c5cded
31,19 #c5cded
32,19 #c5cded
33,19 #c5cded
34,19 #c5cded
35,19 #c5cded
36,19 #c5cded
37,19 #c5cded
38,19 #c5cded
39,19 #c5cded
40,19 #c5cded
41,19 #c5cded
42,19 #c5cded
61,19 #c5cded
62,19 #c5cded
63,19 #c5cded
0,20 #c5cded
1,20 #c5cded
2,20 #c5cded
3,20 #c5cded
4,20 #c5cded
5,20 #c5cded
6,20 #c5cded
7,20 #c5cded
8,20 #c5cded
9,20 #c5cded
10,20 #c5cded
11,20 #c5cded
12,20 #c5cded
13,20 #c5cded
14,20 #c5cded
15,20 #c5cded
16,20 #c5cded
17,20 #c5cded
18,20 #c5cded
19,20 #c5cded
20,20 #c5cded
21,20 #c5cded
22,20 #c5cded
23,20 #c5cded
24,20 #c5cded
25,20 #c5cded
26,20 #c5cded
27,20 #c5cded
28,20 #c5cded
29,20 #c5cded
30,20 #c5cded
31,20 #c5cded
32,20 #c5cded
33,20 #c5cded
34,20 #c5cded
35,20 #c5cded
36,20 #c5cded
37,20 #c5cded
38,20 #c5cded
39,20 #c5cded
40,20 #c5cded
41,20 #c5cded
42,20 #c5cded
62,20 #c5cded
63,20 #c5cded
0,21 #c5cded
1,21 #c5cded
2,21 #c5cded
3,21 #c5cded
4,21 #c5cded
5,21 #c5cded
6,21 #c5cded
7,21 #c5cded
8,21 #c5cded
9,21 #c5cded
10,21 #c5cded
11,21 #c5cded
12,21 #c5cded
13,21 #c5cded
14,21 #c5cded
15,21 #c5cded
16,21 #c5cded
17,21 #c5cded
18,21 #c5cded
19,21 #c5cded
20,21 #c5cded
21,21 #c5cded
22,21 #c5cded
23,21 #c5cded
24,21 #c5cded
25,21 #c5cded
26,21 #c5cded
27,21 #c5cded
28,21 #c5cded
29,21 #c5cded
30,21 #c5cded
31,21 #c5cded
32,21 #c5cded
33,21 #c5cded
34,21 #c5cded
35,21 #c5cded
36,21 #c5cded
37,21 #c5cded
38,21 #c5cded
39,21 #c5cded
40,21 #c5cded
41,21 #c5cded
42,21 #c5cded
61,21 #c5cded
62,21 #c5cded
63,21 #c5cded
0,22 #c5cded
1,22 #c5cded
2,22 #c5cded
3,22 #c5cded
4,22 #c5cded
5,22 #c5cded
6,22 #c5cded
7,22 #c5cded
8,22 #c5cded
9,22 #c5cded
10,22 #c5cded
11,22 #c5cded
12,22 #c5cded
13,22 #c5cded
14,22 #c5cded
15,22 #c5cded
16,22 #c5cded
17,22 #c5cded
18,22 #c5cded
19,22 #c5cded
20,22 #c5cded
21,22 #c5cded
22,22 #c5cded
23,22 #c5cded
24,22 #c5cded
25,22 #c5cded
26,22 #c5cded
27,22 #c5cded
28,22 #c5cded
29,22 #c5cded
30,22 #c5cded
31,22 #c5cded
32,22 #c5cded
33,22 #c5cded
34,22 #c5cded
35,22 #c5cded
36,22 #c5cded
37,22 #c5cded
38,22 #c5cded
39,22 #c5cded
40,22 #c5cded
41,22 #c5cded
59,22 #c5cded
60,22 #c5cded
61,22 #c5cded
62,22 #c5cded
63,22 #c5cded
0,23 #c5cded
1,23 #c5cded
2,23 #c5cded
3,23 #c5cded
4,23 #c5cded
5,23 #c5cded
6,23 #c5cded
7,23 #c5cded
8,23 #c5cded
9,23 #c5cded
10,23 #c5cded
11,23 #c5cded
12,23 #c5cded
13,23 #c5cded
14,23 #c5cded
15,23 #c5cded
16,23 #c5cded
17,23 #c5cded
18,23 #c5cded
19,23 #c5cded
20,23 #c5cded
21,23 #c5cded
22,23 #c5cded
23,23 #c5cded
24,23 #c5cded
25,23 #c5cded
26,23 #c5cded
27,23 #c5cded
28,23 #c5cded
29,23 #c5cded
30,23 #c5cded
31,23 #c5cded
32,23 #c5cded
33,23 #c5cded
34,23 #c5cded
35,23 #c5cded
36,23 #c5cded
37,23 #c5cded
38,23 #c5cded
39,23 #c5cded
40,23 #c5cded
59,23 #c5cded
60,23 #c5cded
61,23 #c5cded
62,23 #c5cded
63,23 #c5cded
0,24 #c5cded
1,24 #c5cded
2,24 #c5cded
3,24 #c5cded
4,24 #c5cded
5,24 #c5cded
6,24 #c5cded
7,24 #c5cded
8,24 #c5cded
9,24 #c5cded
10,24 #c5cded
11,24 #c5cded
12,24 #c5cded
13,24 #c5cded
14,24 #c5cded
15,24 #c5cded
16,24 #c5cded
17,24 #c5cded
18,24 #c5cded
19,24 #c5cded
20,24 #c5cded
21,24 #c5cded
22,24 #c5cded
23,24 #c5cded
24,24 #c5cded
25,24 #c5cded
26,24 #c5cded
27,24 #c5cded
28,24 #c5cded
29,24 #c5cded
30,24 #c5cded
31,24 #c5cded
32,24 #c5cded
33,24 #c5cded
34,24 #c5cded
35,24 #c5cded
36,24 #c5cded
37,24 #c5cded
38,24 #c5cded
39,24 #c5cded
51,24 #c5cded
52,24 #c5cded
53,24 #c5cded
54,24 #c5cded
55,24 #c5cded
56,24 #c5cded
57,24 #c5cded
58,24 #c5cded
59,24 #c5cded
60,24 #c5cded
61,24 #c5cded
62,24 #c5cded
63,24 #c5cded
0,25 #c5cded
1,25 #c5cded
2,25 #c5cded
3,25 #c5cded
4,25 #c5cded
5,25 #c5cded
6,25 #c5cded
7,25 #c5cded
8,25 #c5cded
9,25 #c5cded
10,25 #c5cded
11,25 #c5cded
12,25 #c5cded
13,25 #c5cded
14,25 #c5cded
15,25 #c5cded
16,25 #c5cded
17,25 #c5cded
18,25 #c5cded
19,25 #c5cded
20,25 #c5cded
21,25 #c5cded
22,25 #c5cded
23,25 #c5cded
37,25 #c5cded
38,25 #c5cded
51,25 #c5cded
52,25 #c5cded
53,25 #c5cded
54,25 #c5cded
55,25 #c5cded
56,25 #c5cded
57,25 #c5cded
58,25 #c5cded
59,25 #c5cded
60,25 #c5cded
61,25 #c5cded
62,25 #c5cded
63,25 #c5cded
0,26 #c5cded
1,26 #c5cded
2,26 #c5cded
3,26 #c5cded
4,26 #c5cded
5,26 #c5cded
6,26 #c5cded
7,26 #c5cded
17,26 #c5cded
51,26 #c5cded
52,26 #c5cded
53,26 #c5cded
54,26 #c5cded
55,26 #c5cded
56,26 #c5cded
57,26 #c5cded
58,26 #c5cded
59,26 #c5cded
60,26 #c5cded
61,26 #c5cded
62,26 #c5cded
63,26 #c5cded
0,27 #c5cded
1,27 #c5cded
2,27 #c5cded
3,27 #c5cded
50,27 #c5cded
51,27 #c5cded
52,27 #c5cded
53,27 #c5cded
54,27 #c5cded
55,27 #c5cded
56,27 #c5cded
57,27 #c5cded
58,27 #c5cded
59,27 #c5cded
60,27 #c5cded
61,27 #c5cded
62,27 #c5cded
63,27 #c5cded
0,28 #c5cded
1,28 #c5cded
2,28 #c5cded
49,28 #c5cded
50,28 #c5cded
51,28 #c5cded
52,28 #c5cded
53,28 #c5cded
54,28 #c5cded
55,28 #c5cded
56,28 #c5cded
57,28 #c5cded
58,28 #c5cded
59,28 #c5cded
60,28 #c5cded
61,28 #c5cded
62,28 #c5cded
63,28 #c5cded
0,29 #c5cded
1,29 #c5cded
48,29 #c5cded
49,29 #c5cded
50,29 #c5cded
51,29 #c5cded
52,29 #c5cded
53,29 #c5cded
54,29 #c5cded
55,29 #c5cded
56,29 #c5cded
57,29 #c5cded
58,29 #c5cded
59,29 #c5cded
60,29 #c5cded
61,29 #c5cded
62,29 #c5cded
63,29 #c5cded
0,30 #c5cded
1,30 #c5cded
46,30 #c5cded
47,30 #c5cded
48,30 #c5cded
49,30 #c5cded
50,30 #c5cded
51,30 #c5cded
52,30 #c5cded
53,30 #c5cded
54,30 #c5cded
55,30 #c5cded
56,30 #c5cded
57,30 #c5cded
58,30 #c5cded
59,30 #c5cded
60,30 #c5cded
61,30 #c5cded
62,30 #c5cded
63,30 #c5cded
0,31 #c5cded
1,31 #c5cded
46,31 #c5cded
47,31 #c5cded
48,31 #c5cded
49,31 #c5cded
50,31 #c5cded
51,31 #c5cded
52,31 #c5cded
53,31 #c5cded
54,31 #c5cded
55,31 #c5cded
56,31 #c5cded
57,31 #c5cded
58,31 #c5cded
59,31 #c5cded
60,31 #c5cded
61,31 #c5cded
62,31 #c5cded
63,31 #c5cded
0,32 #c5cded
1,32 #c5cded
2,32 #c5cded
46,32 #c5cded
47,32 #c5cded
48,32 #c5cded
49,32 #c5cded
50,32 #c5cded
51,32 #c5cded
52,32 #c5cded
53,32 #c5cded
54,32 #c5cded
55,32 #c5cded
56,32 #c5cded
57,32 #c5cded
58,32 #c5cded
59,32 #c5cded
60,32 #c5cded
61,32 #c5cded
62,32 #c5cded
63,32 #c5cded
0,33 #c5cded
1,33 #c5cded
2,33 #c5cded
3,33 #c5cded
4,33 #c5cded
46,33 #c5cded
47,33 #c5cded
48,33 #c5cded
49,33 #c5cded
50,33 #c5cded
51,33 #c5cded
52,33 #c5cded
53,33 #c5cded
54,33 #c5cded
55,33 #c5cded
56,33 #c5cded
57,33 #c5cded
58,33 #c5cded
59,33 #c5cded
60,33 #c5cded
61,33 #c5cded
62,33 #c5cded
63,33 #c5cded
0,34 #c5cded
1,34 #c5cded
2,34 #c5cded
3,34 #c5cded
4,34 #c5cded
5,34 #c5cded
16,34 #c5cded
18,34 #c5cded
46,34 #c5cded
47,34 #c5cded
48,34 #c5cded
49,34 #c5cded
50,34 #c5cded
51,34 #c5cded
52,34 #c5cded
53,34 #c5cded
54,34 #c5cded
55,34 #c5cded
56,34 #c5cded
57,34 #c5cded
58,34 #c5cded
59,34 #c5cded
60,34 #c5cded
61,34 #c5cded
62,34 #c5cded
63,34 #c5cded
0,35 #c5cded
1,35 #c5cded
2,35 #c5cded
3,35 #c5cded
4,35 #c5cded
5,35 #c5cded
6,35 #c5cded
7,35 #c5cded
8,35 #c5cded
9,35 #c5cded
10,35 #c5cded
11,35 #c5cded
12,35 #c5cded
13,35 #c5cded
14,35 #c5cded
15,35 #c5cded
16,35 #c5cded
17,35 #c5cded
18,35 #c5cded
46,35 #c5cded
47,35 #c5cded
48,35 #c5cded
49,35 #c5cded
50,35 #c5cded
51,35 #c5cded
52,35 #c5cded
53,35 #c5cded
54,35 #c5cded
55,35 #c5cded
56,35 #c5cded
57,35 #c5cded
58,35 #c5cded
59,35 #c5cded
60,35 #c5cded
61,35 #c5cded
62,35 #c5cded
63,35 #c5cded
0,36 #c5cded
1,36 #c5cded
2,36 #c5cded
3,36 #c5cded
4,36 #c5cded
5,36 #c5cded
6,36 #c5cded
7,36 #c5cded
8,36 #c5cded
9,36 #c5cded
10,36 #c5cded
11,36 #c5cded
12,36 #c5cded
13,36 #c5cded
14,36 #c5cded
15,36 #c5cded
16,36 #c5cded
17,36 #c5cded
18,36 #c5cded
46,36 #c5cded
47,36 #c5cded
48,36 #c5cded
49,36 #c5cded
50,36 #c5cded
51,36 #c5cded
52,36 #c5cded
53,36 #c5cded
54,36 #c5cded
55,36 #c5cded
56,36 #c5cded
57,36 #c5cded
58,36 #c5cded
59,36 #c5cded
60,36 #c5cded
61,36 #c5cded
62,36 #c5cded
63,36 #c5cded
0,37 #c5cded
1,37 #c5cded
2,37 #c5cded
3,37 #c5cded
4,37 #c5cded
5,37 #c5cded
6,37 #c5cded
7,37 #c5cded
8,37 #c5cded
9,37 #c5cded
10,37 #c5cded
11,37 #c5cded
12,37 #c5cded
13,37 #c5cded
14,37 #c5cded
15,37 #c5cded
16,37 #c5cded
17,37 #c5cded
18,37 #c5cded
46,37 #c5cded
47,37 #c5cded
48,37 #c5cded
49,37 #c5cded
50,37 #c5cded
51,37 #c5cded
52,37 #c5cded
53,37 #c5cded
54,37 #c5cded
55,37 #c5cded
56,37 #c5cded
57,37 #c5cded
58,37 #c5cded
59,37 #c5cded
60,37 #c5cded
61,37 #c5cded
62,37 #c5cded
63,37 #c5cded
0,38 #c5cded
1,38 #c5cded
2,38 #c5cded
3,38 #c5cded
4,38 #c5cded
5,38 #c5cded
6,38 #c5cded
7,38 #c5cded
8,38 #c5cded
9,38 #c5cded
10,38 #c5cded
11,38 #c5cded
12,38 #c5cded
13,38 #c5cded
14,38 #c5cded
15,38 #c5cded
16,38 #c5cded
17,38 #c5cded
18,38 #c5cded
19,38 #c5cded
45,38 #c5cded
46,38 #c5cded
47,38 #c5cded
48,38 #c5cded
49,38 #c5cded
50,38 #c5cded
51,38 #c5cded
52,38 #c5cded
53,38 #c5cded
54,38 #c5cded
55,38 #c5cded
56,38 #c5cded
57,38 #c5cded
58,38 #c5cded
59,38 #c5cded
60,38 #c5cded
61,38 #c5cded
62,38 #c5cded
63,38 #c5cded
0,39 #c5cded
1,39 #c5cded
2,39 #c5cded
3,39 #c5cded
4,39 #c5cded
5,39 #c5cded
6,39 #c5cded
7,39 #c5cded
8,39 #c5cded
9,39 #c5cded
10,39 #c5cded
11,39 #c5cded
12,39 #c5cded
13,39 #c5cded
14,39 #c5cded
15,39 #c5cded
16,39 #c5cded
17,39 #c5cded
18,39 #c5cded
19,39 #c5cded
25,39 #c5cded
26,39 #c5cded
27,39 #c5cded
28,39 #c5cded
29,39 #c5cded
30,39 #c5cded
31,39 #c5cded
32,39 #c5cded
33,39 #c5cded
34,39 #c5cded
35,39 #c5cded
36,39 #c5cded
37,39 #c5cded
38,39 #c5cded
39,39 #c5cded
45,39 #c5cded
46,39 #c5cded
47,39 #c5cded
48,39 #c5cded
49,39 #c5cded
50,39 #c5cded
51,39 #c5cded
52,39 #c5cded
53,39 #c5cded
54,39 #c5cded
55,39 #c5cded
56,39 #c5cded
57,39 #c5cded
58,39 #c5cded
59,39 #c5cded
60,39 #c5cded
61,39 #c5cded
62,39 #c5cded
63,39 #c5cded
0,40 #c5cded
1,40 #c5cded
2,40 #c5cded
3,40 #c5cded
4,40 #c5cded
5,40 #c5cded
6,40 #c5cded
7,40 #c5cded
8,40 #c5cded
9,40 #c5cded
10,40 #c5cded
11,40 #c5cded
12,40 #c5cded
13,40 #c5cded
14,40 #c5cded
15,40 #c5cded
16,40 #c5cded
17,40 #c5cded
18,40 #c5cded
19,40 #c5cded
25,40 #c5cded
26,40 #c5cded
27,40 #c5cded
28,40 #c5cded
29,40 #c5cded
30,40 #c5cded
31,40 #c5cded
32,40 #c5cded
33,40 #c5cded
34,40 #c5cded
35,40 #c5cded
36,40 #c5cded
37,40 #c5cded
38,40 #c5cded
39,40 #c5cded
45,40 #c5cded
46,40 #c5cded
47,40 #c5cded
48,40 #c5cded
49,40 #c5cded
50,40 #c5cded
51,40 #c5cded
52,40 #c5cded
53,40 #c5cded
54,40 #c5cded
55,40 #c5cded
56,40 #c5cded
57,40 #c5cded
58,40 #c5cded
59,40 #c5cded
60,40 #c5cded
61,40 #c5cded
62,40 #c5cded
63,40 #c5cded
0,41 #c5cded
1,41 #c5cded
2,41 #c5cded
3,41 #c5cded
4,41 #c5cded
5,41 #c5cded
6,41 #c5cded
7,41 #c5cded
8,41 #c5cded
9,41 #c5cded
10,41 #c5cded
11,41 #c5cded
12,41 #c5cded
13,41 #c5cded
14,41 #c5cded
15,41 #c5cded
16,41 #c5cded
17,41 #c5cded
18,41 #c5cded
19,41 #c5cded
25,41 #c5cded
26,41 #c5cded
27,41 #c5cded
28,41 #c5cded
29,41 #c5cded
30,41 #c5cded
31,41 #c5cded
32,41 #c5cded
33,41 #c5cded
34,41 #c5cded
35,41 #c5cded
36,41 #c5cded
37,41 #c5cded
38,41 #c5cded
39,41 #c5cded
44,41 #c5cded
45,41 #c5cded
46,41 #c5cded
47,41 #c5cded
48,41 #c5cded
49,41 #c5cded
50,41 #c5cded
51,41 #c5cded
52,41 #c5cded
53,41 #c5cded
54,41 #c5cded
55,41 #c5cded
56,41 #c5cded
57,41 #c5cded
58,41 #c5cded
59,41 #c5cded
60,41 #c5cded
61,41 #c5cded
62,41 #c5cded
63,41 #c5cded
0,42 #c5cded
1,42 #c5cded
2,42 #c5cded
3,42 #c5cded
4,42 #c5cded
5,42 #c5cded
6,42 #c5cded
7,42 #c5cded
8,42 #c5cded
9,42 #c5cded
10,42 #c5cded
11,42 #c5cded
12,42 #c5cded
13,42 #c5cded
14,42 #c5cded
15,42 #c5cded
16,42 #c5cded
17,42 #c5cded
18,42 #c5cded
19,42 #c5cded
25,42 #c5cded
26,42 #c5cded
27,42 #c5cded
28,42 #c5cded
29,42 #c5cded
30,42 #c5cded
31,42 #c5cded
32,42 #c5cded
33,42 #c5cded
34,42 #c5cded
35,42 #c5cded
36,42 #c5cded
37,42 #c5cded
38,42 #c5cded
39,42 #c5cded
44,42 #c5cded
45,42 #c5cded
46,42 #c5cded
47,42 #c5cded
48,42 #c5cded
49,42 #c5cded
50,42 #c5cded
51,42 #c5cded
52,42 #c5cded
53,42 #c5cded
54,42 #c5cded
55,42 #c5cded
56,42 #c5cded
57,42 #c5cded
58,42 #c5cded
59,42 #c5cded
60,42 #c5cded
61,42 #c5cded
62,42 #c5cded
63,42 #c5cded
0,43 #c5cded
1,43 #c5cded
2,43 #c5cded
3,43 #c5cded
4,43 #c5cded
5,43 #c5cded
6,43 #c5cded
7,43 #c5cded
8,43 #c5cded
9,43 #c5cded
10,43 #c5cded
11,43 #c5cded
12,43 #c5cded
13,43 #c5cded
14,43 #c5cded
15,43 #c5cded
16,43 #c5cded
17,43 #c5cded
18,43 #c5cded
19,43 #c5cded
25,43 #c5cded
26,43 #c5cded
27,43 #c5cded
28,43 #c5cded
29,43 #c5cded
30,43 #c5cded
31,43 #c5cded
32,43 #c5cded
33,43 #c5cded
34,43 #c5cded
35,43 #c5cded
36,43 #c5cded
37,43 #c5cded
38,43 #c5cded
39,43 #c5cded
45,43 #c5cded
46,43 #c5cded
47,43 #c5cded
48,43 #c5cded
49,43 #c5cded
50,43 #c5cded
51,43 #c5cded
52,43 #c5cded
53,43 #c5cded
54,43 #c5cded
55,43 #c5cded
56,43 #c5cded
57,43 #c5cded
58,43 #c5cded
59,43 #c5cded
60,43 #c5cded
61,43 #c5cded
62,43 #c5cded
63,43 #c5cded
0,44 #c5cded
1,44 #c5cded
2,44 #c5cded
3,44 #c5cded
4,44 #c5cded
5,44 #c5cded
6,44 #c5cded
7,44 #c5cded
8,44 #c5cded
9,44 #c5cded
10,44 #c5cded
11,44 #c5cded
12,44 #c5cded
13,44 #c5cded
14,44 #c5cded
15,44 #c5cded
16,44 #c5cded
17,44 #c5cded
18,44 #c5cded
19,44 #c5cded
25,44 #c5cded
26,44 #c5cded
27,44 #c5cded
28,44 #c5cded
29,44 #c5cded
30,44 #c5cded
31,44 #c5cded
32,44 #c5cded
33,44 #c5cded
34,44 #c5cded
35,44 #c5cded
36,44 #c5cded
37,44 #c5cded
38,44 #c5cded
39,44 #c5cded
45,44 #c5cded
46,44 #c5cded
47,44 #c5cded
48,44 #c5cded
49,44 #c5cded
50,44 #c5cded
51,44 #c5cded
52,44 #c5cded
53,44 #c5cded
54,44 #c5cded
55,44 #c5cded
56,44 #c5cded
57,44 #c5cded
58,44 #c5cded
59,44 #c5cded
60,44 #c5cded
61,44 #c5cded
62,44 #c5cded
63,44 #c5cded
0,45 #c5cded
1,45 #c5cded
2,45 #c5cded
3,45 #c5cded
4,45 #c5cded
5,45 #c5cded
6,45 #c5cded
7,45 #c5cded
8,45 #c5cded
9,45 #c5cded
10,45 #c5cded
11,45 #c5cded
12,45 #c5cded
13,45 #c5cded
14,45 #c5cded
15,45 #c5cded
16,45 #c5cded
17,45 #c5cded
18,45 #c5cded
19,45 #c5cded
26,45 #c5cded
27,45 #c5cded
28,45 #c5cded
29,45 #c5cded
30,45 #c5cded
31,45 #c5cded
32,45 #c5cded
33,45 #c5cded
34,45 #c5cded
35,45 #c5cded
36,45 #c5cded
37,45 #c5cded
38,45 #c5cded
39,45 #c5cded
45,45 #c5cded
46,45 #c5cded
47,45 #c5cded
48,45 #c5cded
49,45 #c5cded
50,45 #c5cded
51,45 #c5cded
52,45 #c5cded
53,45 #c5cded
54,45 #c5cded
55,45 #c5cded
56,45 #c5cded
57,45 #c5cded
58,45 #c5cded
59,45 #c5cded
60,45 #c5cded
61,45 #c5cded
62,45 #c5cded
63,45 #c5cded
0,46 #c5cded
1,46 #c5cded
2,46 #c5cded
3,46 #c5cded
4,46 #c5cded
5,46 #c5cded
6,46 #c5cded
7,46 #c5cded
8,46 #c5cded
9,46 #c5cded
10,46 #c5cded
11,46 #c5cded
12,46 #c5cded
13,46 #c5cded
14,46 #c5cded
15,46 #c5cded
16,46 #c5cded
17,46 #c5cded
18,46 #c5cded
19,46 #c5cded
26,46 #c5cded
27,46 #c5cded
28,46 #c5cded
29,46 #c5cded
30,46 #c5cded
31,46 #c5cded
32,46 #c5cded
33,46 #c5cded
34,46 #c5cded
35,46 #c5cded
36,46 #c5cded
37,46 #c5cded
38,46 #c5cded
39,46 #c5cded
46,46 #c5cded
47,46 #c5cded
48,46 #c5cded
49,46 #c5cded
50,46 #c5cded
51,46 #c5cded
52,46 #c5cded
53,46 #c5cded
54,46 #c5cded
55,46 #c5cded
56,46 #c5cded
57,46 #c5cded
58,46 #c5cded
59,46 #c5cded
60,46 #c5cded
61,46 #c5cded
62,46 #c5cded
63,46 #c5cded
0,47 #c5cded
1,47 #c5cded
2,47 #c5cded
3,47 #c5cded
4,47 #c5cded
5,47 #c5cded
6,47 #c5cded
7,47 #c5cded
8,47 #c5cded
9,47 #c5cded
10,47 #c5cded
11,47 #c5cded
12,47 #c5cded
13,47 #c5cded
14,47 #c5cded
15,47 #c5cded
16,47 #c5cded
17,47 #c5cded
18,47 #c5cded
19,47 #c5cded
26,47 #c5cded
27,47 #c5cded
28,47 #c5cded
29,47 #c5cded
30,47 #c5cded
31,47 #c5cded
32,47 #c5cded
33,47 #c5cded
34,47 #c5cded
35,47 #c5cded
36,47 #c5cded
37,47 #c5cded
38,47 #c5cded
39,47 #c5cded
46,47 #c5cded
47,47 #c5cded
48,47 #c5cded
49,47 #c5cded
50,47 #c5cded
51,47 #c5cded
52,47 #c5cded
53,47 #c5cded
54,47 #c5cded
55,47 #c5cded
56,47 #c5cded
57,47 #c5cded
58,47 #c5cded
59,47 #c5cded
60,47 #c5cded
61,47 #c5cded
62,47 #c5cded
63,47 #c5cded
0,48 #c5cded
1,48 #c5cded
2,48 #c5cded
3,48 #c5cded
4,48 #c5cded
5,48 #c5cded
6,48 #c5cded
7,48 #c5cded
8,48 #c5cded
9,48 #c5cded
10,48 #c5cded
11,48 #c5cded
12,48 #c5cded
13,48 #c5cded
14,48 #c5cded
15,48 #c5cded
16,48 #c5cded
17,48 #c5cded
18,48 #c5cded
26,48 #c5cded
27,48 #c5cded
28,48 #c5cded
29,48 #c5cded
30,48 #c5cded
31,48 #c5cded
32,48 #c5cded
33,48 #c5cded
34,48 #c5cded
35,48 #c5cded
36,48 #c5cded
37,48 #c5cded
38,48 #c5cded
46,48 #c5cded
47,48 #c5cded
48,48 #c5cded
49,48 #c5cded
50,48 #c5cded
51,48 #c5cded
52,48 #c5cded
53,48 #c5cded
54,48 #c5cded
55,48 #c5cded
56,48 #c5cded
57,48 #c5cded
58,48 #c5cded
59,48 #c5cded
60,48 #c5cded
61,48 #c5cded
62,48 #c5cded
63,48 #c5cded
0,49 #c5cded
1,49 #c5cded
2,49 #c5cded
3,49 #c5cded
4,49 #c5cded
5,49 #c5cded
6,49 #c5cded
7,49 #c5cded
8,49 #c5cded
9,49 #c5cded
10,49 #c5cded
11,49 #c5cded
12,49 #c5cded
13,49 #c5cded
14,49 #c5cded
15,49 #c5cded
16,49 #c5cded
17,49 #c5cded
18,49 #c5cded
27,49 #c5cded
28,49 #c5cded
29,49 #c5cded
30,49 #c5cded
31,49 #c5cded
32,49 #c5cded
33,49 #c5cded
34,49 #c5cded
35,49 #c5cded
36,49 #c5cded
37,49 #c5cded
38,49 #c5cded
47,49 #c5cded
48,49 #c5cded
49,49 #c5cded
50,49 #c5cded
51,49 #c5cded
52,49 #c5cded
53,49 #c5cded
54,49 #c5cded
55,49 #c5cded
56,49 #c5cded
57,49 #c5cded
58,49 #c5cded
59,49 #c5cded
60,49 #c5cded
61,49 #c5cded
62,49 #c5cded
63,49 #c5cded
0,50 #c5cded
1,50 #c5cded
2,50 #c5cded
3,50 #c5cded
4,50 #c5cded
5,50 #c5cded
6,50 #c5cded
7,50 #c5cded
8,50 #c5cded
9,50 #c5cded
10,50 #c5cded
11,50 #c5cded
12,50 #c5cded
13,50 #c5cded
14,50 #c5cded
15,50 #c5cded
16,50 #c5cded
17,50 #c5cded
18,50 #c5cded
28,50 #c5cded
29,50 #c5cded
30,50 #c5cded
31,50 #c5cded
32,50 #c5cded
33,50 #c5cded
34,50 #c5cded
35,50 #c5cded
36,50 #c5cded
37,50 #c5cded
38,50 #c5cded
48,50 #c5cded
49,50 #c5cded
50,50 #c5cded
51,50 #c5cded
52,50 #c5cded
53,50 #c5cded
54,50 #c5cded
55,50 #c5cded
56,50 #c5cded
57,50 #c5cded
58,50 #c5cded
59,50 #c5cded
60,50 #c5cded
61,50 #c5cded
62,50 #c5cded
63,50 #c5cded
0,51 #c5cded
1,51 #c5cded
2,51 #c5cded
3,51 #c5cded
4,51 #c5cded
5,51 #c5cded
6,51 #c5cded
7,51 #c5cded
8,51 #c5cded
9,51 #c5cded
10,51 #c5cded
11,51 #c5cded
12,51 #c5cded
13,51 #c5cded
14,51 #c5cded
15,51 #c5cded
16,51 #c5cded
17,51 #c5cded
18,51 #c5cded
19,51 #c5cded
23,51 #c5cded
27,51 #c5cded
28,51 #c5cded
29,51 #c5cded
30,51 #c5cded
31,51 #c5cded
32,51 #c5cded
33,51 #c5cded
34,51 #c5cded
35,51 #c5cded
36,51 #c5cded
37,51 #c5cded
38,51 #c5cded
39,51 #c5cded
43,51 #c5cded
47,51 #c5cded
48,51 #c5cded
49,51 #c5cded
50,51 #c5cded
51,51 #c5cded
52,51 #c5cded
53,51 #c5cded
54,51 #c5cded
55,51 #c5cded
56,51 #c5cded
57,51 #c5cded
58,51 #c5cded
59,51 #c5cded
60,51 #c5cded
61,51 #c5cded
62,51 #c5cded
63,51 #c5cded
0,52 #c5cded
1,52 #c5cded
2,52 #c5cded
3,52 #c5cded
4,52 #c5cded
5,52 #c5cded
6,52 #c5cded
7,52 #c5cded
8,52 #c5cded
9,52 #c5cded
10,52 #c5cded
11,52 #c5cded
12,52 #c5cded
13,52 #c5cded
14,52 #c5cded
15,52 #c5cded
16,52 #c5cded
17,52 #c5cded
18,52 #c5cded
19,52 #c5cded
20,52 #c5cded
21,52 #c5cded
22,52 #c5cded
23,52 #c5cded
24,52 #c5cded
25,52 #c5cded
26,52 #c5cded
27,52 #c5cded
28,52 #c5cded
29,52 #c5cded
30,52 #c5cded
31,52 #c5cded
32,52 #c5cded
33,52 #c5cded
34,52 #c5cded
35,52 #c5cded
36,52 #c5cded
37,52 #c5cded
38,52 #c5cded
39,52 #c5cded
40,52 #c5cded
41,52 #c5cded
42,52 #c5cded
43,52 #c5cded
44,52 #c5cded
45,52 #c5cded
46,52 #c5cded
47,52 #c5cded
48,52 #c5cded
49,52 #c5cded
50,52 #c5cded
51,52 #c5cded
52,52 #c5cded
53,52 #c5cded
54,52 #c5cded
55,52 #c5cded
56,52 #c5cded
57,52 #c5cded
58,52 #c5cded
59,52 #c5cded
60,52 #c5cded
61,52 #c5cded
62,52 #c5cded
63,52 #c5cded
0,53 #c5cded
1,53 #c5cded
2,53 #c5cded
3,53 #c5cded
4,53 #c5cded
5,53 #c5cded
6,53 #c5cded
7,53 #c5cded
8,53 #c5cded
9,53 #c5cded
10,53 #c5cded
11,53 #c5cded
12,53 #c5cded
13,53 #c5cded
14,53 #c5cded
15,53 #c5cded
16,53 #c5cded
17,53 #c5cded
18,53 #c5cded
19,53 #c5cded
20,53 #c5cded
21,53 #c5cded
22,53 #c5cded
23,53 #c5cded
24,53 #c5cded
25,53 #c5cded
26,53 #c5cded
27,53 #c5cded
28,53 #c5cded
29,53 #c5cded
30,53 #c5cded
31,53 #c5cded
32,53 #c5cded
33,53 #c5cded
34,53 #c5cded
35,53 #c5cded
36,53 #c5cded
37,53 #c5cded
38,53 #c5cded
39,53 #c5cded
40,53 #c5cded
41,53 #c5cded
42,53 #c5cded
43,53 #c5cded
44,53 #c5cded
45,53 #c5cded
46,53 #c5cded
47,53 #c5cded
48,53 #c5cded
49,53 #c5cded
50,53 #c5cded
51,53 #c5cded
52,53 #c5cded
53,53 #c5cded
54,53 #c5cded
55,53 #c5cded
56,53 #c5cded
57,53 #c5cded
58,53 #c5cded
59,53 #c5cded
60,53 #c5cded
61,53 #c5cded
62,53 #c5cded
63,53 #c5cded
0,54 #c5cded
1,54 #c5cded
2,54 #c5cded
3,54 #c5cded
4,54 #c5cded
5,54 #c5cded
6,54 #c5cded
7,54 #c5cded
8,54 #c5cded
9,54 #c5cded
10,54 #c5cded
11,54 #c5cded
12,54 #c5cded
13,54 #c5cded
14,54 #c5cded
15,54 #c5cded
16,54 #c5cded
17,54 #c5cded
18,54 #c5cded
19,54 #c5cded
20,54 #c5cded
21,54 #c5cded
22,54 #c5cded
23,54 #c5cded
24,54 #c5cded
25,54 #c5cded
26,54 #c5cded
27,54 #c5cded
28,54 #c5cded
29,54 #c5cded
30,54 #c5cded
31,54 #c5cded
32,54 #c5cded
33,54 #c5cded
34,54 #c5cded
35,54 #c5cded
36,54 #c5cded
37,54 #c5cded
38,54 #c5cded
39,54 #c5cded
40,54 #c5cded
41,54 #c5cded
42,54 #c5cded
43,54 #c5cded
44,54 #c5cded
45,54 #c5cded
46,54 #c5cded
47,54 #c5cded
48,54 #c5cded
49,54 #c5cded
50,54 #c5cded
51,54 #c5cded
52,54 #c5cded
53,54 #c5cded
54,54 #c5cded
55,54 #c5cded
56,54 #c5cded
57,54 #c5cded
58,54 #c5cded
59,54 #c5cded
60,54 #c5cded
61,54 #c5cded
62,54 #c5cded
63,54 #c5cded
0,55 #c5cded
1,55 #c5cded
2,55 #c5cded
3,55 #c5cded
4,55 #c5cded
5,55 #c5cded
6,55 #c5cded
7,55 #c5cded
8,55 #c5cded
9,55 #c5cded
10,55 #c5cded
11,55 #c5cded
12,55 #c5cded
13,55 #c5cded
14,55 #c5cded
15,55 #c5cded
16,55 #c5cded
17,55 #c5cded
18,55 #c5cded
19,55 #c5cded
20,55 #c5cded
21,55 #c5cded
22,55 #c5cded
23,55 #c5cded
24,55 #c5cded
25,55 #c5cded
26,55 #c5cded
27,55 #c5cded
28,55 #c5cded
29,55 #c5cded
30,55 #c5cded
31,55 #c5cded
32,55 #c5cded
33,55 #c5cded
34,55 #c5cded
35,55 #c5cded
36,55 #c5cded
37,55 #c5cded
38,55 #c5cded
39,55 #c5cded
40,55 #c5cded
41,55 #c5cded
42,55 #c5cded
43,55 #c5cded
44,55 #c5cded
45,55 #c5cded
46,55 #c5cded
47,55 #c5cded
48,55 #c5cded
49,55 #c5cded
50,55 #c5cded
51,55 #c5cded
52,55 #c5cded
53,55 #c5cded
54,55 #c5cded
55,55 #c5cded
56,55 #c5cded
57,55 #c5cded
58,55 #c5cded
59,55 #c5cded
60,55 #c5cded
61,55 #c5cded
62,55 #c5cded
63,55 #c5cded
0,56 #c5cded
1,56 #c5cded
2,56 #c5cded
3,56 #c5cded
4,56 #c5cded
5,56 #c5cded
6,56 #c5cded
7,56 #c5cded
8,56 #c5cded
9,56 #c5cded
10,56 #c5cded
11,56 #c5cded
12,56 #c5cded
13,56 #c5cded
14,56 #c5cded
15,56 #c5cded
16,56 #c5cded
17,56 #c5cded
18,56 #c5cded
19,56 #c5cded
20,56 #c5cded
21,56 #c5cded
22,56 #c5cded
23,56 #c5cded
24,56 #c5cded
25,56 #c5cded
26,56 #c5cded
27,56 #c5cded
28,56 #c5cded
29,56 #c5cded
30,56 #c5cded
31,56 #c5cded
32,56 #c5cded
33,56 #c5cded
34,56 #c5cded
35,56 #c5cded
36,56 #c5cded
37,56 #c5cded
38,56 #c5cded
39,56 #c5cded
40,56 #c5cded
41,56 #c5cded
42,56 #c5cded
43,56 #c5cded
44,56 #c5cded
45,56 #c5cded
46,56 #c5cded
47,56 #c5cded
48,56 #c5cded
49,56 #c5cded
50,56 #c5cded
51,56 #c5cded
52,56 #c5cded
53,56 #c5cded
54,56 #c5cded
55,56 #c5cded
56,56 #c5cded
57,56 #c5cded
58,56 #c5cded
59,56 #c5cded
60,56 #c5cded
61,56 #c5cded
62,56 #c5cded
63,56 #c5cded
0,57 #c5cded
1,57 #c5cded
2,57 #c5cded
3,57 #c5cded
4,57 #c5cded
5,57 #c5cded
6,57 #c5cded
7,57 #c5cded
8,57 #c5cded
9,57 #c5cded
10,57 #c5cded
11,57 #c5cded
12,57 #c5cded
13,57 #c5cded
14,57 #c5cded
15,57 #c5cded
16,57 #c5cded
17,57 #c5cded
18,57 #c5cded
19,57 #c5cded
20,57 #c5cded
21,57 #c5cded
22,57 #c5cded
23,57 #c5cded
24,57 #c5cded
25,57 #c5cded
26,57 #c5cded
27,57 #c5cded
28,57 #c5cded
29,57 #c5cded
30,57 #c5cded
31,57 #c5cded
32,57 #c5cded
33,57 #c5cded
34,57 #c5cded
35,57 #c5cded
36,57 #c5cded
37,57 #c5cded
38,57 #c5cded
39,57 #c5cded
40,57 #c5cded
41,57 #c5cded
42,57 #c5cded
43,57 #c5cded
44,57 #c5cded
45,57 #c5cded
46,57 #c5cded
47,57 #c5cded
48,57 #c5cded
49,57 #c5cded
50,57 #c5cded
51,57 #c5cded
52,57 #c5cded
53,57 #c5cded
54,57 #c5cded
55,57 #c5cded
56,57 #c5cded
57,57 #c5cded
58,57 #c5cded
59,57 #c5cded
60,57 #c5cded
61,57 #c5cded
62,57 #c5cded
63,57 #c5cded
0,58 #c5cded
1,58 #c5cded
2,58 #c5cded
3,58 #c5cded
4,58 #c5cded
5,58 #c5cded
6,58 #c5cded
7,58 #c5cded
8,58 #c5cded
9,58 #c5cded
10,58 #c5cded
11,58 #c5cded
12,58 #c5cded
13,58 #c5cded
14,58 #c5cded
15,58 #c5cded
16,58 #c5cded
17,58 #c5cded
18,58 #c5cded
19,58 #c5cded
20,58 #c5cded
21,58 #c5cded
22,58 #c5cded
23,58 #c5cded
24,58 #c5cded
25,58 #c5cded
26,58 #c5cded
27,58 #c5cded
28,58 #c5cded
29,58 #c5cded
30,58 #c5cded
31,58 #c5cded
32,58 #c5cded
33,58 #c5cded
34,58 #c5cded
35,58 #c5cded
36,58 #c5cded
37,58 #c5cded
38,58 #c5cded
39,58 #c5cded
40,58 #c5cded
41,58 #c5cded
42,58 #c5cded
43,58 #c5cded
44,58 #c5cded
45,58 #c5cded
46,58 #c5cded
47,58 #c5cded
48,58 #c5cded
49,58 #c5cded
50,58 #c5cded
51,58 #c5cded
52,58 #c5cded
53,58 #c5cded
54,58 #c5cded
55,58 #c5cded
56,58 #c5cded
57,58 #c5cded
58,58 #c5cded
59,58 #c5cded
60,58 #c5cded
61,58 #c5cded
62,58 #c5cded
63,58 #c5cded
0,59 #c5cded
1,59 #c5cded
2,59 #c5cded
3,59 #c5cded
4,59 #c5cded
5,59 #c5cded
6,59 #c5cded
7,59 #c5cded
8,59 #c5cded
9,59 #c5cded
10,59 #c5cded
11,59 #c5cded
12,59 #c5cded
13,59 #c5cded
14,59 #c5cded
15,59 #c5cded
16,59 #c5cded
17,59 #c5cded
18,59 #c5cded
19,59 #c5cded
20,59 #c5cded
21,59 #c5cded
22,59 #c5cded
23,59 #c5cded
24,59 #c5cded
25,59 #c5cded
26,59 #c5cded
27,59 #c5cded
28,59 #c5cded
29,59 #c5cded
30,59 #c5cded
31,59 #c5cded
32,59 #c5cded
33,59 #c5cded
34,59 #c5cded
35,59 #c5cded
36,59 #c5cded
37,59 #c5cded
38,59 #c5cded
39,59 #c5cded
40,59 #c5cded
41,59 #c5cded
42,59 #c5cded
43,59 #c5cded
44,59 #c5cded
45,59 #c5cded
46,59 #c5cded
47,59 #c5cded
48,59 #c5cded
49,59 #c5cded
50,59 #c5cded
51,59 #c5cded
52,59 #c5cded
53,59 #c5cded
54,59 #c5cded
55,59 #c5cded
56,59 #c5cded
57,59 #c5cded
58,59 #c5cded
59,59 #c5cded
60,59 #c5cded
61,59 #c5cded
62,59 #c5cded
63,59 #c5cded
0,60 #c5cded
1,60 #c5cded
2,60 #c5cded
3,60 #c5cded
4,60 #c5cded
5,60 #c5cded
6,60 #c5cded
7,60 #c5cded
8,60 #c5cded
9,60 #c5cded
10,60 #c5cded
11,60 #c5cded
12,60 #c5cded
13,60 #c5cded
14,60 #c5cded
15,60 #c5cded
16,60 #c5cded
17,60 #c5cded
18,60 #c5cded
19,60 #c5cded
20,60 #c5cded
21,60 #c5cded
22,60 #c5cded
23,60 #c5cded
24,60 #c5cded
25,60 #c5cded
26,60 #c5cded
27,60 #c5cded
28,60 #c5cded
29,60 #c5cded
30,60 #c5cded
31,60 #c5cded
32,60 #c5cded
33,60 #c5cded
34,60 #c5cded
35,60 #c5cded
36,60 #c5cded
37,60 #c5cded
38,60 #c5cded
39,60 #c5cded
40,60 #c5cded
41,60 #c5cded
42,60 #c5cded
43,60 #c5cded
44,60 #c5cded
45,60 #c5cded
46,60 #c5cded
47,60 #c5cded
48,60 #c5cded
49,60 #c5cded
50,60 #c5cded
51,60 #c5cded
52,60 #c5cded
53,60 #c5cded
54,60 #c5cded
55,60 #c5cded
56,60 #c5cded
57,60 #c5cded
58,60 #c5cded
59,60 #c5cded
60,60 #c5cded
61,60 #c5cded
62,60 #c5cded
63,60 #c5cded
0,61 #c5cded
1,61 #c5cded
2,61 #c5cded
3,61 #c5cded
4,61 #c5cded
5,61 #c5cded
6,61 #c5cded
7,61 #c5cded
8,61 #c5cded
9,61 #c5cded
10,61 #c5cded
11,61 #c5cded
12,61 #c5cded
13,61 #c5cded
14,61 #c5cded
15,61 #c5cded
16,61 #c5cded
17,61 #c5cded
18,61 #c5cded
19,61 #c5cded
20,61 #c5cded
21,61 #c5cded
22,61 #c5cded
23,61 #c5cded
24,61 #c5cded
25,61 #c5cded
26,61 #c5cded
27,61 #c5cded
28,61 #c5cded
29,61 #c5cded
30,61 #c5cded
31,61 #c5cded
32,61 #c5cded
33,61 #c5cded
34,61 #c5cded
35,61 #c5cded
36,61 #c5cded
37,61 #c5cded
38,61 #c5cded
39,61 #c5cded
40,61 #c5cded
41,61 #c5cded
42,61 #c5cded
43,61 #c5cded
44,61 #c5cded
45,61 #c5cded
46,61 #c5cded
47,61 #c5cded
48,61 #c5cded
49,61 #c5cded
50,61 #c5cded
51,61 #c5cded
52,61 #c5cded
53,61 #c5cded
54,61 #c5cded
55,61 #c5cded
56,61 #c5cded
57,61 #c5cded
58,61 #c5cded
59,61 #c5cded
60,61 #c5cded
61,61 #c5cded
62,61 #c5cded
63,61 #c5cded
0,62 #c5cded
1,62 #c5cded
2,62 #c5cded
3,62 #c5cded
4,62 #c5cded
5,62 #c5cded
6,62 #c5cded
7,62 #c5cded
8,62 #c5cded
9,62 #c5cded
10,62 #c5cded
11,62 #c5cded
12,62 #c5cded
13,62 #c5cded
14,62 #c5cded
15,62 #c5cded
16,62 #c5cded
17,62 #c5cded
18,62 #c5cded
19,62 #c5cded
20,62 #c5cded
21,62 #c5cded
22,62 #c5cded
23,62 #c5cded
24,62 #c5cded
25,62 #c5cded
26,62 #c5cded
27,62 #c5cded
28,62 #c5cded
29,62 #c5cded
30,62 #c5cded
31,62 #c5cded
32,62 #c5cded
33,62 #c5cded
34,62 #c5cded
35,62 #c5cded
36,62 #c5cded
37,62 #c5cded
38,62 #c5cded
39,62 #c5cded
40,62 #c5cded
41,62 #c5cded
42,62 #c5cded
43,62 #c5cded
44,62 #c5cded
45,62 #c5cded
46,62 #c5cded
47,62 #c5cded
48,62 #c5cded
49,62 #c5cded
50,62 #c5cded
51,62 #c5cded
52,62 #c5cded
53,62 #c5cded
54,62 #c5cded
55,62 #c5cded
56,62 #c5cded
57,62 #c5cded
58,62 #c5cded
59,62 #c5cded
60,62 #c5cded
61,62 #c5cded
62,62 #c5cded
63,62 #c5cded
0,63 #c5cded
1,63 #c5cded
2,63 #c5cded
3,63 #c5cded
4,63 #c5cded
5,63 #c5cded
6,63 #c5cded
7,63 #c5cded
8,63 #c5cded
9,63 #c5cded
10,63 #c5cded
11,63 #c5cded
12,63 #c5cded
13,63 #c5cded
14,63 #c5cded
15,63 #c5cded
16,63 #c5cded
17,63 #c5cded
18,63 #c5cded
19,63 #c5cded
20,63 #c5cded
21,63 #c5cded
22,63 #c5cded
23,63 #c5cded
24,63 #c5cded
25,63 #c5cded
26,63 #c5cded
27,63 #c5cded
28,63 #c5cded
29,63 #c5cded
30,63 #c5cded
31,63 #c5cded
32,63 #c5cded
33,63 #c5cded
34,63 #c5cded
35,63 #c5cded
36,63 #c5cded
37,63 #c5cded
38,63 #c5cded
39,63 #c5cded
40,63 #c5cded
41,63 #c5cded
42,63 #c5cded
43,63 #c5cded
44,63 #c5cded
45,63 #c5cded
46,63 #c5cded
47,63 #c5cded
48,63 #c5cded
49,63 #c5cded
50,63 #c5cded
51,63 #c5cded
52,63 #c5cded
53,63 #c5cded
54,63 #c5cded
55,63 #c5cded
56,63 #c5cded
57,63 #c5cded
58,63 #c5cded
59,63 #c5cded
60,63 #c5cded
61,63 #c5cded
62,63 #c5cded
63,63 #c5cded
#### #c4550c (key b) - 301 px
46,10 #c4550c
47,10 #c4550c
51,10 #c4550c
52,10 #c4550c
47,11 #c4550c
52,11 #c4550c
47,12 #c4550c
48,12 #c4550c
52,12 #c4550c
53,12 #c4550c
47,13 #c4550c
48,13 #c4550c
52,13 #c4550c
53,13 #c4550c
47,14 #c4550c
48,14 #c4550c
52,14 #c4550c
53,14 #c4550c
50,15 #c4550c
51,15 #c4550c
52,15 #c4550c
48,16 #c4550c
49,16 #c4550c
50,16 #c4550c
51,16 #c4550c
52,16 #c4550c
53,16 #c4550c
44,17 #c4550c
45,17 #c4550c
46,17 #c4550c
47,17 #c4550c
48,17 #c4550c
49,17 #c4550c
51,17 #c4550c
52,17 #c4550c
53,17 #c4550c
54,17 #c4550c
44,18 #c4550c
45,18 #c4550c
46,18 #c4550c
47,18 #c4550c
48,18 #c4550c
49,18 #c4550c
50,18 #c4550c
51,18 #c4550c
52,18 #c4550c
53,18 #c4550c
54,18 #c4550c
55,18 #c4550c
56,18 #c4550c
57,18 #c4550c
44,19 #c4550c
45,19 #c4550c
46,19 #c4550c
47,19 #c4550c
48,19 #c4550c
49,19 #c4550c
50,19 #c4550c
51,19 #c4550c
52,19 #c4550c
53,19 #c4550c
54,19 #c4550c
55,19 #c4550c
56,19 #c4550c
57,19 #c4550c
58,19 #c4550c
59,19 #c4550c
44,20 #c4550c
45,20 #c4550c
46,20 #c4550c
47,20 #c4550c
48,20 #c4550c
49,20 #c4550c
50,20 #c4550c
51,20 #c4550c
52,20 #c4550c
53,20 #c4550c
54,20 #c4550c
55,20 #c4550c
56,20 #c4550c
57,20 #c4550c
58,20 #c4550c
59,20 #c4550c
44,21 #c4550c
45,21 #c4550c
46,21 #c4550c
47,21 #c4550c
48,21 #c4550c
43,22 #c4550c
44,22 #c4550c
45,22 #c4550c
42,23 #c4550c
43,23 #c4550c
44,23 #c4550c
45,23 #c4550c
46,23 #c4550c
41,24 #c4550c
42,24 #c4550c
43,24 #c4550c
44,24 #c4550c
45,24 #c4550c
40,25 #c4550c
41,25 #c4550c
42,25 #c4550c
43,25 #c4550c
44,25 #c4550c
39,26 #c4550c
40,26 #c4550c
41,26 #c4550c
42,26 #c4550c
43,26 #c4550c
39,27 #c4550c
40,27 #c4550c
41,27 #c4550c
42,27 #c4550c
8,29 #c4550c
9,29 #c4550c
10,29 #c4550c
11,29 #c4550c
12,29 #c4550c
13,29 #c4550c
14,29 #c4550c
15,29 #c4550c
16,29 #c4550c
18,29 #c4550c
19,29 #c4550c
20,29 #c4550c
21,29 #c4550c
22,29 #c4550c
23,29 #c4550c
24,29 #c4550c
25,29 #c4550c
26,29 #c4550c
27,29 #c4550c
28,29 #c4550c
29,29 #c4550c
30,29 #c4550c
31,29 #c4550c
32,29 #c4550c
33,29 #c4550c
34,29 #c4550c
35,29 #c4550c
36,29 #c4550c
37,29 #c4550c
38,29 #c4550c
39,29 #c4550c
40,29 #c4550c
41,29 #c4550c
42,29 #c4550c
8,30 #c4550c
9,30 #c4550c
10,30 #c4550c
11,30 #c4550c
12,30 #c4550c
13,30 #c4550c
14,30 #c4550c
15,30 #c4550c
16,30 #c4550c
18,30 #c4550c
19,30 #c4550c
20,30 #c4550c
21,30 #c4550c
22,30 #c4550c
23,30 #c4550c
24,30 #c4550c
25,30 #c4550c
26,30 #c4550c
27,30 #c4550c
28,30 #c4550c
29,30 #c4550c
30,30 #c4550c
31,30 #c4550c
32,30 #c4550c
33,30 #c4550c
34,30 #c4550c
35,30 #c4550c
36,30 #c4550c
37,30 #c4550c
38,30 #c4550c
39,30 #c4550c
40,30 #c4550c
41,30 #c4550c
42,30 #c4550c
8,31 #c4550c
9,31 #c4550c
10,31 #c4550c
11,31 #c4550c
12,31 #c4550c
13,31 #c4550c
14,31 #c4550c
15,31 #c4550c
16,31 #c4550c
18,31 #c4550c
19,31 #c4550c
20,31 #c4550c
21,31 #c4550c
22,31 #c4550c
23,31 #c4550c
24,31 #c4550c
25,31 #c4550c
26,31 #c4550c
27,31 #c4550c
28,31 #c4550c
29,31 #c4550c
30,31 #c4550c
31,31 #c4550c
32,31 #c4550c
33,31 #c4550c
34,31 #c4550c
35,31 #c4550c
36,31 #c4550c
37,31 #c4550c
38,31 #c4550c
39,31 #c4550c
40,31 #c4550c
41,31 #c4550c
42,31 #c4550c
19,32 #c4550c
20,32 #c4550c
22,32 #c4550c
23,32 #c4550c
24,32 #c4550c
25,32 #c4550c
26,32 #c4550c
27,32 #c4550c
28,32 #c4550c
29,32 #c4550c
30,32 #c4550c
31,32 #c4550c
32,32 #c4550c
33,32 #c4550c
34,32 #c4550c
35,32 #c4550c
36,32 #c4550c
37,32 #c4550c
38,32 #c4550c
39,32 #c4550c
40,32 #c4550c
41,32 #c4550c
43,32 #c4550c
44,32 #c4550c
19,33 #c4550c
20,33 #c4550c
22,33 #c4550c
23,33 #c4550c
24,33 #c4550c
25,33 #c4550c
26,33 #c4550c
27,33 #c4550c
28,33 #c4550c
29,33 #c4550c
30,33 #c4550c
31,33 #c4550c
32,33 #c4550c
33,33 #c4550c
34,33 #c4550c
35,33 #c4550c
36,33 #c4550c
37,33 #c4550c
38,33 #c4550c
39,33 #c4550c
40,33 #c4550c
41,33 #c4550c
43,33 #c4550c
44,33 #c4550c
20,34 #c4550c
21,34 #c4550c
43,34 #c4550c
44,34 #c4550c
20,35 #c4550c
21,35 #c4550c
43,35 #c4550c
44,35 #c4550c
20,36 #c4550c
21,36 #c4550c
42,36 #c4550c
43,36 #c4550c
20,37 #c4550c
21,37 #c4550c
42,37 #c4550c
43,37 #c4550c
21,38 #c4550c
22,38 #c4550c
42,38 #c4550c
43,38 #c4550c
21,39 #c4550c
22,39 #c4550c
42,39 #c4550c
43,39 #c4550c
21,40 #c4550c
22,40 #c4550c
42,40 #c4550c
43,40 #c4550c
21,41 #c4550c
22,41 #c4550c
41,41 #c4550c
42,41 #c4550c
22,42 #c4550c
23,42 #c4550c
41,42 #c4550c
42,42 #c4550c
#### #3a2518 (key c) - 262 px
46,7 #3a2518
51,7 #3a2518
45,8 #3a2518
46,8 #3a2518
47,8 #3a2518
50,8 #3a2518
51,8 #3a2518
52,8 #3a2518
45,9 #3a2518
47,9 #3a2518
50,9 #3a2518
52,9 #3a2518
44,10 #3a2518
48,10 #3a2518
49,10 #3a2518
53,10 #3a2518
44,11 #3a2518
48,11 #3a2518
49,11 #3a2518
53,11 #3a2518
44,12 #3a2518
49,12 #3a2518
54,12 #3a2518
44,13 #3a2518
49,13 #3a2518
54,13 #3a2518
44,14 #3a2518
49,14 #3a2518
54,14 #3a2518
44,15 #3a2518
53,15 #3a2518
43,16 #3a2518
54,16 #3a2518
43,17 #3a2518
55,17 #3a2518
43,18 #3a2518
58,18 #3a2518
43,19 #3a2518
60,19 #3a2518
43,20 #3a2518
61,20 #3a2518
43,21 #3a2518
60,21 #3a2518
42,22 #3a2518
58,22 #3a2518
41,23 #3a2518
50,23 #3a2518
51,23 #3a2518
52,23 #3a2518
53,23 #3a2518
54,23 #3a2518
55,23 #3a2518
56,23 #3a2518
57,23 #3a2518
58,23 #3a2518
40,24 #3a2518
50,24 #3a2518
24,25 #3a2518
25,25 #3a2518
26,25 #3a2518
27,25 #3a2518
28,25 #3a2518
29,25 #3a2518
30,25 #3a2518
31,25 #3a2518
32,25 #3a2518
33,25 #3a2518
34,25 #3a2518
35,25 #3a2518
36,25 #3a2518
39,25 #3a2518
50,25 #3a2518
8,26 #3a2518
9,26 #3a2518
10,26 #3a2518
11,26 #3a2518
12,26 #3a2518
13,26 #3a2518
14,26 #3a2518
15,26 #3a2518
16,26 #3a2518
18,26 #3a2518
19,26 #3a2518
20,26 #3a2518
21,26 #3a2518
22,26 #3a2518
23,26 #3a2518
37,26 #3a2518
38,26 #3a2518
49,26 #3a2518
50,26 #3a2518
4,27 #3a2518
5,27 #3a2518
6,27 #3a2518
7,27 #3a2518
17,27 #3a2518
18,27 #3a2518
19,27 #3a2518
20,27 #3a2518
48,27 #3a2518
49,27 #3a2518
3,28 #3a2518
18,28 #3a2518
47,28 #3a2518
48,28 #3a2518
2,29 #3a2518
17,29 #3a2518
46,29 #3a2518
47,29 #3a2518
2,30 #3a2518
17,30 #3a2518
45,30 #3a2518
2,31 #3a2518
17,31 #3a2518
45,31 #3a2518
3,32 #3a2518
17,32 #3a2518
18,32 #3a2518
21,32 #3a2518
42,32 #3a2518
45,32 #3a2518
5,33 #3a2518
16,33 #3a2518
17,33 #3a2518
18,33 #3a2518
21,33 #3a2518
42,33 #3a2518
45,33 #3a2518
6,34 #3a2518
7,34 #3a2518
8,34 #3a2518
9,34 #3a2518
10,34 #3a2518
11,34 #3a2518
12,34 #3a2518
13,34 #3a2518
14,34 #3a2518
15,34 #3a2518
17,34 #3a2518
19,34 #3a2518
22,34 #3a2518
42,34 #3a2518
45,34 #3a2518
19,35 #3a2518
22,35 #3a2518
42,35 #3a2518
45,35 #3a2518
19,36 #3a2518
22,36 #3a2518
41,36 #3a2518
44,36 #3a2518
45,36 #3a2518
19,37 #3a2518
22,37 #3a2518
41,37 #3a2518
44,37 #3a2518
45,37 #3a2518
20,38 #3a2518
23,38 #3a2518
24,38 #3a2518
25,38 #3a2518
26,38 #3a2518
27,38 #3a2518
28,38 #3a2518
29,38 #3a2518
30,38 #3a2518
31,38 #3a2518
32,38 #3a2518
33,38 #3a2518
34,38 #3a2518
35,38 #3a2518
36,38 #3a2518
37,38 #3a2518
38,38 #3a2518
39,38 #3a2518
40,38 #3a2518
41,38 #3a2518
44,38 #3a2518
20,39 #3a2518
23,39 #3a2518
24,39 #3a2518
40,39 #3a2518
41,39 #3a2518
44,39 #3a2518
20,40 #3a2518
23,40 #3a2518
24,40 #3a2518
40,40 #3a2518
41,40 #3a2518
44,40 #3a2518
20,41 #3a2518
23,41 #3a2518
24,41 #3a2518
40,41 #3a2518
43,41 #3a2518
20,42 #3a2518
21,42 #3a2518
24,42 #3a2518
40,42 #3a2518
43,42 #3a2518
20,43 #3a2518
21,43 #3a2518
24,43 #3a2518
40,43 #3a2518
43,43 #3a2518
44,43 #3a2518
20,44 #3a2518
21,44 #3a2518
24,44 #3a2518
40,44 #3a2518
43,44 #3a2518
44,44 #3a2518
20,45 #3a2518
22,45 #3a2518
25,45 #3a2518
40,45 #3a2518
43,45 #3a2518
44,45 #3a2518
20,46 #3a2518
22,46 #3a2518
25,46 #3a2518
40,46 #3a2518
43,46 #3a2518
45,46 #3a2518
20,47 #3a2518
22,47 #3a2518
25,47 #3a2518
40,47 #3a2518
43,47 #3a2518
45,47 #3a2518
19,48 #3a2518
22,48 #3a2518
25,48 #3a2518
39,48 #3a2518
42,48 #3a2518
45,48 #3a2518
19,49 #3a2518
22,49 #3a2518
23,49 #3a2518
26,49 #3a2518
39,49 #3a2518
42,49 #3a2518
43,49 #3a2518
46,49 #3a2518
19,50 #3a2518
23,50 #3a2518
27,50 #3a2518
39,50 #3a2518
43,50 #3a2518
47,50 #3a2518
20,51 #3a2518
21,51 #3a2518
22,51 #3a2518
24,51 #3a2518
25,51 #3a2518
26,51 #3a2518
40,51 #3a2518
41,51 #3a2518
42,51 #3a2518
44,51 #3a2518
45,51 #3a2518
46,51 #3a2518
#### #a64c10 (key d) - 91 px
8,32 #a64c10
9,32 #a64c10
10,32 #a64c10
11,32 #a64c10
12,32 #a64c10
13,32 #a64c10
14,32 #a64c10
15,32 #a64c10
16,32 #a64c10
8,33 #a64c10
9,33 #a64c10
10,33 #a64c10
11,33 #a64c10
12,33 #a64c10
13,33 #a64c10
14,33 #a64c10
15,33 #a64c10
23,34 #a64c10
24,34 #a64c10
25,34 #a64c10
26,34 #a64c10
27,34 #a64c10
28,34 #a64c10
29,34 #a64c10
30,34 #a64c10
31,34 #a64c10
32,34 #a64c10
33,34 #a64c10
34,34 #a64c10
35,34 #a64c10
36,34 #a64c10
37,34 #a64c10
38,34 #a64c10
39,34 #a64c10
40,34 #a64c10
41,34 #a64c10
23,35 #a64c10
24,35 #a64c10
25,35 #a64c10
26,35 #a64c10
27,35 #a64c10
28,35 #a64c10
29,35 #a64c10
30,35 #a64c10
31,35 #a64c10
32,35 #a64c10
33,35 #a64c10
34,35 #a64c10
35,35 #a64c10
36,35 #a64c10
37,35 #a64c10
38,35 #a64c10
39,35 #a64c10
40,35 #a64c10
41,35 #a64c10
23,36 #a64c10
24,36 #a64c10
25,36 #a64c10
26,36 #a64c10
27,36 #a64c10
28,36 #a64c10
29,36 #a64c10
30,36 #a64c10
31,36 #a64c10
32,36 #a64c10
33,36 #a64c10
34,36 #a64c10
35,36 #a64c10
36,36 #a64c10
37,36 #a64c10
38,36 #a64c10
39,36 #a64c10
40,36 #a64c10
23,37 #a64c10
24,37 #a64c10
25,37 #a64c10
26,37 #a64c10
27,37 #a64c10
28,37 #a64c10
29,37 #a64c10
30,37 #a64c10
31,37 #a64c10
32,37 #a64c10
33,37 #a64c10
34,37 #a64c10
35,37 #a64c10
36,37 #a64c10
37,37 #a64c10
38,37 #a64c10
39,37 #a64c10
40,37 #a64c10
#### #f5b658 (key e) - 83 px
45,15 #f5b658
46,15 #f5b658
47,15 #f5b658
48,15 #f5b658
49,15 #f5b658
44,16 #f5b658
45,16 #f5b658
46,16 #f5b658
47,16 #f5b658
24,26 #f5b658
25,26 #f5b658
26,26 #f5b658
27,26 #f5b658
28,26 #f5b658
29,26 #f5b658
30,26 #f5b658
31,26 #f5b658
32,26 #f5b658
33,26 #f5b658
34,26 #f5b658
35,26 #f5b658
36,26 #f5b658
8,27 #f5b658
9,27 #f5b658
10,27 #f5b658
11,27 #f5b658
12,27 #f5b658
13,27 #f5b658
14,27 #f5b658
15,27 #f5b658
16,27 #f5b658
21,27 #f5b658
22,27 #f5b658
23,27 #f5b658
24,27 #f5b658
25,27 #f5b658
26,27 #f5b658
27,27 #f5b658
28,27 #f5b658
29,27 #f5b658
30,27 #f5b658
31,27 #f5b658
32,27 #f5b658
33,27 #f5b658
34,27 #f5b658
35,27 #f5b658
36,27 #f5b658
37,27 #f5b658
38,27 #f5b658
8,28 #f5b658
9,28 #f5b658
10,28 #f5b658
11,28 #f5b658
12,28 #f5b658
13,28 #f5b658
14,28 #f5b658
15,28 #f5b658
16,28 #f5b658
17,28 #f5b658
19,28 #f5b658
20,28 #f5b658
21,28 #f5b658
22,28 #f5b658
23,28 #f5b658
24,28 #f5b658
25,28 #f5b658
26,28 #f5b658
27,28 #f5b658
28,28 #f5b658
29,28 #f5b658
30,28 #f5b658
31,28 #f5b658
32,28 #f5b658
33,28 #f5b658
34,28 #f5b658
35,28 #f5b658
36,28 #f5b658
37,28 #f5b658
38,28 #f5b658
39,28 #f5b658
40,28 #f5b658
41,28 #f5b658
42,28 #f5b658
#### #eec991 (key f) - 81 px
49,21 #eec991
50,21 #eec991
51,21 #eec991
52,21 #eec991
53,21 #eec991
54,21 #eec991
55,21 #eec991
56,21 #eec991
57,21 #eec991
58,21 #eec991
59,21 #eec991
46,22 #eec991
47,22 #eec991
48,22 #eec991
49,22 #eec991
50,22 #eec991
51,22 #eec991
52,22 #eec991
53,22 #eec991
54,22 #eec991
55,22 #eec991
56,22 #eec991
57,22 #eec991
47,23 #eec991
48,23 #eec991
49,23 #eec991
46,24 #eec991
47,24 #eec991
48,24 #eec991
49,24 #eec991
45,25 #eec991
46,25 #eec991
47,25 #eec991
48,25 #eec991
49,25 #eec991
44,26 #eec991
45,26 #eec991
46,26 #eec991
47,26 #eec991
48,26 #eec991
43,27 #eec991
44,27 #eec991
45,27 #eec991
46,27 #eec991
47,27 #eec991
4,28 #eec991
5,28 #eec991
6,28 #eec991
7,28 #eec991
43,28 #eec991
44,28 #eec991
45,28 #eec991
46,28 #eec991
3,29 #eec991
4,29 #eec991
5,29 #eec991
6,29 #eec991
7,29 #eec991
43,29 #eec991
44,29 #eec991
45,29 #eec991
3,30 #eec991
4,30 #eec991
5,30 #eec991
6,30 #eec991
7,30 #eec991
43,30 #eec991
44,30 #eec991
3,31 #eec991
4,31 #eec991
5,31 #eec991
6,31 #eec991
7,31 #eec991
43,31 #eec991
44,31 #eec991
4,32 #eec991
5,32 #eec991
6,32 #eec991
7,32 #eec991
6,33 #eec991
7,33 #eec991
#### #3a1818 (key g) - 41 px
46,9 #3a1818
51,9 #3a1818
45,10 #3a1818
50,10 #3a1818
45,11 #3a1818
46,11 #3a1818
50,11 #3a1818
51,11 #3a1818
45,12 #3a1818
46,12 #3a1818
50,12 #3a1818
51,12 #3a1818
45,13 #3a1818
46,13 #3a1818
50,13 #3a1818
51,13 #3a1818
45,14 #3a1818
46,14 #3a1818
50,14 #3a1818
51,14 #3a1818
50,17 #3a1818
60,20 #3a1818
21,45 #3a1818
21,46 #3a1818
44,46 #3a1818
21,47 #3a1818
44,47 #3a1818
20,48 #3a1818
21,48 #3a1818
43,48 #3a1818
44,48 #3a1818
20,49 #3a1818
21,49 #3a1818
44,49 #3a1818
45,49 #3a1818
20,50 #3a1818
21,50 #3a1818
22,50 #3a1818
44,50 #3a1818
45,50 #3a1818
46,50 #3a1818
#### #884315 (key h) - 34 px
22,43 #884315
23,43 #884315
41,43 #884315
42,43 #884315
22,44 #884315
23,44 #884315
41,44 #884315
42,44 #884315
23,45 #884315
24,45 #884315
41,45 #884315
42,45 #884315
23,46 #884315
24,46 #884315
41,46 #884315
42,46 #884315
23,47 #884315
24,47 #884315
41,47 #884315
42,47 #884315
23,48 #884315
24,48 #884315
40,48 #884315
41,48 #884315
24,49 #884315
25,49 #884315
40,49 #884315
41,49 #884315
24,50 #884315
25,50 #884315
26,50 #884315
40,50 #884315
41,50 #884315
42,50 #884315

## Frame 2 - changes from frame 1

239 pixels change. Set each to the listed colour, grouped by colour (key a #c5cded = clear back to background):
#### #c5cded (key a - BACKGROUND/clear) - 42 px
2,31 #c5cded
3,32 #c5cded
4,32 #c5cded
5,33 #c5cded
16,33 #c5cded
6,34 #c5cded
7,34 #c5cded
8,34 #c5cded
9,34 #c5cded
10,34 #c5cded
11,34 #c5cded
12,34 #c5cded
13,34 #c5cded
14,34 #c5cded
15,34 #c5cded
17,34 #c5cded
19,48 #c5cded
20,48 #c5cded
39,48 #c5cded
40,48 #c5cded
19,49 #c5cded
20,49 #c5cded
26,49 #c5cded
39,49 #c5cded
40,49 #c5cded
46,49 #c5cded
19,50 #c5cded
20,50 #c5cded
26,50 #c5cded
27,50 #c5cded
39,50 #c5cded
40,50 #c5cded
46,50 #c5cded
47,50 #c5cded
20,51 #c5cded
21,51 #c5cded
25,51 #c5cded
26,51 #c5cded
40,51 #c5cded
41,51 #c5cded
45,51 #c5cded
46,51 #c5cded
#### #c4550c (key b) - 20 px
8,28 #c4550c
9,28 #c4550c
10,28 #c4550c
11,28 #c4550c
12,28 #c4550c
13,28 #c4550c
14,28 #c4550c
15,28 #c4550c
16,28 #c4550c
19,34 #c4550c
19,35 #c4550c
44,36 #c4550c
44,37 #c4550c
20,38 #c4550c
44,38 #c4550c
20,39 #c4550c
44,39 #c4550c
20,40 #c4550c
44,40 #c4550c
21,42 #c4550c
#### #3a2518 (key c) - 92 px
8,25 #3a2518
9,25 #3a2518
10,25 #3a2518
11,25 #3a2518
12,25 #3a2518
13,25 #3a2518
14,25 #3a2518
15,25 #3a2518
16,25 #3a2518
4,26 #3a2518
5,26 #3a2518
6,26 #3a2518
7,26 #3a2518
17,26 #3a2518
3,27 #3a2518
2,28 #3a2518
17,28 #3a2518
3,31 #3a2518
5,32 #3a2518
16,32 #3a2518
6,33 #3a2518
7,33 #3a2518
8,33 #3a2518
9,33 #3a2518
10,33 #3a2518
11,33 #3a2518
12,33 #3a2518
13,33 #3a2518
14,33 #3a2518
15,33 #3a2518
18,34 #3a2518
21,34 #3a2518
18,35 #3a2518
21,35 #3a2518
42,36 #3a2518
42,37 #3a2518
19,38 #3a2518
22,38 #3a2518
42,38 #3a2518
45,38 #3a2518
19,39 #3a2518
22,39 #3a2518
25,39 #3a2518
39,39 #3a2518
42,39 #3a2518
45,39 #3a2518
19,40 #3a2518
22,40 #3a2518
25,40 #3a2518
39,40 #3a2518
42,40 #3a2518
45,40 #3a2518
25,41 #3a2518
39,41 #3a2518
42,41 #3a2518
45,41 #3a2518
23,42 #3a2518
25,42 #3a2518
42,42 #3a2518
45,42 #3a2518
23,43 #3a2518
25,43 #3a2518
42,43 #3a2518
45,43 #3a2518
23,44 #3a2518
25,44 #3a2518
42,44 #3a2518
45,44 #3a2518
23,45 #3a2518
42,45 #3a2518
45,45 #3a2518
23,46 #3a2518
42,46 #3a2518
23,47 #3a2518
42,47 #3a2518
21,48 #3a2518
24,48 #3a2518
26,48 #3a2518
41,48 #3a2518
46,48 #3a2518
21,49 #3a2518
24,49 #3a2518
25,49 #3a2518
41,49 #3a2518
44,49 #3a2518
45,49 #3a2518
21,50 #3a2518
25,50 #3a2518
41,50 #3a2518
45,50 #3a2518
23,51 #3a2518
43,51 #3a2518
#### #a64c10 (key d) - 24 px
8,31 #a64c10
9,31 #a64c10
10,31 #a64c10
11,31 #a64c10
12,31 #a64c10
13,31 #a64c10
14,31 #a64c10
15,31 #a64c10
16,31 #a64c10
22,34 #a64c10
22,35 #a64c10
41,36 #a64c10
41,37 #a64c10
23,39 #a64c10
24,39 #a64c10
40,39 #a64c10
41,39 #a64c10
23,40 #a64c10
24,40 #a64c10
40,40 #a64c10
41,40 #a64c10
40,41 #a64c10
41,41 #a64c10
41,42 #a64c10
#### #f5b658 (key e) - 10 px
8,26 #f5b658
9,26 #f5b658
10,26 #f5b658
11,26 #f5b658
12,26 #f5b658
13,26 #f5b658
14,26 #f5b658
15,26 #f5b658
16,26 #f5b658
17,27 #f5b658
#### #eec991 (key f) - 5 px
4,27 #eec991
5,27 #eec991
6,27 #eec991
7,27 #eec991
3,28 #eec991
#### #3a1818 (key g) - 16 px
24,41 #3a1818
24,42 #3a1818
24,43 #3a1818
41,43 #3a1818
24,44 #3a1818
41,44 #3a1818
24,45 #3a1818
41,45 #3a1818
24,46 #3a1818
41,46 #3a1818
24,47 #3a1818
41,47 #3a1818
25,48 #3a1818
42,49 #3a1818
42,50 #3a1818
43,50 #3a1818
#### #884315 (key h) - 30 px
43,41 #884315
44,41 #884315
43,42 #884315
44,42 #884315
21,43 #884315
43,43 #884315
44,43 #884315
21,44 #884315
43,44 #884315
44,44 #884315
21,45 #884315
22,45 #884315
43,45 #884315
44,45 #884315
21,46 #884315
22,46 #884315
43,46 #884315
44,46 #884315
21,47 #884315
22,47 #884315
43,47 #884315
44,47 #884315
22,48 #884315
43,48 #884315
44,48 #884315
45,48 #884315
22,49 #884315
23,49 #884315
22,50 #884315
23,50 #884315

## Frame 3 - changes from frame 2

343 pixels change. Set each to the listed colour, grouped by colour (key a #c5cded = clear back to background):
#### #c5cded (key a - BACKGROUND/clear) - 64 px
40,24 #c5cded
24,25 #c5cded
25,25 #c5cded
26,25 #c5cded
27,25 #c5cded
28,25 #c5cded
29,25 #c5cded
30,25 #c5cded
31,25 #c5cded
32,25 #c5cded
33,25 #c5cded
34,25 #c5cded
35,25 #c5cded
36,25 #c5cded
39,25 #c5cded
18,26 #c5cded
19,26 #c5cded
20,26 #c5cded
21,26 #c5cded
22,26 #c5cded
23,26 #c5cded
37,26 #c5cded
38,26 #c5cded
42,39 #c5cded
22,40 #c5cded
42,40 #c5cded
22,41 #c5cded
42,41 #c5cded
43,41 #c5cded
23,42 #c5cded
42,42 #c5cded
43,42 #c5cded
23,43 #c5cded
43,43 #c5cded
23,44 #c5cded
43,44 #c5cded
23,45 #c5cded
43,45 #c5cded
23,46 #c5cded
24,46 #c5cded
43,46 #c5cded
44,46 #c5cded
23,47 #c5cded
24,47 #c5cded
43,47 #c5cded
44,47 #c5cded
23,48 #c5cded
24,48 #c5cded
43,48 #c5cded
44,48 #c5cded
23,49 #c5cded
24,49 #c5cded
25,49 #c5cded
43,49 #c5cded
44,49 #c5cded
45,49 #c5cded
24,50 #c5cded
25,50 #c5cded
44,50 #c5cded
45,50 #c5cded
23,51 #c5cded
24,51 #c5cded
43,51 #c5cded
44,51 #c5cded
#### #c4550c (key b) - 37 px
39,28 #c4550c
40,28 #c4550c
18,32 #c4550c
21,32 #c4550c
42,32 #c4550c
22,34 #c4550c
23,34 #c4550c
24,34 #c4550c
25,34 #c4550c
26,34 #c4550c
27,34 #c4550c
28,34 #c4550c
29,34 #c4550c
30,34 #c4550c
31,34 #c4550c
32,34 #c4550c
33,34 #c4550c
34,34 #c4550c
35,34 #c4550c
36,34 #c4550c
37,34 #c4550c
38,34 #c4550c
39,34 #c4550c
40,34 #c4550c
19,36 #c4550c
45,36 #c4550c
19,37 #c4550c
45,37 #c4550c
19,38 #c4550c
45,38 #c4550c
19,39 #c4550c
45,39 #c4550c
19,40 #c4550c
45,40 #c4550c
19,41 #c4550c
20,41 #c4550c
20,42 #c4550c
#### #3a2518 (key c) - 135 px
40,25 #3a2518
24,26 #3a2518
25,26 #3a2518
26,26 #3a2518
27,26 #3a2518
28,26 #3a2518
29,26 #3a2518
30,26 #3a2518
31,26 #3a2518
32,26 #3a2518
33,26 #3a2518
34,26 #3a2518
35,26 #3a2518
36,26 #3a2518
39,26 #3a2518
21,27 #3a2518
22,27 #3a2518
23,27 #3a2518
37,27 #3a2518
38,27 #3a2518
19,28 #3a2518
20,28 #3a2518
18,29 #3a2518
18,36 #3a2518
21,36 #3a2518
43,36 #3a2518
46,36 #3a2518
18,37 #3a2518
21,37 #3a2518
43,37 #3a2518
46,37 #3a2518
18,38 #3a2518
21,38 #3a2518
43,38 #3a2518
46,38 #3a2518
18,39 #3a2518
21,39 #3a2518
23,39 #3a2518
24,39 #3a2518
26,39 #3a2518
27,39 #3a2518
28,39 #3a2518
29,39 #3a2518
30,39 #3a2518
31,39 #3a2518
32,39 #3a2518
33,39 #3a2518
34,39 #3a2518
35,39 #3a2518
36,39 #3a2518
37,39 #3a2518
38,39 #3a2518
40,39 #3a2518
41,39 #3a2518
43,39 #3a2518
46,39 #3a2518
18,40 #3a2518
21,40 #3a2518
23,40 #3a2518
26,40 #3a2518
38,40 #3a2518
41,40 #3a2518
43,40 #3a2518
46,40 #3a2518
18,41 #3a2518
21,41 #3a2518
26,41 #3a2518
38,41 #3a2518
41,41 #3a2518
44,41 #3a2518
47,41 #3a2518
19,42 #3a2518
22,42 #3a2518
24,42 #3a2518
27,42 #3a2518
38,42 #3a2518
41,42 #3a2518
44,42 #3a2518
47,42 #3a2518
19,43 #3a2518
22,43 #3a2518
24,43 #3a2518
27,43 #3a2518
39,43 #3a2518
44,43 #3a2518
47,43 #3a2518
19,44 #3a2518
22,44 #3a2518
24,44 #3a2518
27,44 #3a2518
39,44 #3a2518
44,44 #3a2518
47,44 #3a2518
19,45 #3a2518
22,45 #3a2518
24,45 #3a2518
27,45 #3a2518
39,45 #3a2518
44,45 #3a2518
47,45 #3a2518
19,46 #3a2518
22,46 #3a2518
28,46 #3a2518
39,46 #3a2518
48,46 #3a2518
19,47 #3a2518
22,47 #3a2518
28,47 #3a2518
39,47 #3a2518
48,47 #3a2518
19,48 #3a2518
22,48 #3a2518
25,48 #3a2518
29,48 #3a2518
39,48 #3a2518
45,48 #3a2518
49,48 #3a2518
19,49 #3a2518
22,49 #3a2518
26,49 #3a2518
27,49 #3a2518
28,49 #3a2518
39,49 #3a2518
42,49 #3a2518
46,49 #3a2518
47,49 #3a2518
48,49 #3a2518
19,50 #3a2518
23,50 #3a2518
39,50 #3a2518
43,50 #3a2518
20,51 #3a2518
21,51 #3a2518
40,51 #3a2518
41,51 #3a2518
#### #a64c10 (key d) - 28 px
22,36 #a64c10
42,36 #a64c10
22,37 #a64c10
42,37 #a64c10
22,38 #a64c10
23,38 #a64c10
24,38 #a64c10
25,38 #a64c10
26,38 #a64c10
27,38 #a64c10
28,38 #a64c10
29,38 #a64c10
30,38 #a64c10
31,38 #a64c10
32,38 #a64c10
33,38 #a64c10
34,38 #a64c10
35,38 #a64c10
36,38 #a64c10
37,38 #a64c10
38,38 #a64c10
39,38 #a64c10
40,38 #a64c10
25,40 #a64c10
39,40 #a64c10
39,41 #a64c10
39,42 #a64c10
40,42 #a64c10
#### #f5b658 (key e) - 22 px
19,29 #f5b658
20,29 #f5b658
21,29 #f5b658
22,29 #f5b658
23,29 #f5b658
24,29 #f5b658
25,29 #f5b658
26,29 #f5b658
27,29 #f5b658
28,29 #f5b658
29,29 #f5b658
30,29 #f5b658
31,29 #f5b658
32,29 #f5b658
33,29 #f5b658
34,29 #f5b658
35,29 #f5b658
36,29 #f5b658
37,29 #f5b658
38,29 #f5b658
39,29 #f5b658
40,29 #f5b658
#### #eec991 (key f) - 2 px
43,32 #eec991
44,32 #eec991
#### #3a1818 (key g) - 27 px
25,41 #3a1818
25,42 #3a1818
26,42 #3a1818
25,43 #3a1818
26,43 #3a1818
40,43 #3a1818
25,44 #3a1818
26,44 #3a1818
40,44 #3a1818
25,45 #3a1818
26,45 #3a1818
40,45 #3a1818
26,46 #3a1818
27,46 #3a1818
40,46 #3a1818
26,47 #3a1818
27,47 #3a1818
40,47 #3a1818
26,48 #3a1818
27,48 #3a1818
28,48 #3a1818
40,48 #3a1818
41,48 #3a1818
40,49 #3a1818
41,49 #3a1818
40,50 #3a1818
41,50 #3a1818
#### #884315 (key h) - 28 px
45,41 #884315
46,41 #884315
45,42 #884315
46,42 #884315
20,43 #884315
45,43 #884315
46,43 #884315
20,44 #884315
45,44 #884315
46,44 #884315
20,45 #884315
45,45 #884315
46,45 #884315
20,46 #884315
46,46 #884315
47,46 #884315
20,47 #884315
46,47 #884315
47,47 #884315
20,48 #884315
21,48 #884315
46,48 #884315
47,48 #884315
48,48 #884315
20,49 #884315
21,49 #884315
20,50 #884315
21,50 #884315

## Frame 4 - changes from frame 3

289 pixels change. Set each to the listed colour, grouped by colour (key a #c5cded = clear back to background):
#### #c5cded (key a - BACKGROUND/clear) - 77 px
8,25 #c5cded
9,25 #c5cded
10,25 #c5cded
11,25 #c5cded
12,25 #c5cded
13,25 #c5cded
14,25 #c5cded
15,25 #c5cded
16,25 #c5cded
4,26 #c5cded
5,26 #c5cded
6,26 #c5cded
7,26 #c5cded
17,26 #c5cded
3,27 #c5cded
2,28 #c5cded
43,39 #c5cded
23,40 #c5cded
43,40 #c5cded
23,41 #c5cded
21,42 #c5cded
22,42 #c5cded
44,42 #c5cded
21,43 #c5cded
22,43 #c5cded
24,43 #c5cded
41,43 #c5cded
42,43 #c5cded
44,43 #c5cded
21,44 #c5cded
22,44 #c5cded
24,44 #c5cded
41,44 #c5cded
42,44 #c5cded
44,44 #c5cded
21,45 #c5cded
22,45 #c5cded
24,45 #c5cded
25,45 #c5cded
41,45 #c5cded
42,45 #c5cded
44,45 #c5cded
45,45 #c5cded
21,46 #c5cded
22,46 #c5cded
25,46 #c5cded
41,46 #c5cded
42,46 #c5cded
45,46 #c5cded
21,47 #c5cded
22,47 #c5cded
25,47 #c5cded
41,47 #c5cded
42,47 #c5cded
45,47 #c5cded
21,48 #c5cded
22,48 #c5cded
25,48 #c5cded
26,48 #c5cded
41,48 #c5cded
42,48 #c5cded
45,48 #c5cded
46,48 #c5cded
21,49 #c5cded
22,49 #c5cded
26,49 #c5cded
41,49 #c5cded
42,49 #c5cded
46,49 #c5cded
22,50 #c5cded
23,50 #c5cded
42,50 #c5cded
43,50 #c5cded
21,51 #c5cded
22,51 #c5cded
41,51 #c5cded
42,51 #c5cded
#### #c4550c (key b) - 17 px
8,31 #c4550c
9,31 #c4550c
10,31 #c4550c
11,31 #c4550c
12,31 #c4550c
13,31 #c4550c
14,31 #c4550c
15,31 #c4550c
16,31 #c4550c
45,35 #c4550c
46,38 #c4550c
46,39 #c4550c
46,40 #c4550c
45,41 #c4550c
46,41 #c4550c
18,42 #c4550c
19,42 #c4550c
#### #3a2518 (key c) - 114 px
8,26 #3a2518
9,26 #3a2518
10,26 #3a2518
11,26 #3a2518
12,26 #3a2518
13,26 #3a2518
14,26 #3a2518
15,26 #3a2518
16,26 #3a2518
4,27 #3a2518
5,27 #3a2518
6,27 #3a2518
7,27 #3a2518
17,27 #3a2518
3,28 #3a2518
2,31 #3a2518
3,32 #3a2518
5,33 #3a2518
16,33 #3a2518
6,34 #3a2518
7,34 #3a2518
8,34 #3a2518
9,34 #3a2518
10,34 #3a2518
11,34 #3a2518
12,34 #3a2518
13,34 #3a2518
14,34 #3a2518
15,34 #3a2518
17,34 #3a2518
43,35 #3a2518
46,35 #3a2518
44,38 #3a2518
47,38 #3a2518
44,39 #3a2518
47,39 #3a2518
24,40 #3a2518
27,40 #3a2518
44,40 #3a2518
47,40 #3a2518
24,41 #3a2518
27,41 #3a2518
17,42 #3a2518
20,42 #3a2518
45,42 #3a2518
48,42 #3a2518
17,43 #3a2518
20,43 #3a2518
25,43 #3a2518
28,43 #3a2518
37,43 #3a2518
40,43 #3a2518
45,43 #3a2518
48,43 #3a2518
17,44 #3a2518
20,44 #3a2518
25,44 #3a2518
28,44 #3a2518
37,44 #3a2518
40,44 #3a2518
45,44 #3a2518
48,44 #3a2518
17,45 #3a2518
20,45 #3a2518
26,45 #3a2518
29,45 #3a2518
37,45 #3a2518
40,45 #3a2518
46,45 #3a2518
49,45 #3a2518
17,46 #3a2518
20,46 #3a2518
26,46 #3a2518
29,46 #3a2518
37,46 #3a2518
40,46 #3a2518
46,46 #3a2518
49,46 #3a2518
17,47 #3a2518
20,47 #3a2518
26,47 #3a2518
29,47 #3a2518
37,47 #3a2518
40,47 #3a2518
46,47 #3a2518
49,47 #3a2518
17,48 #3a2518
20,48 #3a2518
27,48 #3a2518
30,48 #3a2518
37,48 #3a2518
40,48 #3a2518
47,48 #3a2518
50,48 #3a2518
17,49 #3a2518
20,49 #3a2518
31,49 #3a2518
37,49 #3a2518
40,49 #3a2518
51,49 #3a2518
17,50 #3a2518
21,50 #3a2518
28,50 #3a2518
29,50 #3a2518
30,50 #3a2518
37,50 #3a2518
41,50 #3a2518
48,50 #3a2518
49,50 #3a2518
50,50 #3a2518
18,51 #3a2518
19,51 #3a2518
38,51 #3a2518
39,51 #3a2518
#### #a64c10 (key d) - 13 px
16,32 #a64c10
8,33 #a64c10
9,33 #a64c10
10,33 #a64c10
11,33 #a64c10
12,33 #a64c10
13,33 #a64c10
14,33 #a64c10
15,33 #a64c10
42,35 #a64c10
26,40 #a64c10
25,41 #a64c10
26,41 #a64c10
#### #f5b658 (key e) - 10 px
8,28 #f5b658
9,28 #f5b658
10,28 #f5b658
11,28 #f5b658
12,28 #f5b658
13,28 #f5b658
14,28 #f5b658
15,28 #f5b658
16,28 #f5b658
17,28 #f5b658
#### #eec991 (key f) - 5 px
3,31 #eec991
4,32 #eec991
5,32 #eec991
6,33 #eec991
7,33 #eec991
#### #3a1818 (key g) - 26 px
27,43 #3a1818
38,43 #3a1818
39,43 #3a1818
27,44 #3a1818
38,44 #3a1818
39,44 #3a1818
27,45 #3a1818
28,45 #3a1818
38,45 #3a1818
39,45 #3a1818
28,46 #3a1818
38,46 #3a1818
39,46 #3a1818
28,47 #3a1818
38,47 #3a1818
39,47 #3a1818
29,48 #3a1818
38,48 #3a1818
39,48 #3a1818
28,49 #3a1818
29,49 #3a1818
30,49 #3a1818
38,49 #3a1818
39,49 #3a1818
38,50 #3a1818
39,50 #3a1818
#### #884315 (key h) - 27 px
47,42 #884315
18,43 #884315
19,43 #884315
47,43 #884315
18,44 #884315
19,44 #884315
47,44 #884315
18,45 #884315
19,45 #884315
47,45 #884315
48,45 #884315
18,46 #884315
19,46 #884315
48,46 #884315
18,47 #884315
19,47 #884315
48,47 #884315
18,48 #884315
19,48 #884315
49,48 #884315
18,49 #884315
19,49 #884315
48,49 #884315
49,49 #884315
50,49 #884315
18,50 #884315
19,50 #884315

## Frame 5 - changes from frame 4

295 pixels change. Set each to the listed colour, grouped by colour (key a #c5cded = clear back to background):
#### #c5cded (key a - BACKGROUND/clear) - 53 px
21,38 #c5cded
21,39 #c5cded
22,39 #c5cded
23,39 #c5cded
28,39 #c5cded
29,39 #c5cded
30,39 #c5cded
31,39 #c5cded
32,39 #c5cded
33,39 #c5cded
34,39 #c5cded
35,39 #c5cded
36,39 #c5cded
41,39 #c5cded
21,40 #c5cded
41,40 #c5cded
20,41 #c5cded
21,41 #c5cded
41,41 #c5cded
20,42 #c5cded
40,42 #c5cded
41,42 #c5cded
20,43 #c5cded
40,43 #c5cded
20,44 #c5cded
40,44 #c5cded
20,45 #c5cded
29,45 #c5cded
40,45 #c5cded
20,46 #c5cded
40,46 #c5cded
20,47 #c5cded
40,47 #c5cded
19,48 #c5cded
20,48 #c5cded
30,48 #c5cded
39,48 #c5cded
40,48 #c5cded
50,48 #c5cded
19,49 #c5cded
20,49 #c5cded
31,49 #c5cded
39,49 #c5cded
40,49 #c5cded
51,49 #c5cded
20,50 #c5cded
21,50 #c5cded
40,50 #c5cded
41,50 #c5cded
19,51 #c5cded
20,51 #c5cded
39,51 #c5cded
40,51 #c5cded
#### #c4550c (key b) - 38 px
40,25 #c4550c
39,26 #c4550c
18,29 #c4550c
19,29 #c4550c
20,29 #c4550c
21,29 #c4550c
22,29 #c4550c
23,29 #c4550c
24,29 #c4550c
25,29 #c4550c
26,29 #c4550c
27,29 #c4550c
28,29 #c4550c
29,29 #c4550c
30,29 #c4550c
31,29 #c4550c
32,29 #c4550c
33,29 #c4550c
34,29 #c4550c
35,29 #c4550c
36,29 #c4550c
37,29 #c4550c
38,29 #c4550c
39,29 #c4550c
40,29 #c4550c
43,32 #c4550c
44,32 #c4550c
45,34 #c4550c
18,36 #c4550c
18,37 #c4550c
18,38 #c4550c
18,39 #c4550c
18,40 #c4550c
17,41 #c4550c
18,41 #c4550c
17,42 #c4550c
46,42 #c4550c
47,42 #c4550c
#### #3a2518 (key c) - 121 px
40,24 #3a2518
24,25 #3a2518
25,25 #3a2518
26,25 #3a2518
27,25 #3a2518
28,25 #3a2518
29,25 #3a2518
30,25 #3a2518
31,25 #3a2518
32,25 #3a2518
33,25 #3a2518
34,25 #3a2518
35,25 #3a2518
36,25 #3a2518
39,25 #3a2518
18,26 #3a2518
19,26 #3a2518
20,26 #3a2518
21,26 #3a2518
22,26 #3a2518
23,26 #3a2518
37,26 #3a2518
38,26 #3a2518
18,32 #3a2518
21,32 #3a2518
42,32 #3a2518
43,34 #3a2518
46,34 #3a2518
17,36 #3a2518
20,36 #3a2518
17,37 #3a2518
20,37 #3a2518
17,38 #3a2518
20,38 #3a2518
22,38 #3a2518
23,38 #3a2518
24,38 #3a2518
25,38 #3a2518
26,38 #3a2518
27,38 #3a2518
28,38 #3a2518
29,38 #3a2518
30,38 #3a2518
31,38 #3a2518
32,38 #3a2518
33,38 #3a2518
34,38 #3a2518
35,38 #3a2518
36,38 #3a2518
37,38 #3a2518
38,38 #3a2518
39,38 #3a2518
40,38 #3a2518
17,39 #3a2518
20,39 #3a2518
17,40 #3a2518
20,40 #3a2518
37,40 #3a2518
40,40 #3a2518
16,41 #3a2518
19,41 #3a2518
37,41 #3a2518
40,41 #3a2518
16,42 #3a2518
19,42 #3a2518
36,42 #3a2518
39,42 #3a2518
16,43 #3a2518
19,43 #3a2518
36,43 #3a2518
39,43 #3a2518
16,44 #3a2518
19,44 #3a2518
36,44 #3a2518
39,44 #3a2518
16,45 #3a2518
19,45 #3a2518
25,45 #3a2518
28,45 #3a2518
36,45 #3a2518
39,45 #3a2518
16,46 #3a2518
19,46 #3a2518
36,46 #3a2518
39,46 #3a2518
16,47 #3a2518
19,47 #3a2518
36,47 #3a2518
39,47 #3a2518
15,48 #3a2518
18,48 #3a2518
26,48 #3a2518
29,48 #3a2518
35,48 #3a2518
38,48 #3a2518
46,48 #3a2518
49,48 #3a2518
15,49 #3a2518
18,49 #3a2518
30,49 #3a2518
35,49 #3a2518
38,49 #3a2518
50,49 #3a2518
15,50 #3a2518
19,50 #3a2518
27,50 #3a2518
31,50 #3a2518
35,50 #3a2518
39,50 #3a2518
47,50 #3a2518
51,50 #3a2518
16,51 #3a2518
17,51 #3a2518
28,51 #3a2518
29,51 #3a2518
30,51 #3a2518
36,51 #3a2518
37,51 #3a2518
48,51 #3a2518
49,51 #3a2518
50,51 #3a2518
#### #a64c10 (key d) - 30 px
22,34 #a64c10
23,34 #a64c10
24,34 #a64c10
25,34 #a64c10
26,34 #a64c10
27,34 #a64c10
28,34 #a64c10
29,34 #a64c10
30,34 #a64c10
31,34 #a64c10
32,34 #a64c10
33,34 #a64c10
34,34 #a64c10
35,34 #a64c10
36,34 #a64c10
37,34 #a64c10
38,34 #a64c10
39,34 #a64c10
40,34 #a64c10
42,34 #a64c10
25,39 #a64c10
26,39 #a64c10
38,39 #a64c10
39,39 #a64c10
38,40 #a64c10
38,41 #a64c10
25,42 #a64c10
26,42 #a64c10
37,42 #a64c10
38,42 #a64c10
#### #f5b658 (key e) - 22 px
24,26 #f5b658
25,26 #f5b658
26,26 #f5b658
27,26 #f5b658
28,26 #f5b658
29,26 #f5b658
30,26 #f5b658
31,26 #f5b658
32,26 #f5b658
33,26 #f5b658
34,26 #f5b658
35,26 #f5b658
36,26 #f5b658
21,27 #f5b658
22,27 #f5b658
23,27 #f5b658
37,27 #f5b658
38,27 #f5b658
19,28 #f5b658
20,28 #f5b658
39,28 #f5b658
40,28 #f5b658
#### #3a1818 (key g) - 16 px
37,43 #3a1818
37,44 #3a1818
26,45 #3a1818
37,45 #3a1818
37,46 #3a1818
37,47 #3a1818
27,48 #3a1818
36,48 #3a1818
37,48 #3a1818
36,49 #3a1818
37,49 #3a1818
28,50 #3a1818
29,50 #3a1818
30,50 #3a1818
36,50 #3a1818
37,50 #3a1818
#### #884315 (key h) - 15 px
17,43 #884315
17,44 #884315
17,45 #884315
17,46 #884315
17,47 #884315
16,48 #884315
17,48 #884315
47,48 #884315
16,49 #884315
17,49 #884315
16,50 #884315
17,50 #884315
48,50 #884315
49,50 #884315
50,50 #884315

## Frame 6 - changes from frame 5

357 pixels change. Set each to the listed colour, grouped by colour (key a #c5cded = clear back to background):
#### #c5cded (key a - BACKGROUND/clear) - 118 px
2,31 #c5cded
3,32 #c5cded
4,32 #c5cded
5,33 #c5cded
16,33 #c5cded
6,34 #c5cded
7,34 #c5cded
8,34 #c5cded
9,34 #c5cded
10,34 #c5cded
11,34 #c5cded
12,34 #c5cded
13,34 #c5cded
14,34 #c5cded
15,34 #c5cded
17,34 #c5cded
46,34 #c5cded
46,35 #c5cded
17,36 #c5cded
17,37 #c5cded
17,38 #c5cded
47,38 #c5cded
17,39 #c5cded
27,39 #c5cded
37,39 #c5cded
47,39 #c5cded
17,40 #c5cded
27,40 #c5cded
37,40 #c5cded
47,40 #c5cded
16,41 #c5cded
17,41 #c5cded
27,41 #c5cded
37,41 #c5cded
16,42 #c5cded
17,42 #c5cded
36,42 #c5cded
37,42 #c5cded
48,42 #c5cded
16,43 #c5cded
17,43 #c5cded
28,43 #c5cded
36,43 #c5cded
37,43 #c5cded
48,43 #c5cded
16,44 #c5cded
17,44 #c5cded
28,44 #c5cded
36,44 #c5cded
37,44 #c5cded
48,44 #c5cded
16,45 #c5cded
17,45 #c5cded
28,45 #c5cded
36,45 #c5cded
37,45 #c5cded
48,45 #c5cded
49,45 #c5cded
16,46 #c5cded
17,46 #c5cded
28,46 #c5cded
29,46 #c5cded
36,46 #c5cded
37,46 #c5cded
48,46 #c5cded
49,46 #c5cded
16,47 #c5cded
17,47 #c5cded
28,47 #c5cded
29,47 #c5cded
36,47 #c5cded
37,47 #c5cded
48,47 #c5cded
49,47 #c5cded
15,48 #c5cded
16,48 #c5cded
17,48 #c5cded
29,48 #c5cded
35,48 #c5cded
36,48 #c5cded
37,48 #c5cded
49,48 #c5cded
15,49 #c5cded
16,49 #c5cded
17,49 #c5cded
18,49 #c5cded
29,49 #c5cded
30,49 #c5cded
35,49 #c5cded
36,49 #c5cded
37,49 #c5cded
38,49 #c5cded
49,49 #c5cded
50,49 #c5cded
15,50 #c5cded
16,50 #c5cded
17,50 #c5cded
18,50 #c5cded
19,50 #c5cded
30,50 #c5cded
31,50 #c5cded
35,50 #c5cded
36,50 #c5cded
37,50 #c5cded
38,50 #c5cded
39,50 #c5cded
50,50 #c5cded
51,50 #c5cded
16,51 #c5cded
17,51 #c5cded
18,51 #c5cded
29,51 #c5cded
30,51 #c5cded
36,51 #c5cded
37,51 #c5cded
38,51 #c5cded
49,51 #c5cded
50,51 #c5cded
#### #c4550c (key b) - 20 px
8,28 #c4550c
9,28 #c4550c
10,28 #c4550c
11,28 #c4550c
12,28 #c4550c
13,28 #c4550c
14,28 #c4550c
15,28 #c4550c
16,28 #c4550c
43,34 #c4550c
43,35 #c4550c
20,36 #c4550c
20,37 #c4550c
20,38 #c4550c
44,38 #c4550c
20,39 #c4550c
44,39 #c4550c
20,40 #c4550c
44,40 #c4550c
45,42 #c4550c
#### #3a2518 (key c) - 131 px
8,25 #3a2518
9,25 #3a2518
10,25 #3a2518
11,25 #3a2518
12,25 #3a2518
13,25 #3a2518
14,25 #3a2518
15,25 #3a2518
16,25 #3a2518
4,26 #3a2518
5,26 #3a2518
6,26 #3a2518
7,26 #3a2518
17,26 #3a2518
3,27 #3a2518
2,28 #3a2518
17,28 #3a2518
3,31 #3a2518
5,32 #3a2518
16,32 #3a2518
6,33 #3a2518
7,33 #3a2518
8,33 #3a2518
9,33 #3a2518
10,33 #3a2518
11,33 #3a2518
12,33 #3a2518
13,33 #3a2518
14,33 #3a2518
15,33 #3a2518
42,34 #3a2518
45,34 #3a2518
42,35 #3a2518
45,35 #3a2518
18,36 #3a2518
18,37 #3a2518
18,38 #3a2518
21,38 #3a2518
46,38 #3a2518
18,39 #3a2518
21,39 #3a2518
23,39 #3a2518
26,39 #3a2518
38,39 #3a2518
41,39 #3a2518
43,39 #3a2518
46,39 #3a2518
18,40 #3a2518
21,40 #3a2518
23,40 #3a2518
26,40 #3a2518
38,40 #3a2518
41,40 #3a2518
43,40 #3a2518
46,40 #3a2518
18,41 #3a2518
21,41 #3a2518
23,41 #3a2518
26,41 #3a2518
38,41 #3a2518
41,41 #3a2518
18,42 #3a2518
21,42 #3a2518
38,42 #3a2518
41,42 #3a2518
44,42 #3a2518
47,42 #3a2518
18,43 #3a2518
21,43 #3a2518
24,43 #3a2518
27,43 #3a2518
38,43 #3a2518
41,43 #3a2518
44,43 #3a2518
47,43 #3a2518
18,44 #3a2518
21,44 #3a2518
24,44 #3a2518
27,44 #3a2518
38,44 #3a2518
41,44 #3a2518
44,44 #3a2518
47,44 #3a2518
18,45 #3a2518
21,45 #3a2518
24,45 #3a2518
27,45 #3a2518
38,45 #3a2518
41,45 #3a2518
44,45 #3a2518
47,45 #3a2518
18,46 #3a2518
21,46 #3a2518
24,46 #3a2518
27,46 #3a2518
38,46 #3a2518
41,46 #3a2518
44,46 #3a2518
47,46 #3a2518
18,47 #3a2518
21,47 #3a2518
24,47 #3a2518
27,47 #3a2518
38,47 #3a2518
41,47 #3a2518
44,47 #3a2518
47,47 #3a2518
22,48 #3a2518
25,48 #3a2518
28,48 #3a2518
42,48 #3a2518
45,48 #3a2518
48,48 #3a2518
19,49 #3a2518
20,49 #3a2518
21,49 #3a2518
25,49 #3a2518
28,49 #3a2518
39,49 #3a2518
40,49 #3a2518
41,49 #3a2518
45,49 #3a2518
48,49 #3a2518
25,50 #3a2518
29,50 #3a2518
45,50 #3a2518
49,50 #3a2518
26,51 #3a2518
27,51 #3a2518
46,51 #3a2518
47,51 #3a2518
#### #a64c10 (key d) - 14 px
8,31 #a64c10
9,31 #a64c10
10,31 #a64c10
11,31 #a64c10
12,31 #a64c10
13,31 #a64c10
14,31 #a64c10
15,31 #a64c10
16,31 #a64c10
24,39 #a64c10
40,39 #a64c10
24,40 #a64c10
40,40 #a64c10
24,41 #a64c10
#### #f5b658 (key e) - 10 px
8,26 #f5b658
9,26 #f5b658
10,26 #f5b658
11,26 #f5b658
12,26 #f5b658
13,26 #f5b658
14,26 #f5b658
15,26 #f5b658
16,26 #f5b658
17,27 #f5b658
#### #eec991 (key f) - 5 px
4,27 #eec991
5,27 #eec991
6,27 #eec991
7,27 #eec991
3,28 #eec991
#### #3a1818 (key g) - 29 px
39,41 #3a1818
40,41 #3a1818
39,42 #3a1818
40,42 #3a1818
25,43 #3a1818
39,43 #3a1818
40,43 #3a1818
25,44 #3a1818
39,44 #3a1818
40,44 #3a1818
25,45 #3a1818
39,45 #3a1818
40,45 #3a1818
25,46 #3a1818
26,46 #3a1818
39,46 #3a1818
40,46 #3a1818
25,47 #3a1818
26,47 #3a1818
39,47 #3a1818
40,47 #3a1818
26,48 #3a1818
39,48 #3a1818
40,48 #3a1818
41,48 #3a1818
26,49 #3a1818
27,49 #3a1818
26,50 #3a1818
27,50 #3a1818
#### #884315 (key h) - 30 px
19,41 #884315
20,41 #884315
19,42 #884315
20,42 #884315
19,43 #884315
20,43 #884315
45,43 #884315
19,44 #884315
20,44 #884315
45,44 #884315
19,45 #884315
20,45 #884315
45,45 #884315
46,45 #884315
19,46 #884315
20,46 #884315
45,46 #884315
46,46 #884315
19,47 #884315
20,47 #884315
45,47 #884315
46,47 #884315
19,48 #884315
20,48 #884315
21,48 #884315
46,48 #884315
46,49 #884315
47,49 #884315
46,50 #884315
47,50 #884315

## Frame 7 - changes from frame 6

352 pixels change. Set each to the listed colour, grouped by colour (key a #c5cded = clear back to background):
#### #c5cded (key a - BACKGROUND/clear) - 110 px
40,24 #c5cded
24,25 #c5cded
25,25 #c5cded
26,25 #c5cded
27,25 #c5cded
28,25 #c5cded
29,25 #c5cded
30,25 #c5cded
31,25 #c5cded
32,25 #c5cded
33,25 #c5cded
34,25 #c5cded
35,25 #c5cded
36,25 #c5cded
39,25 #c5cded
18,26 #c5cded
19,26 #c5cded
20,26 #c5cded
21,26 #c5cded
22,26 #c5cded
23,26 #c5cded
37,26 #c5cded
38,26 #c5cded
18,36 #c5cded
46,36 #c5cded
18,37 #c5cded
46,37 #c5cded
18,38 #c5cded
46,38 #c5cded
18,39 #c5cded
46,39 #c5cded
18,40 #c5cded
26,40 #c5cded
38,40 #c5cded
46,40 #c5cded
18,41 #c5cded
19,41 #c5cded
26,41 #c5cded
38,41 #c5cded
46,41 #c5cded
47,41 #c5cded
18,42 #c5cded
19,42 #c5cded
26,42 #c5cded
27,42 #c5cded
38,42 #c5cded
39,42 #c5cded
47,42 #c5cded
18,43 #c5cded
19,43 #c5cded
27,43 #c5cded
38,43 #c5cded
39,43 #c5cded
47,43 #c5cded
18,44 #c5cded
19,44 #c5cded
27,44 #c5cded
38,44 #c5cded
39,44 #c5cded
47,44 #c5cded
18,45 #c5cded
19,45 #c5cded
27,45 #c5cded
38,45 #c5cded
39,45 #c5cded
47,45 #c5cded
18,46 #c5cded
19,46 #c5cded
20,46 #c5cded
27,46 #c5cded
38,46 #c5cded
39,46 #c5cded
40,46 #c5cded
47,46 #c5cded
18,47 #c5cded
19,47 #c5cded
20,47 #c5cded
27,47 #c5cded
38,47 #c5cded
39,47 #c5cded
40,47 #c5cded
47,47 #c5cded
18,48 #c5cded
19,48 #c5cded
20,48 #c5cded
27,48 #c5cded
28,48 #c5cded
38,48 #c5cded
39,48 #c5cded
40,48 #c5cded
47,48 #c5cded
48,48 #c5cded
19,49 #c5cded
20,49 #c5cded
21,49 #c5cded
27,49 #c5cded
28,49 #c5cded
39,49 #c5cded
40,49 #c5cded
41,49 #c5cded
47,49 #c5cded
48,49 #c5cded
28,50 #c5cded
29,50 #c5cded
48,50 #c5cded
49,50 #c5cded
27,51 #c5cded
28,51 #c5cded
47,51 #c5cded
48,51 #c5cded
#### #c4550c (key b) - 37 px
39,28 #c4550c
40,28 #c4550c
18,32 #c4550c
21,32 #c4550c
42,32 #c4550c
22,34 #c4550c
23,34 #c4550c
24,34 #c4550c
25,34 #c4550c
26,34 #c4550c
27,34 #c4550c
28,34 #c4550c
29,34 #c4550c
30,34 #c4550c
31,34 #c4550c
32,34 #c4550c
33,34 #c4550c
34,34 #c4550c
35,34 #c4550c
36,34 #c4550c
37,34 #c4550c
38,34 #c4550c
39,34 #c4550c
40,34 #c4550c
21,36 #c4550c
43,36 #c4550c
21,37 #c4550c
43,37 #c4550c
21,38 #c4550c
43,38 #c4550c
21,39 #c4550c
43,39 #c4550c
21,40 #c4550c
43,40 #c4550c
43,41 #c4550c
44,41 #c4550c
44,42 #c4550c
#### #3a2518 (key c) - 113 px
40,25 #3a2518
24,26 #3a2518
25,26 #3a2518
26,26 #3a2518
27,26 #3a2518
28,26 #3a2518
29,26 #3a2518
30,26 #3a2518
31,26 #3a2518
32,26 #3a2518
33,26 #3a2518
34,26 #3a2518
35,26 #3a2518
36,26 #3a2518
39,26 #3a2518
21,27 #3a2518
22,27 #3a2518
23,27 #3a2518
37,27 #3a2518
38,27 #3a2518
19,28 #3a2518
20,28 #3a2518
18,29 #3a2518
19,36 #3a2518
22,36 #3a2518
42,36 #3a2518
45,36 #3a2518
19,37 #3a2518
22,37 #3a2518
42,37 #3a2518
45,37 #3a2518
19,38 #3a2518
45,38 #3a2518
19,39 #3a2518
22,39 #3a2518
24,39 #3a2518
25,39 #3a2518
27,39 #3a2518
28,39 #3a2518
29,39 #3a2518
30,39 #3a2518
31,39 #3a2518
32,39 #3a2518
33,39 #3a2518
34,39 #3a2518
35,39 #3a2518
36,39 #3a2518
37,39 #3a2518
39,39 #3a2518
40,39 #3a2518
42,39 #3a2518
45,39 #3a2518
19,40 #3a2518
22,40 #3a2518
25,40 #3a2518
39,40 #3a2518
42,40 #3a2518
45,40 #3a2518
20,41 #3a2518
25,41 #3a2518
39,41 #3a2518
42,41 #3a2518
45,41 #3a2518
20,42 #3a2518
23,42 #3a2518
25,42 #3a2518
40,42 #3a2518
43,42 #3a2518
46,42 #3a2518
20,43 #3a2518
23,43 #3a2518
26,43 #3a2518
40,43 #3a2518
43,43 #3a2518
46,43 #3a2518
20,44 #3a2518
23,44 #3a2518
26,44 #3a2518
40,44 #3a2518
43,44 #3a2518
46,44 #3a2518
20,45 #3a2518
23,45 #3a2518
26,45 #3a2518
40,45 #3a2518
43,45 #3a2518
46,45 #3a2518
26,46 #3a2518
43,46 #3a2518
46,46 #3a2518
26,47 #3a2518
43,47 #3a2518
46,47 #3a2518
21,48 #3a2518
26,48 #3a2518
41,48 #3a2518
43,48 #3a2518
46,48 #3a2518
22,49 #3a2518
23,49 #3a2518
24,49 #3a2518
26,49 #3a2518
42,49 #3a2518
43,49 #3a2518
46,49 #3a2518
23,50 #3a2518
27,50 #3a2518
43,50 #3a2518
47,50 #3a2518
24,51 #3a2518
25,51 #3a2518
44,51 #3a2518
45,51 #3a2518
#### #a64c10 (key d) - 22 px
23,38 #a64c10
24,38 #a64c10
25,38 #a64c10
26,38 #a64c10
27,38 #a64c10
28,38 #a64c10
29,38 #a64c10
30,38 #a64c10
31,38 #a64c10
32,38 #a64c10
33,38 #a64c10
34,38 #a64c10
35,38 #a64c10
36,38 #a64c10
37,38 #a64c10
38,38 #a64c10
39,38 #a64c10
40,38 #a64c10
41,39 #a64c10
23,40 #a64c10
41,40 #a64c10
24,42 #a64c10
#### #f5b658 (key e) - 22 px
19,29 #f5b658
20,29 #f5b658
21,29 #f5b658
22,29 #f5b658
23,29 #f5b658
24,29 #f5b658
25,29 #f5b658
26,29 #f5b658
27,29 #f5b658
28,29 #f5b658
29,29 #f5b658
30,29 #f5b658
31,29 #f5b658
32,29 #f5b658
33,29 #f5b658
34,29 #f5b658
35,29 #f5b658
36,29 #f5b658
37,29 #f5b658
38,29 #f5b658
39,29 #f5b658
40,29 #f5b658
#### #eec991 (key f) - 2 px
43,32 #eec991
44,32 #eec991
#### #3a1818 (key g) - 18 px
41,41 #3a1818
41,42 #3a1818
42,42 #3a1818
24,43 #3a1818
41,43 #3a1818
42,43 #3a1818
24,44 #3a1818
41,44 #3a1818
42,44 #3a1818
24,45 #3a1818
41,45 #3a1818
42,45 #3a1818
42,46 #3a1818
42,47 #3a1818
42,48 #3a1818
25,49 #3a1818
24,50 #3a1818
25,50 #3a1818
#### #884315 (key h) - 28 px
21,41 #884315
22,41 #884315
21,42 #884315
22,42 #884315
21,43 #884315
22,43 #884315
44,43 #884315
21,44 #884315
22,44 #884315
44,44 #884315
21,45 #884315
22,45 #884315
44,45 #884315
22,46 #884315
23,46 #884315
44,46 #884315
22,47 #884315
23,47 #884315
44,47 #884315
22,48 #884315
23,48 #884315
24,48 #884315
44,48 #884315
45,48 #884315
44,49 #884315
45,49 #884315
44,50 #884315
45,50 #884315

## Frame 8 - changes from frame 7

210 pixels change. Set each to the listed colour, grouped by colour (key a #c5cded = clear back to background):
#### #c5cded (key a - BACKGROUND/clear) - 51 px
8,25 #c5cded
9,25 #c5cded
10,25 #c5cded
11,25 #c5cded
12,25 #c5cded
13,25 #c5cded
14,25 #c5cded
15,25 #c5cded
16,25 #c5cded
4,26 #c5cded
5,26 #c5cded
6,26 #c5cded
7,26 #c5cded
17,26 #c5cded
3,27 #c5cded
2,28 #c5cded
18,35 #c5cded
19,38 #c5cded
19,39 #c5cded
19,40 #c5cded
39,40 #c5cded
39,41 #c5cded
20,42 #c5cded
45,42 #c5cded
46,42 #c5cded
20,43 #c5cded
25,43 #c5cded
26,43 #c5cded
40,43 #c5cded
45,43 #c5cded
46,43 #c5cded
20,44 #c5cded
25,44 #c5cded
26,44 #c5cded
40,44 #c5cded
45,44 #c5cded
46,44 #c5cded
20,45 #c5cded
26,45 #c5cded
40,45 #c5cded
46,45 #c5cded
26,46 #c5cded
46,46 #c5cded
26,47 #c5cded
46,47 #c5cded
27,50 #c5cded
47,50 #c5cded
25,51 #c5cded
26,51 #c5cded
45,51 #c5cded
46,51 #c5cded
#### #c4550c (key b) - 17 px
8,31 #c4550c
9,31 #c4550c
10,31 #c4550c
11,31 #c4550c
12,31 #c4550c
13,31 #c4550c
14,31 #c4550c
15,31 #c4550c
16,31 #c4550c
21,35 #c4550c
22,38 #c4550c
22,39 #c4550c
22,40 #c4550c
21,41 #c4550c
22,41 #c4550c
42,42 #c4550c
43,42 #c4550c
#### #3a2518 (key c) - 83 px
8,26 #3a2518
9,26 #3a2518
10,26 #3a2518
11,26 #3a2518
12,26 #3a2518
13,26 #3a2518
14,26 #3a2518
15,26 #3a2518
16,26 #3a2518
4,27 #3a2518
5,27 #3a2518
6,27 #3a2518
7,27 #3a2518
17,27 #3a2518
3,28 #3a2518
2,31 #3a2518
3,32 #3a2518
5,33 #3a2518
16,33 #3a2518
6,34 #3a2518
7,34 #3a2518
8,34 #3a2518
9,34 #3a2518
10,34 #3a2518
11,34 #3a2518
12,34 #3a2518
13,34 #3a2518
14,34 #3a2518
15,34 #3a2518
17,34 #3a2518
19,35 #3a2518
22,35 #3a2518
20,38 #3a2518
23,38 #3a2518
20,39 #3a2518
20,40 #3a2518
23,40 #3a2518
40,40 #3a2518
40,41 #3a2518
21,42 #3a2518
24,42 #3a2518
41,42 #3a2518
44,42 #3a2518
21,43 #3a2518
24,43 #3a2518
41,43 #3a2518
44,43 #3a2518
21,44 #3a2518
24,44 #3a2518
41,44 #3a2518
44,44 #3a2518
21,45 #3a2518
22,45 #3a2518
25,45 #3a2518
41,45 #3a2518
44,45 #3a2518
45,45 #3a2518
22,46 #3a2518
25,46 #3a2518
44,46 #3a2518
45,46 #3a2518
22,47 #3a2518
25,47 #3a2518
44,47 #3a2518
45,47 #3a2518
23,48 #3a2518
44,48 #3a2518
21,49 #3a2518
27,49 #3a2518
41,49 #3a2518
44,49 #3a2518
47,49 #3a2518
21,50 #3a2518
24,50 #3a2518
25,50 #3a2518
26,50 #3a2518
41,50 #3a2518
45,50 #3a2518
46,50 #3a2518
22,51 #3a2518
23,51 #3a2518
42,51 #3a2518
43,51 #3a2518
#### #a64c10 (key d) - 10 px
16,32 #a64c10
8,33 #a64c10
9,33 #a64c10
10,33 #a64c10
11,33 #a64c10
12,33 #a64c10
13,33 #a64c10
14,33 #a64c10
15,33 #a64c10
41,41 #a64c10
#### #f5b658 (key e) - 10 px
8,28 #f5b658
9,28 #f5b658
10,28 #f5b658
11,28 #f5b658
12,28 #f5b658
13,28 #f5b658
14,28 #f5b658
15,28 #f5b658
16,28 #f5b658
17,28 #f5b658
#### #eec991 (key f) - 5 px
3,31 #eec991
4,32 #eec991
5,32 #eec991
6,33 #eec991
7,33 #eec991
#### #3a1818 (key g) - 7 px
22,48 #3a1818
45,48 #3a1818
22,49 #3a1818
45,49 #3a1818
46,49 #3a1818
22,50 #3a1818
23,50 #3a1818
#### #884315 (key h) - 27 px
23,42 #884315
23,43 #884315
42,43 #884315
43,43 #884315
23,44 #884315
42,44 #884315
43,44 #884315
23,45 #884315
24,45 #884315
42,45 #884315
43,45 #884315
24,46 #884315
42,46 #884315
43,46 #884315
24,47 #884315
42,47 #884315
43,47 #884315
25,48 #884315
42,48 #884315
43,48 #884315
24,49 #884315
25,49 #884315
26,49 #884315
42,49 #884315
43,49 #884315
42,50 #884315
43,50 #884315

## Loop check: frame 8 -> frame 1 differs by 243 px (listed for reference, frame 1 already defined)

## Full grids for checking (not needed for clicking)

Frame 1:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbffffcaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaacccccccccccccaacbbbbbfffffcaaaaaaaaaaaaa
aaaaaaaacccccccccacccccceeeeeeeeeeeeeccbbbbbfffffccaaaaaaaaaaaaa
aaaacccceeeeeeeeecccceeeeeeeeeeeeeeeeeebbbbfffffccaaaaaaaaaaaaaa
aaacffffeeeeeeeeeeceeeeeeeeeeeeeeeeeeeeeeeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddcccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccacacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddddddddddddddddddcbbccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddddddddddddddddddcbbccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbcccccccccccccccccccbbcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbccaaaaaaaaaaaaaaaccbbcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbccaaaaaaaaaaaaaaaccbbcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbccaaaaaaaaaaaaaaacbbcaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaccbbcaaaaaaaaaaaaaaacbbcaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacggchhcaaaaaaaaaaaaachhcggcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacggcchhcaaaaaaaaaaaachhccggcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacgggchhhcaaaaaaaaaaachhhcgggcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacccacccaaaaaaaaaaaaacccacccaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Frame 2:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbffffcaaaaaaaaaaaaa
aaaaaaaacccccccccaaaaaaacccccccccccccaacbbbbbfffffcaaaaaaaaaaaaa
aaaacccceeeeeeeeeccccccceeeeeeeeeeeeeccbbbbbfffffccaaaaaaaaaaaaa
aaacffffeeeeeeeeeeccceeeeeeeeeeeeeeeeeebbbbfffffccaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcceeeeeeeeeeeeeeeeeeeeeeeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddcccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccaccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcccccccccccccccccccccbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddcaaaaaaaaaaaaacddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddcaaaaaaaaaaaaacddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbcgcaaaaaaaaaaaaacddchhcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbcgcaaaaaaaaaaaaaacdchhcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacchhhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaacgcccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhhcaaaaaaaaaaaaaaacgggcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Frame 3:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaabbbbbffffcaaaaaaaaaaaaa
aaaaaaaacccccccccaaaaaaaaaaaaaaaaaaaaaaacbbbbfffffcaaaaaaaaaaaaa
aaaacccceeeeeeeeecaaaaaacccccccccccccaacbbbbfffffccaaaaaaaaaaaaa
aaacffffeeeeeeeeeecccccceeeeeeeeeeeeeccbbbbfffffccaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcccceeeeeeeeeeeeeeeeeebbeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcceeeeeeeeeeeeeeeeeeeeeebbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddccbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccaccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcbbbbbbbbbbbbbbbbbbbdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcccbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcccccccccccccccccccccacbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcacddcaaaaaaaaaaacddcacbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcacggcaaaaaaaaaaacddcaachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcacggcaaaaaaaaaacddcaachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhcacggcaaaaaaaaaaacggcachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhcacggcaaaaaaaaaaacggcachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhcacggcaaaaaaaaaaacggcachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhcaacggcaaaaaaaaaacggcaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhcaacggcaaaaaaaaaacggcaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhcaacgggcaaaaaaaaacggcaachhhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhcaaacccaaaaaaaaaacggcaaacccaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaachhhcaaaaaaaaaaaaaaacgggcaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Frame 4:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaabbbbbffffcaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbfffffcaaaaaaaaaaaaa
aaaaaaaacccccccccaaaaaaacccccccccccccaacbbbbfffffccaaaaaaaaaaaaa
aaaacccceeeeeeeeeccccccceeeeeeeeeeeeeccbbbbfffffccaaaaaaaaaaaaaa
aaacffffeeeeeeeeeeccceeeeeeeeeeeeeeeeeebbeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcceeeeeeeeeeeeeeeeeeeeeebbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddcccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccaccbbcbbbbbbbbbbbbbbbbbbbdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddccccbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcccccccccccccccccccccaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcaacddcaaaaaaaaaacddcaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcaacddcaaaaaaaaaacddcaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaacbbcaaacggcaaaaaaaaaacddcaaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhcaaaacggcaaaaaaaacggcaaaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhcaaaacggcaaaaaaaacggcaaaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhcaaaaacggcaaaaaaacggcaaaaachhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhcaaaaacggcaaaaaaacggcaaaaachhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhcaaaaacggcaaaaaaacggcaaaaachhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhcaaaaaacggcaaaaaacggcaaaaaachhcaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhcaaaaaacgggcaaaaacggcaaaaaachhhcaaaaaaaaaaaa
aaaaaaaaaaaaaaaaachhhcaaaaaacccaaaaaacgggcaaaaaacccaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Frame 5:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbffffcaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaacccccccccccccaacbbbbbfffffcaaaaaaaaaaaaa
aaaaaaaacccccccccacccccceeeeeeeeeeeeeccbbbbbfffffccaaaaaaaaaaaaa
aaaacccceeeeeeeeecccceeeeeeeeeeeeeeeeeebbbbfffffccaaaaaaaaaaaaaa
aaacffffeeeeeeeeeeceeeeeeeeeeeeeeeeeeeeeeeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddcccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccaccbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaacbbccdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaacbbccdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaacbbcacccccccccccccccccccccccbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaacbbcaaacddcaaaaaaaaacddcaaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaacbbcaaacddcaaaaaaaaacddcaaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaacbbcaaaacddcaaaaaaaaacddcaaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaacbbcaaaacddcaaaaaaaacddcaaaaacbbcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaachhcaaaaacggcaaaaaaacggcaaaaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaachhcaaaaacggcaaaaaaacggcaaaaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaachhcaaaaacggcaaaaaaacggcaaaaaachhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaachhcaaaaaacggcaaaaaacggcaaaaaachhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaachhcaaaaaacggcaaaaaacggcaaaaaachhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaachhcaaaaaaacggcaaaaacggcaaaaaaachhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaachhcaaaaaaaacggcaaaacggcaaaaaaaachhcaaaaaaaaaaaaa
aaaaaaaaaaaaaaachhhcaaaaaaacgggcaaacgggcaaaaaaachhhcaaaaaaaaaaaa
aaaaaaaaaaaaaaaacccaaaaaaaaacccaaaaacccaaaaaaaaacccaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Frame 6:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbffffcaaaaaaaaaaaaa
aaaaaaaacccccccccaaaaaaacccccccccccccaacbbbbbfffffcaaaaaaaaaaaaa
aaaacccceeeeeeeeeccccccceeeeeeeeeeeeeccbbbbbfffffccaaaaaaaaaaaaa
aaacffffeeeeeeeeeeccceeeeeeeeeeeeeeeeeebbbbfffffccaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcceeeeeeeeeeeeeeeeeeeeeeeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddcccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccaccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcccccccccccccccccccccccbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcacddcaaaaaaaaaaacddcacbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcacddcaaaaaaaaaaacddcacbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhcacddcaaaaaaaaaaacggcaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhcaacddcaaaaaaaaaacggcaacbbcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhcaacggcaaaaaaaaaacggcaachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhcaacggcaaaaaaaaaacggcaachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhcaacggcaaaaaaaaaacggcaachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhcaacggcaaaaaaaaaacggcaachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhcaacggcaaaaaaaaaacggcaachhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaachhhcaacggcaaaaaaaaacgggcaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacccaaacggcaaaaaaaaaacccaaachhcaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaacgggcaaaaaaaaaaaaaaachhhcaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Frame 7:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaabbbbbffffcaaaaaaaaaaaaa
aaaaaaaacccccccccaaaaaaaaaaaaaaaaaaaaaaacbbbbfffffcaaaaaaaaaaaaa
aaaacccceeeeeeeeecaaaaaacccccccccccccaacbbbbfffffccaaaaaaaaaaaaa
aaacffffeeeeeeeeeecccccceeeeeeeeeeeeeccbbbbfffffccaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcccceeeeeeeeeeeeeeeeeebbeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcceeeeeeeeeeeeeeeeeeeeeebbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddccbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccaccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcbbbbbbbbbbbbbbbbbbbdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaacbbcddddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddddddddddddddddddccbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcccccccccccccccccccdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcddcaaaaaaaaaaaaacddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcdcaaaaaaaaaaaaacggcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcdcaaaaaaaaaaaaaacggcbbcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcggcaaaaaaaaaaaaacggchhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcggcaaaaaaaaaaaaacggchhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaachhcggcaaaaaaaaaaaaacggchhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhhccaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaacccgcaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaacgggcaaaaaaaaaaaaaaachhhcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

Frame 8:
```
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacaaaacaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacccaacccaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgcaacgcaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacgbbccgbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbccggbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacggbbcggbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeeebbbcaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaceeeebbbbbbcaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbgbbbbcaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbbbbbbbbbbbbgcaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffffffffffcaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbffffffffffffcaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbbfffcccccccccaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaabbbbbffffcaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaacbbbbfffffcaaaaaaaaaaaaa
aaaaaaaacccccccccaaaaaaacccccccccccccaacbbbbfffffccaaaaaaaaaaaaa
aaaacccceeeeeeeeeccccccceeeeeeeeeeeeeccbbbbfffffccaaaaaaaaaaaaaa
aaacffffeeeeeeeeeeccceeeeeeeeeeeeeeeeeebbeeffffccaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcceeeeeeeeeeeeeeeeeeeeeebbfffccaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aacfffffbbbbbbbbbcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaacffffdddddddddcbbbbbbbbbbbbbbbbbbbbbbbbbffcaaaaaaaaaaaaaaaaaa
aaaaacffddddddddcccbbcbbbbbbbbbbbbbbbbbbbbcbbcaaaaaaaaaaaaaaaaaa
aaaaaaccccccccccaccbbcbbbbbbbbbbbbbbbbbbbdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddddcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbcdddddddddddddddddccbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbccccccccccccccccccdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbcdcaaaaaaaaaaaaaacdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaacbbcdcaaaaaaaaaaaaaacdcbbcaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaccbbcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhcaaaaaaaaaaaaaaaachhcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaachhcaaaaaaaaaaaaaaaachhcaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaacchhcaaaaaaaaaaaaaaachhccaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaacgchhcaaaaaaaaaaaaaachhcgcaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaacgchhhcaaaaaaaaaaaaachhcggcaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaacggcccaaaaaaaaaaaaaachhhccaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaacccaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```
