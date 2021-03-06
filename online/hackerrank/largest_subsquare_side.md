LARGEST SUB-SQUARE SIDE
=======================

As a game developer, you need to analyze the various worlds that have been
designed. Each world is modeled as a 2-dimensional square grid where each 
cell contains an integer value. 

A grid can be divided into `square`  subgrids that 
have rows and columns ≤ the number of rows and columns in the original grid.
For each subgrid, all of its elements are summed to get a `total value`
for the subgrid. A fellow analyst provides an integer and wants to know the maximum
number of rows or columns of the square subgrids such that all of the subgrids
of that size have a total value less than that integer.

As an example, a `grid` and all its subgrids are shown below:

Grid:

2 2 2
3 3 3
4 4 4

Square subgrids:

rows/columns = 1

2, 2, 2, 3, 3, 3, 4, 4, 4
maximum sum = 4

rows/columns = 2

2 2	2 2	3 3	3 3
3 3	3 3	4 4	4 4
maximum sum = 14

rows/columns = 3

2 2 2
3 3 3
4 4 4
maximum sum = 27

If the desired maximum total value k is ≥ 27, the entire grid satisfies the condition
so answer = 3. If 14 ≤ k < 27, answer = 2. If 4 ≤ k < 14, answer = 1. 
Finally, if k < 4 there is no subgrid satisfies the condition, 
so answer = 0.
