

TABLE 1 – Initial Feasible Solution (NW Corner)

Allocations (occupied cells in bold)

 A B C D Supply
F1 225    225
F2 25 390   415
F3  390 355  745
F4   135 690 825
F5    230 230
Dem 250 780 490 920 

Vacant cells & Improvements

1. Cell (1,B) – cost = 210
      Loop: (1,B)+, (1,A)–, (2,A)+, (2,B)–
      Improvement = 210 – 170 + 120 – 110 = +50
2. Cell (1,C) – cost = 215
      Loop: (1,C)+, (1,A)–, (2,A)+, (2,B)–, (3,B)+, (3,C)–
      Improvement = 215 – 170 + 120 – 110 + 140 – 150 = +45
3. Cell (1,D) – cost = 241
      Loop: (1,D)+, (1,A)–, (2,A)+, (2,B)–, (3,B)+, (3,C)–, (4,C)+, (4,D)–
      Improv = 241 – 170 + 120 – 110 + 140 – 150 + 310 – 510 = –129 ✅ most negative
4. Cell (2,C) – cost = 268
      Loop: (2,C)+, (2,B)–, (3,B)+, (3,C)–
      Improv = 268 – 110 + 140 – 150 = +148
5. Cell (2,D) – cost = 200
      Loop: (2,D)+, (2,B)–, (3,B)+, (3,C)–, (4,C)+, (4,D)–
      Improv = 200 – 110 + 140 – 150 + 310 – 510 = –120 (also negative, but –129 is more negative)
6. Cell (3,A) – cost = 130
      Loop: (3,A)+, (3,B)–, (2,B)+, (2,A)–
      Improv = 130 – 140 + 110 – 120 = –20
7. Cell (3,D) – cost = 110
      Loop: (3,D)+, (3,C)–, (4,C)+, (4,D)–
      Improv = 110 – 150 + 310 – 510 = –240 ✅ most negative (choose this)
8. Cell (4,A) – cost = 510
      Loop: (4,A)+, (4,C)–, (3,C)+, (3,B)–, (2,B)+, (2,A)–
      Improv = 510 – 310 + 150 – 140 + 110 – 120 = +200
9. Cell (4,B) – cost = 401
      Loop: (4,B)+, (4,C)–, (3,C)+, (3,B)–
      Improv = 401 – 310 + 150 – 140 = +101
10. Cell (5,A) – cost = 410
        Loop: (5,A)+, (5,D)–, (4,D)+, (4,C)–, (3,C)+, (3,B)–, (2,B)+, (2,A)–
        Improv = 410 – 610 + 510 – 310 + 150 – 140 + 110 – 120 = 0
11. Cell (5,B) – cost = 451
        Loop: (5,B)+, (5,D)–, (4,D)+, (4,C)–, (3,C)+, (3,B)–
        Improv = 451 – 610 + 510 – 310 + 150 – 140 = +51
12. Cell (5,C) – cost = 460
        Loop: (5,C)+, (5,D)–, (4,D)+, (4,C)–
        Improv = 460 – 610 + 510 – 310 = +50

Entering cell: (3,D) with improvement –240 (most negative).

---

TABLE 2 – After shifting 355 units on (3,D) loop

Allocations

 A B C D Supply
F1 225    225
F2 25 390   415
F3  390  355 745
F4   490 335 825
F5    230 230
Dem 250 780 490 920 

Vacant cells & Improvements

1. (1,B) – 210
      Loop: (1,B)+, (1,A)–, (2,A)+, (2,B)–
      Improv = 210 – 170 + 120 – 110 = +50
2. (1,C) – 215
      Loop: (1,C)+, (1,A)–, (2,A)+, (2,B)–, (3,B)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 215 – 170 + 120 – 110 + 140 – 110 + 510 – 310 = +285
3. (1,D) – 241
      Loop: (1,D)+, (1,A)–, (2,A)+, (2,B)–, (3,B)+, (3,D)–
      Improv = 241 – 170 + 120 – 110 + 140 – 110 = +111
4. (2,C) – 268
      Loop: (2,C)+, (2,B)–, (3,B)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 268 – 110 + 140 – 110 + 510 – 310 = +388
5. (2,D) – 200
      Loop: (2,D)+, (2,B)–, (3,B)+, (3,D)–
      Improv = 200 – 110 + 140 – 110 = +120
6. (3,A) – 130
      Loop: (3,A)+, (3,B)–, (2,B)+, (2,A)–
      Improv = 130 – 140 + 110 – 120 = –20
