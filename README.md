# mathematical-optimisation-project
implementation of the model in the paper:
https://www.sciencedirect.com/science/article/pii/S0377221721010432?via%3Dihub

[Project_Oil-test+plot.ipynb](https://github.com/dsancin/mathematical-optimisation-project/blob/main/Project_Oil-test%2Bplot.ipynb) contains the solution of an example case using gurobi.

[Project_Oil analisi dimensionale.ipynb](https://github.com/dsancin/mathematical-optimisation-project/blob/main/Project_Oil%20analisi%20dimensionale.ipynb) Runs multiple instance of various dimensions using gurobi.

[time_gurobi.txt](https://github.com/dsancin/mathematical-optimisation-project/blob/main/time_gurobi.txt) contains the results of the dimensional analysis, the column oreder is: number of collection points, number of source points, runtime (manually limited to 3 hours) and percentage gap between lower and upper bounds (inf means that no solutions were found).

[Project_Oil VNS.ipynb](https://github.com/dsancin/mathematical-optimisation-project/blob/main/Project_Oil%20VNS.ipynb) contains an attempt at implementing a Variable Neighborhood Search for solving the problem. implented the Constructive Heuristic and a simplified VNS. example solution (same case as the gurobi test), a final solution is reached but it is not the best optimal solution due to how the algorithm is implemented. Once there is only one route the program stops because it can only modify the routes (almost all operation requires at least two routes) and not create them. Dimensional analysis was run on this code increasing manually n_CC and n_SP and increasing the maximum route length constraint to 3600 in the VNS algorithm for n_CC 40 to 80, for n_CC 100 it had to be increased to 5000 (in the CH it's left at 1800).


