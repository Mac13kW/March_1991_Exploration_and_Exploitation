# March_1991_Exploration_and_Exploitation
This is a recreation of the computational model from March JG. 1991. Exploration and Exploitation in Organizational Learning, Organization Science. 2(1):71-87. The model has been recreated without access to the original code. The purpose of the exercise was to assess the ease of reproducing the original results using only the notes from the paper.

The code has been reproduced in R, using R Studio Version 1.0.136 (Windows 10).

The code reproduces Figure 1. but to a different scaling (does not reach the 0.95 value). This is a well known problem with that model - it is relatively easy to reproduce the code, but difficult to reproduce the figures. Doing requires making additional assumptions that cannot be found in the paper itself.


_Technical notes:_

Interestingly, the original code cannot be followed exactly as described in the paper. The text says that the simulation runs until it reaches a steady state, i.e., "at which all individuals and the code share the same (not necesarilly accurate) beliefe with respect to each dimension" p. 75 However, because individuals don't learn when code is 0 and the code only learns  from superior individuals (page 74), it is possible that such equilibrium will never be reached. Consider reality R[-1, 1, -1, 1], C[0, 1, 1, 1], and all Individuals are I[1, 1, 1, 1]. No further learning is possible and there will be no convergence in beliefs between the individuals and the code