7. (3,C) – 150
      Loop: (3,C)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 150 – 110 + 510 – 310 = +240
8. (4,A) – 510
      Loop: (4,A)+, (4,C)–, (2,C)? no – better: (4,A)+, (4,D)–, (3,D)+, (3,B)–, (2,B)+, (2,A)–
      Improv = 510 – 510 + 110 – 140 + 110 – 120 = –40
9. (4,B) – 401
      Loop: (4,B)+, (4,D)–, (3,D)+, (3,B)–
      Improv = 401 – 510 + 110 – 140 = –139 ✅ most negative
10. (5,A) – 410
        Loop: (5,A)+, (5,D)–, (4,D)+, (4,C)–, (2,C)? no – simpler: (5,A)+, (5,D)–, (4,D)+, (4,C)–, (3,C)? no, need occupied: (4,C) is occupied, then (4,D) occupied, (3,D) occupied, (3,B) occupied, (2,B) occupied, (2,A) occupied.
        Actually loop: (5,A)+ → (5,D)– → (4,D)+ → (4,C)– → (3,C)? (3,C) vacant → invalid. Use (4,C) then (2,C)? (2,C) vacant. So need different path. Let's find correct loop:
        (5,A)+, (5,D)–, (4,D)+, (4,C)–, (2,C)+? (2,C) vacant. Alternative: (5,A)+, (5,D)–, (3,D)+, (3,B)–, (2,B)+, (2,A)–. Yes! That works.
        Improv = 410 – 610 + 110 – 140 + 110 – 120 = –240 ✅ most negative (tie with –139? –240 is more negative)
11. (5,B) – 451
        Loop: (5,B)+, (5,D)–, (4,D)+, (4,C)–, (2,C)+? no. Use (5,B)+, (5,D)–, (3,D)+, (3,B)–
        Improv = 451 – 610 + 110 – 140 = –189
12. (5,C) – 460
        Loop: (5,C)+, (5,D)–, (4,D)+, (4,C)–
        Improv = 460 – 610 + 510 – 310 = +50

Entering cell: (5,A) with improvement –240 (most negative).
(Note: (4,B) also negative but less magnitude.)

---

TABLE 3 – After shifting 25 units on (5,A) loop

Allocations

 A B C D Supply
F1 225    225
F2  415   415
F3  365  380 745
F4   490 335 825
F5 25   205 230
Dem 250 780 490 920 

Improvements

1. (1,B) – 210
      Loop: (1,B)+, (1,A)–, (5,A)+, (5,D)–, (3,D)+, (3,B)–
      Improv = 210 – 170 + 410 – 610 + 110 – 140 = –190 ✅ most negative
2. (1,C) – 215
      Loop: (1,C)+, (1,A)–, (5,A)+, (5,D)–, (4,D)+, (4,C)–
      Improv = 215 – 170 + 410 – 610 + 510 – 310 = +45
3. (1,D) – 241
      Loop: (1,D)+, (1,A)–, (5,A)+, (5,D)–
      Improv = 241 – 170 + 410 – 610 = –129
4. (2,A) – 120
      Loop: (2,A)+, (2,B)–, (3,B)+, (3,D)–, (5,D)+, (5,A)–
      Improv = 120 – 110 + 140 – 110 + 610 – 410 = +240
5. (2,C) – 268
      Loop: (2,C)+, (2,B)–, (3,B)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 268 – 110 + 140 – 110 + 510 – 310 = +388
6. (2,D) – 200
      Loop: (2,D)+, (2,B)–, (3,B)+, (3,D)–
      Improv = 200 – 110 + 140 – 110 = +120
7. (3,A) – 130
      Loop: (3,A)+, (3,B)–, (2,B)+, (2,A)? (2,A) vacant – no. Alternative: (3,A)+, (3,D)–, (5,D)+, (5,A)–
      Improv = 130 – 110 + 610 – 410 = +220
8. (3,C) – 150
      Loop: (3,C)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 150 – 110 + 510 – 310 = +240
9. (4,A) – 510
      Loop: (4,A)+, (4,C)–, (2,C)? no. (4,A)+, (4,D)–, (5,D)+, (5,A)–
      Improv = 510 – 510 + 610 – 410 = +200
10. (4,B) – 401
        Loop: (4,B)+, (4,D)–, (3,D)+, (3,B)–
        Improv = 401 – 510 + 110 – 140 = –139
