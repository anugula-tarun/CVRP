
# Capacitated Vehicle Routing Problem 

This repository contains a solution for the Capacitated Vehicle Routing Problem (CVRP) implemented using two different approaches.

## Approach 1: Warm Start with OR-Tools and solving Pulp model

In this approach, the CVRP is solved by leveraging the OR-Tools solution as a warm start for the Pulp model. This combination of powerful optimization tools allows for efficient and effective solution generation.

## Approach 2: Capacitated Clustering and TSP Solver

The second approach involves applying capacitated clustering to group the problem's nodes into clusters based on capacity constraints. Then, the Traveling Salesman Problem (TSP) is solved independently within each cluster to optimize the routes.

