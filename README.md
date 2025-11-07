

# Title: problem definition
The Traveling Salesman Problem (TSP) is a classic combinatorial optimization problem that seeks the shortest possible route visiting a set of locations exactly once and returning to the starting point.
 It is formally defined as finding the shortest closed path that visits each vertex in a graph exactly once, where the graph is typically undirected and weighted, with vertices representing cities and edge weights representing distances or costs.
 The problem is NP-hard, meaning no known polynomial-time algorithm can solve all instances optimally, and the number of possible routes grows factorially with the number of cities, making brute-force solutions impractical for large instances

 # Solution implementation
 The solution is rappresented as a vector of the places ordered as the order of visit of each point. The selection is based on an elitist approach.
 During each generation each individual can be a mutation of a random parent (exploitation) or a crossover between two parents (exploration).
 During early generation exploration is more utilized, gradually switching to using mostly exploitation.

 ## Mutation
 The solution rappresentation stores the phenotypic trait in the edge of the elements, so a mutation that minimizes a change in that characteristic is chosen. The algorithm used is the inversion mutation.

 ## Crossover
 Similarly for the mutation process in the crossover algorithm chosen is the inver over that minimizes the change in edges.