11. (5,B) – 451
        Loop: (5,B)+, (5,D)–, (3,D)+, (3,B)–
        Improv = 451 – 610 + 110 – 140 = –189
12. (5,C) – 460
        Loop: (5,C)+, (5,D)–, (4,D)+, (4,C)–
        Improv = 460 – 610 + 510 – 310 = +50

Entering cell: (1,B) with improvement –190.

---

TABLE 4 – After shifting 205 units on (1,B) loop

Allocations

 A B C D Supply
F1 20 205   225
F2  415   415
F3  160  585 745
F4   490 335 825
F5 230    230
Dem 250 780 490 920 

Improvements

1. (1,C) – 215
      Loop: (1,C)+, (1,A)–, (5,A)+, (5,D)? (5,D) vacant – no. Use (1,C)+, (1,B)–, (2,B)+, (2,A)? vacant. Better: (1,C)+, (1,B)–, (3,B)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 215 – 210 + 140 – 110 + 510 – 310 = +235
2. (1,D) – 241
      Loop: (1,D)+, (1,B)–, (3,B)+, (3,D)–
      Improv = 241 – 210 + 140 – 110 = +61
3. (2,A) – 120
      Loop: (2,A)+, (2,B)–, (3,B)+, (3,D)–, (4,D)+, (4,C)–, (1,C)+? no. Simpler: (2,A)+, (2,B)–, (1,B)+, (1,A)–
      Improv = 120 – 110 + 210 – 170 = +50
4. (2,C) – 268
      Loop: (2,C)+, (2,B)–, (3,B)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 268 – 110 + 140 – 110 + 510 – 310 = +388
5. (2,D) – 200
      Loop: (2,D)+, (2,B)–, (3,B)+, (3,D)–
      Improv = 200 – 110 + 140 – 110 = +120
6. (3,A) – 130
      Loop: (3,A)+, (3,B)–, (1,B)+, (1,A)–
      Improv = 130 – 140 + 210 – 170 = +30
7. (3,C) – 150
      Loop: (3,C)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 150 – 110 + 510 – 310 = +240
8. (4,A) – 510
      Loop: (4,A)+, (4,C)–, (1,C)? no. (4,A)+, (4,D)–, (3,D)+, (3,B)–, (1,B)+, (1,A)–
      Improv = 510 – 510 + 110 – 140 + 210 – 170 = +10
9. (4,B) – 401
      Loop: (4,B)+, (4,D)–, (3,D)+, (3,B)–
      Improv = 401 – 510 + 110 – 140 = –139 ✅ most negative
10. (5,B) – 451
        Loop: (5,B)+, (5,A)–, (1,A)+, (1,B)–
        Improv = 451 – 410 + 170 – 210 = +1
11. (5,C) – 460
        Loop: (5,C)+, (5,A)–, (1,A)+, (1,B)–, (3,B)+, (3,D)–, (4,D)+, (4,C)–
        Improv = 460 – 410 + 170 – 210 + 140 – 110 + 510 – 310 = +240
12. (5,D) – 610
        Loop: (5,D)+, (5,A)–, (1,A)+, (1,B)–, (3,B)+, (3,D)–
        Improv = 610 – 410 + 170 – 210 + 140 – 110 = +190

Entering cell: (4,B) with improvement –139.

---

TABLE 5 – After shifting 160 units on (4,B) loop

Allocations

 A B C D Supply
F1 20 205   225
F2  415   415
F3    745 745
F4  160 490 175 825
F5 230    230
Dem 250 780 490 920 

Improvements

1. (1,C) – 215
      Loop: (1,C)+, (1,B)–, (4,B)+, (4,C)–
      Improv = 215 – 210 + 401 – 310 = +96
2. (1,D) – 241
      Loop: (1,D)+, (1,B)–, (4,B)+, (4,D)–
      Improv = 241 – 210 + 401 – 510 = –78 ✅ most negative
3. (2,A) – 120
      Loop: (2,A)+, (2,B)–, (1,B)+, (1,A)–
      Improv = 120 – 110 + 210 – 170 = +50
4. (2,C) – 268
      Loop: (2,C)+, (2,B)–, (4,B)+, (4,C)–
      Improv = 268 – 110 + 401 – 310 = +249
5. (2,D) – 200
      Loop: (2,D)+, (2,B)–, (4,B)+, (4,D)–
      Improv = 200 – 110 + 401 – 510 = –19
