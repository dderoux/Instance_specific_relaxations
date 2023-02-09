This folder contains all of the code corresponding to the paper
Instance-specific linear relaxation of semidefinite relaxation
problems. 
The code is written in julia, using jupyter notebooks. Be warned that 
to run this code, it is necessary that you have a mosek license available.
These are free for academics and can be obtained here:
https://www.mosek.com/products/academic-licenses/

The code is organized as follows:

---------Max cut ----------------

MaxcutRelaxations.ipynb
This file contains an implementation of the semidefinite relaxation
for maxcut, its dual and the linear relaxations of them proposed in
the main paper. 

MaxcutEvaluation.ipynb
Code containing the evaluation of the linear relaxations for maxcut,
on the TBSLP graphs, the network graphs and the instances provided
by Mirka and Williamson.


The graphs provided by Mirk and Williamson are contained in the folder
ErdosRenyi. You can also find them in their Github webpage.


MaxCutLpVsEigenBoundAndSepOracle.ipynb
Code containing the function to plot figure 1, section 4
and to compute tables 4 and 5. 



------- Sparse PCA ---------------

SparsePCArelaxations.ipynb
Contains the main function to compute the sparse pca with either 
the semidefinite relaxation or the corresponding linear relaxation.

SparsePCAExplainedVariance
Contains the functions to compute the explained variance of the different
data sets taken from the RDatasets, popular datasets installed in the base of R.
This code produces figure 5.

SparsePCAEvaluation
Contains the code to for the following evaluations of the sparse PCA:
- time taken to solve the linear relaxation versus the semidefinite relaxation. (figure 2).
-time taken to find cuts using eigen vectors vs unsing an LP( figure 4).
-Quality of the iterative linear relaxation after adding eigencuts (figure 3).
-Components obtained in the synthetic experiments (table 6).
-Components obtained for the pit props data set (table 7).


------ Lovasz Theta number ----------


Contains the code to test the linear relaxation of the semidefinite 
program to compute Lovasz Theta number.

- LovasThetaFunctions.ipynb
Containts the formulation for the semidefinite program to compute the Lovasz Theta number
and its linear relaxation.

-LovasThetaFunctions
Contains the code to evaluate the linear relaxation of the semidefinite program
to compute the Lovasz Theta number.
- Erdos-renyi random graphs (Figure 6).
- Erdos-renyi random graphs with second order cone constraints (figure 7).
- 6-regular graphs (figure 8).







