## Wolf Hunt Search Algorithm (WHSA): Harnessing the Social and Hunting Strategies of Wolves for Optimization
The Wolf Hunt Search Algorithm (WHSA) stands as a fascinating testament to the ingenuity of applying natural phenomena to solve complex human problems, particularly in the realm of computational optimization.

# Wolf packs Hunting scene
https://youtu.be/OgE2sRFd4gs?si=od-h9i83HWak452I

Inspired by the intricate social structure and cooperative hunting strategies of wolves in the wild, WHSA translates these behaviors into a computational framework that tackles optimization tasks with remarkable efficiency and adaptability. This essay explores the foundational principles of WHSA, its operational mechanisms, applications, strengths, and potential areas for future exploration.

!["Wolf Hunting Strategy"](https://github.com/lamthienphuc/Wolf-Hunt-Search-Algorithm/blob/main/Screenshot%202024-03-18%20160046.png)

# Operational Mechanisms of WHSA
The operational framework of WHSA is grounded in the simulation of wolf pack dynamics, where individual wolves (agents) search through a multidimensional space to locate the optimal solution (prey). The algorithm is initiated with a population of wolves randomly scattered in the search space. These agents then move towards the best solution based on their social hierarchy, including alpha (the leader), beta (the second in command), and omega (the lowest-ranking wolves).

# General outline:
Initialize: Define the population size, search space boundaries, and fitness function.

Random Initialization: Create a population of wolves (candidate solutions) with random positions within the search space.

Evaluate Fitness: Calculate the fitness score for each wolf using the fitness function.

Identify Alpha, Beta, and Omega: Find the three wolves with the best fitness values (Alpha - highest, Beta - second highest, Omega - third highest).

Encircling Prey: For each wolf (except Alpha, Beta, and Omega):
Calculate the distance between the current wolf and Alpha, Beta, or Omega (whichever is closest).
Update the position of the current wolf by moving closer to the chosen wolf.

Attacking Prey: Randomly modify the step size used for encircling to simulate the attacking behavior.

Escape from Prey: If a wolf's position goes beyond the search space boundaries, randomly re-position it within the boundaries.

Update Positions: Update the positions of all wolves based on the encircling and attacking calculations.

Evaluate New Fitness: Calculate the fitness score for each wolf after the position update.

Repeat: Go back to step 4 and continue iterating until a stopping criteria (e.g., maximum iterations reached) is met.

Return: Return the Alpha wolf (solution with the best fitness value found).


