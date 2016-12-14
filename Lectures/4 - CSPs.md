# CSPs (Constraint Satisfaction Problems)


CSPs are specialized for identification problems.

The example used throughout the lecture is the task of coloring the various states of Australia (with the constraint that adjacent states cannot be painted the same color from among a limited array of options).

## Real World CSPs
- Assignment Problems (e.g. who teaches what class)
- Timetabling Problems (e.g. which class is offered when and where)
- Hardware Configuration
- Factory Scheduling

## Varieties of Constraints
- **Unary Constraints**: involve a single variables
  - Example: South Australia cannot be green.
- **Binary Constraints**: involve a pair of variables
  - Example: South Australia and West Australia cannot be the same color
- **Higher-order Constraints**: involve 3 or more variables
- **Soft Constraints**: Preferences
  - Example: Red > Green
  - Bayes' nets


## Naive Search
Depth-first search is useful when all the solutions are at the bottom.

## Backtracking Search
Backtracking Search is the basic uninformed algorithm for solving CSPs

- ordering doesn't matter
  - SA = red & WA = green is same as WA = green & SA = red
- check that constraints are satisfied as you go
  - pass the goal tests as you go (traditionally, a search node may not pass a goal test but a later node will)

## Filtering
