# Hamiltonian Cycle Project (Combinatorical Optimization course project)

## Project Description

This project aims to solve the **Traveling Salesman Problem (TSP)** using real-world geographical locations, such as churches. The goal is to find a **Hamiltonian cycle** for a given graph, which represents a complete tour of all the locations, visiting each location exactly once and returning to the starting point.

We use the **osmnx** package [[1], [2]] to get the locations of the churches. This package allows us to retrieve, model, analyze, and visualize street networks from OpenStreetMap.

## Problem Statement

The Traveling Salesman Problem is a classic algorithmic problem in the field of computer science and operations research. It focuses on optimization. In this problem, a salesman is given a list of cities and must determine the shortest route that allows him to visit each city once and return to his original location.

In our case, we are trying to find a Hamiltonian cycle in a graph where nodes represent geographical locations (e.g., churches) and edges represent the paths between them. A Hamiltonian cycle is a closed loop on a graph where every node (vertex) is visited exactly once.

## Methodology

There are various algorithmic strategies and heuristics to solve this problem. Here is an overview of the algorithms that are available to get Hamiltonian cycles:

1. **Brute Force Method**: This method involves generating all permutations of the vertices and checking each permutation for a Hamiltonian cycle. This method is simple but not efficient for large graphs.

2. **Backtracking Algorithm**: This method involves creating a path and backtracking whenever the path doesn't lead to a solution. It is more efficient than the brute force method.

3. **Greedy Algorithm**: This method involves making the choice that seems best at the moment. It doesn't always lead to the optimal solution but it's efficient for large graphs.

4. **Dynamic Programming**: This method involves breaking down the problem into smaller subproblems and solving each one only once.

5. **Genetic Algorithm**: This method involves using techniques inspired by evolutionary biology such as mutation, crossover, and selection.

in this project the algorithm that is going t

## Installation and Usage

To use this project, you need to have Docker installed on your machine. You can run the project directly from the official OSMnx Docker image [[3]]. To run the Docker image, use the following command:

```bash
docker run --rm -it --name osmnx -p 8888:8888 -v "$PWD":/home/jovyan/work gboeing/osmnx
```

**Note:** As the Docker image is somewhat large (> 3Gb) it may fail downloading sometimes because of an instable connection, for that the only solution is just trying again the command. 

## References

[[1]]: OSMnx: Python for Street Networks. Retrieved from https://osmnx.readthedocs.io/ 

[[2]]: Boeing, G. 2017. “OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks.” Computers, Environment and Urban Systems. 65, 126-139. doi:10.1016/j.compenvurbsys.2017.05.004 

[[3]]: OSMnx Docker Image. Retrieved from https://hub.docker.com/r/gboeing/osmnx : Docker Installation Guide. Retrieved from https://docs.docker.com/get-docker/ 
