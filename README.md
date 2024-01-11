# mathematical-optimisation-project
implementation of the model in the paper:
https://www.sciencedirect.com/science/article/pii/S0377221721010432?via%3Dihub

[Project_Oil-test+plot.ipynb](https://github.com/dsancin/mathematical-optimisation-project/blob/main/Project_Oil-test%2Bplot.ipynb) contains the solution of an example case.

[Project_Oil analisi dimensionale.ipynb](https://github.com/dsancin/mathematical-optimisation-project/blob/main/Project_Oil%20analisi%20dimensionale.ipynb) Runs multiple instance of various dimensions.

[time_gurobi.txt](https://github.com/dsancin/mathematical-optimisation-project/blob/main/time_gurobi.txt) contains the results of the dimension analysis, the column oreder is: number of collection points, number of source points, runtime (manually limited to 3 hours) and percentage gap between lower and upper bounds (inf means that no solutions were found).

[Project_Oil VNS.ipynb](https://github.com/dsancin/mathematical-optimisation-project/blob/main/Project_Oil%20VNS.ipynb) contains an attempt at implementing a Variable Neighborhood Search for solving the problem. Only the constructive heuristic for the initial solution is implemented.
