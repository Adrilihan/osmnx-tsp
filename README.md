# Travelling Salesman Problem on the Road Network Graph

A simple project developed as part of [Combinatorical Optimization](https://www.ua.pt/pt/uc/4480) curriculum unit where the objective was to solve a modified **Traveling Salesman Problem (TSP)**. Classicaly this problem is solved by finding the shortest possible cycle that visits a set of locations exactly once and returns to the starting point (i.e., a Hamiltonian cycle). In this modified version, the challenge was twofold: first, to determine the shortest route that visits 8 out of a given list of 10 churches in the city of Porto; and second, to solve the problem using the real-world pedestrian road network — yielding the following result

<p align="center">
  <img 
    style="display: block; 
           margin-left: auto;
           margin-right: auto;
           width: 50%;
           height: 50%;"
    src="https://github.com/user-attachments/assets/f3244725-17ff-4169-a682-687091eac9f7" 
    alt="Modified TSP solution displayed onto the road network of OPorto">
</p>

**OSMnx** package was used to get the locations of the churches and extract the road network [^1].

## Algorithms Used

There are various algorithmic strategies and heuristics to solve the Travelling Salesman Problem (TSP), each with different trade-offs between accuracy and computational efficiency. In this project, the following approaches were evaluated:

- Local Search
- Simulated Annealing
- Branch and Bound

## Usage

To run this project, use the conda environment defined in the `environment.yml` with

```sh
conda env create -f environment.yml
```

## References

[^1]: Boeing, G. (2025). [Modeling and Analyzing Urban Networks and Amenities with OSMnx](https://doi.org/10.1111/gean.70009). Geographical Analysis, published online ahead of print. doi:10.1111/gean.70009
