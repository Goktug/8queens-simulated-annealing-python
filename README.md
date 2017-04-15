# Solving 8-Queens problem using Simulated Annealing method

The process involves::

1. Randomly **move** or alter the **state** 
2. Assess the **energy** of the new state using an objective function
3. Compare the energy to the previous state and 
   decide whether to accept the new solution or
   reject it based on the current **temperature**.
4. Repeat until you have converged on an acceptable answer


For a move to be accepted, it must meet one of two requirements

* The move causes a decrease in state energy (i.e. an improvement in the objective function)
* The move increases the state energy (i.e. a slightly worse solution) but is within the bounds of the temperature. The temperature exponetially decreases as the algorithm progresses. In this way, we avoid getting trapped by local minima early in the process but start to hone in on a viable solution by the end. 
