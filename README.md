# Capacited Vehicle Routing Problem variant

In this problem formulation, the demand of certain customers may exceed the capacity of a single vehicle.
We solved using three different approaches.

## Approach 1: PuLP with CBC Solver

In this approach, the VRP is formulated as a mathematical model using the PuLP library in Python. The open solver CBC is used to solve the entire model and generate optimized routes.

## Approach 2: OR-Tools Library with Warm Start in PuLP

In this approach, we leverage the OR-Tools library, which is a constraint programming toolkit, to solve the VRP problem. If necessary, the input is modified to split demands exceeding the vehicle capacity. The output generated by OR-Tools is then used as a warm start in the PuLP model to generate the final trips and routes.

## Approach 3: Iterative Capacitated Clustering and TSP

In this approach, we utilize an iterative capacitated clustering model to generate clusters for the vehicles. Within each cluster, the traveling salesman problem (TSP) formulation is used to find the minimum distance for a route. The resulting vehicle routes are then aggregated to obtain the overall solution.