6. (3,A) – 130
      Loop: (3,A)+, (3,D)–, (4,D)+, (4,B)–, (1,B)+, (1,A)–
      Improv = 130 – 110 + 510 – 401 + 210 – 170 = +169
7. (3,B) – 140
      Loop: (3,B)+, (3,D)–, (4,D)+, (4,B)–
      Improv = 140 – 110 + 510 – 401 = +139
8. (3,C) – 150
      Loop: (3,C)+, (3,D)–, (4,D)+, (4,C)–
      Improv = 150 – 110 + 510 – 310 = +240
9. (4,A) – 510
      Loop: (4,A)+, (4,B)–, (1,B)+, (1,A)–
      Improv = 510 – 401 + 210 – 170 = +149
10. (5,B) – 451
        Loop: (5,B)+, (5,A)–, (1,A)+, (1,B)–
        Improv = 451 – 410 + 170 – 210 = +1
11. (5,C) – 460
        Loop: (5,C)+, (5,A)–, (1,A)+, (1,B)–, (4,B)+, (4,C)–
        Improv = 460 – 410 + 170 – 210 + 401 – 310 = +101
12. (5,D) – 610
        Loop: (5,D)+, (5,A)–, (1,A)+, (1,B)–, (4,B)+, (4,D)–
        Improv = 610 – 410 + 170 – 210 + 401 – 510 = +51

Entering cell: (1,D) with improvement –78.

---

TABLE 6 – After shifting 175 units on (1,D) loop

Allocations

 A B C D Supply
F1 20 30  175 225
F2  415   415
F3    745 745
F4  335 490  825
F5 230    230
Dem 250 780 490 920 

Improvements (check optimality)

1. (1,C) – 215
      Loop: (1,C)+, (1,B)–, (4,B)+, (4,C)–
      Improv = 215 – 210 + 401 – 310 = +96
2. (2,A) – 120
      Loop: (2,A)+, (2,B)–, (1,B)+, (1,A)–
      Improv = 120 – 110 + 210 – 170 = +50
3. (2,C) – 268
      Loop: (2,C)+, (2,B)–, (4,B)+, (4,C)–
      Improv = 268 – 110 + 401 – 310 = +249
4. (2,D) – 200
      Loop: (2,D)+, (2,B)–, (4,B)+, (4,D)? (4,D) vacant – need different: (2,D)+, (2,B)–, (1,B)+, (1,D)–
      Improv = 200 – 110 + 210 – 241 = +59
5. (3,A) – 130
      Loop: (3,A)+, (3,D)–, (1,D)+, (1,A)–
      Improv = 130 – 110 + 241 – 170 = +91
6. (3,B) – 140
      Loop: (3,B)+, (3,D)–, (1,D)+, (1,B)–
      Improv = 140 – 110 + 241 – 210 = +61
7. (3,C) – 150
      Loop: (3,C)+, (3,D)–, (1,D)+, (1,B)–, (4,B)+, (4,C)–
      Improv = 150 – 110 + 241 – 210 + 401 – 310 = +162
8. (4,A) – 510
      Loop: (4,A)+, (4,B)–, (1,B)+, (1,A)–
      Improv = 510 – 401 + 210 – 170 = +149
9. (4,D) – 510
      Loop: (4,D)+, (4,B)–, (1,B)+, (1,D)–
      Improv = 510 – 401 + 210 – 241 = +78
10. (5,B) – 451
        Loop: (5,B)+, (5,A)–, (1,A)+, (1,B)–
        Improv = 451 – 410 + 170 – 210 = +1
11. (5,C) – 460
        Loop: (5,C)+, (5,A)–, (1,A)+, (1,B)–, (4,B)+, (4,C)–
        Improv = 460 – 410 + 170 – 210 + 401 – 310 = +101
12. (5,D) – 610
        Loop: (5,D)+, (5,A)–, (1,A)+, (1,D)–
        Improv = 610 – 410 + 170 – 241 = +129

All improvements are ≥ 0.
✅ Optimal solution reached.

---

Summary of minimum cost

Iteration Table Entering Cell Improvement New Cost
Initial 1 – – 726,050
1 2 (3,D) –240 –240 640,850
2 3 (5,A) –240 –240 634,850
3 4 (1,B) –190 –190 595,900
4 5 (4,B) –139 –139 573,660
5 6 (1,D) –78 –78 560,010
6 (final) 7 (no negatives) – 560,010

Final minimum cost = 560,010