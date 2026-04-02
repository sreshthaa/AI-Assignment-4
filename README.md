# AI-Assignment-4



 1.AUSTRALIA MAP COLORING (CSP)
 Brief Explanation : 
-solves the map coloring problem using Constraint Satisfaction Problem (CSP).
Each state is assigned a color such that no two neighboring states have the same color.
It uses backtracking to try different color assignments until a valid solution is found.

Input : 
-Variables: States → WA, NT, SA, Q, NSW, V, T
-Domains: Colors → {red, green, blue}
-Constraints: Adjacent states must have different colors

Output Format : 
Console : {'WA': 'red', 'NT': 'green', ...}
Graph:
Nodes → states
Edges → borders
Colors → assigned colors (no conflicts)



2.TELANGANA MAP COLORING (CSP)
Brief Explanation : 
This extends the map coloring problem to 33 Telangana districts.
Each district is treated as a variable and assigned one of four colors such that neighboring districts do not share the same color.
The CSP solver uses backtracking with constraints to find a valid coloring.

Input :
Variables: 33 districts
Domains: {red, green, blue, yellow}
Constraints: Neighboring districts must have different colors


Output Format :
Graph:
Nodes → districts
Edges → adjacency

3.SUDOKU SOLVER (CSP)
Brief Explanation : 
-solves a 9×9 Sudoku puzzle using CSP.Each cell is a variable, and constraints ensure that there's no repeated numbers in rows, no repeated numbers in columns,no repeated numbers in 3×3 subgrids.Backtracking is used to fill missing values correctly.

Input : 
Variables: Cells → A1 to I9
Domains: {1–9}
Given values: Pre-filled Sudoku grid
Constraints:
Row uniqueness
Column uniqueness
Block uniqueness


Output Format : 
5 8 3 | 9 2 1 | 6 7 4
9 4 7 | 3 6 5 | 8 2 1
1 2 6 | 8 7 4 | 3 5 9
---------------------
...
Fully solved Sudoku grid in formatted layout



4.CRYPTARITHMETIC (TWO + TWO = FOUR)
Brief Explanation : solves a cryptarithmetic puzzle using CSP.
Each letter represents a unique digit, and the equation: TWO + TWO = FOUR must hold true.
Constraints:
-Unique digits
-Correct column-wise addition
-Carry handling


Input : 
Variables: Letters → T, W, O, F, U, R
Extra Variables: Carry → C1, C2, C3
Domains:
Letters → 0–9
Carry → {0,1}


Constraints:
All letters must be different
No leading zero
Arithmetic must satisfy equation

Output : 
   734
+  734
---------
  1468

And mapping: {'T': 7, 'W': 3, 'O': 4, 'F': 1, 'U': 6, 'R': 8, ...}


