 **Description**

This project is aimed at solving global logistics problem faced by many e-commerce and food delivery companies through genetic algorithms and Vehicle Routing Problem(VRP).


**Problem**

We have a warehouse from which there are n locations for goods delivery.We have k number of vehicles and we need to optimize our route in accordance with 2 conditions:-
    1) Minimization of total distance covered by the k vehicles
    2) Even travel distribution among vehicles to save overall time taken for delivery

**Experiment with maze solver**

Before diving into the main project , i designed solutions for maze and created a maze solver using DEAP library in python.
It consisted of two steps:
  1)Solution generation where i generated set of optimal solutions
  2)Evaluation for the solutions generated for the maze problem

Project flow for maze solver

I used the toolbox library and feeded 4 directions to it.Using random generator i generated 100 characters that made one individual. Similarly generated upto 100 
solutions for the problem.
After the solutions where generated , evaluated the function on weight parameter in DEAP library.Since , i need to minimize the distance from source to destination,
 a negative input was given to weight.
 After the evaluation , the solutions went through tournament selection where the healthier solutions had higher chances to be picked and also did mutation of healthier
solutions with a probability of 20% for better exploration and nagivation through solution space.
Finally the solution space was generated and passed on through multiple generations similar to the natural evolution process before obtaining the final result.
  

  
  

