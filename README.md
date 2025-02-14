All formulas were taken from https://www.cs.ubc.ca/~hoos/SATLIB/benchm.html.
The formulas were tested with the Kissat SAT Solver https://github.com/arminbiere/kissat.
The processor used for most formulas is a 3,1 GHz Dual-Core Intel Core i7.

Exceptions are: DIMACS Benchmark Instances 1) gcp-large and 2) parity. 
The processor used here: Intel(R) Core(TM) i7-8700 CPU @ 3.20GHz. 

The structure for the formulas in the Uniform Random 3-SAT Folder had to be modified: 
The last lines in each cnf file have a % and 0 sign that throw an error when running KISSAT.

The parity formulas in the DIMACS Benchmark Instances had the 0 character in a new line for each clause which also lead to errors.
Example: 
p cnf 64 254
 -2 1
 0
 -3 -2
 0
...