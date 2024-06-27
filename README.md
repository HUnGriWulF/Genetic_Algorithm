 **Description**

This project is aimed at solving global logistics problem faced by many e-commerce and food delivery companies through genetic algorithms and Vehicle Routing Problem(VRP).


**Problem**

We have a warehouse from which there are n locations for goods delivery.We have k number of vehicles and we need to optimize our route in accordance with 2  conditions:-
    1) Minimization of total distance covered by the k vehicles
    2) Even travel distribution among vehicles to save overall time taken for delivery

**Experiment with maze solver**

Before diving into the main project , i designed solutions for maze and created a maze solver using DEAP library in python.
It consisted of two steps:
  1)Solution generation where i generated set of optimal solutions
  2)Evaluation for the solutions generated for the maze problem

**Project flow for maze solver**

I used the toolbox library and feeded 4 directions to it.Using random generator i generated 100 characters that made one individual. Similarly generated upto 100 
solutions for the problem.
After the solutions where generated , evaluated the function on weight parameter in DEAP library.Since , i need to minimize the distance from source to destination,
 a negative input was given to weight.
 After the evaluation , the solutions went through tournament selection where the healthier solutions had higher chances to be picked and also did mutation of healthier
solutions with a probability of 20% for better exploration and nagivation through solution space.
Finally the solution space was generated and passed on through multiple generations similar to the natural evolution process before obtaining the final result.

**Project Summary: Solving Vehicle Routing Problem (VRP) using Genetic Algorithm**

This project aims to solve the Vehicle Routing Problem (VRP) using a Genetic Algorithm (GA). The VRP involves determining optimal routes for multiple vehicles to deliver goods to a set of locations, starting and ending at a central depot, while minimizing total distance traveled and ensuring balance among vehicles.

**Key Components:**

Problem Definition
Locations: Randomly generated points on a 2D plane, excluding the central depot.
Depot: Central starting and ending point for all vehicles.
Vehicles: A fixed number of vehicles available to service the locations.

Genetic Algorithm Setup:
Individual Representation: Each individual is represented as a permutation of location indices, where each permutation represents a potential route for the vehicles.
Fitness Function: Evaluates routes based on two objectives:
Total Distance: Minimize the total distance traveled by all vehicles.
Balance Penalty: Penalize solutions where there is significant imbalance in distances traveled among vehicles.
Genetic Operators: Includes partially matched crossover (PMX) for crossover and shuffle mutation to maintain diversity.

Execution:
Initialization: Generates an initial population of route permutations.
Evolution: Applies genetic operators (crossover and mutation) iteratively to evolve the population towards better solutions.
Selection: Tournament selection is used to select individuals for reproduction based on their fitness.
Termination: The algorithm terminates after a specified number of generations or if a convergence criterion is met.
Visualization:

Plotting Function: Visualizes the optimal routes found by the GA, showing locations as dots, the depot as a square, and routes for each vehicle.







  

  
  

