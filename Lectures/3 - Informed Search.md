# Informed Search

## A\* Search

A\* Search combines the goal-focused drive of greedy-search with the willingness-to-explore options that powers Uniform Cost Search.

Uniform Search orders by path cost, or backward cost **g(n)**

Greedy Search orders by goal proximity or foward cost **h(n)**.

A* Search adds these together to determine cost:
`Backward Cost + Forward Cost = g(n) + h(n)`

## Admissibility

A heuristic is **admissible** if the **heuristic** (estimated) cost from each node to the goal is less than or equal to the **actual** cost to node from each goal.

A\* **tree** search is optimal when using admissible heuristics, otherwise paths that can potentially lead to optimal solutions can become too expensive to explore.

## Consistency

A heuristic is **consistent** if the **heuristic** (estimated) cost of each edge (path) is less than or equal to the **actual** cost of each edge (path) in the graph.

A\* **graph** search is optimal when using consistent heuristics, otherwise a node that can be found at a cheaper cost will not have its cheaper cost factored into the final solution.

Admissibility is a subset to consistency.
