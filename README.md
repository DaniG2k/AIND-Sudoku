# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?

A: If there are two values of length 2, we know that those values must exist in the two boxes, so it is safe to eliminate them from the peers. The implication here is that any other box cannot contain the values present in the twins, as the twins are locked to one of two values. This constraint helps eliminate potential values from other boxes, reducing the number of checks we have to make to solve the sudoku.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?

A: We create two new units along the sudoku board's diagonals. The implication here is that we have an additional two units of values from 1 to 9, which would constrain the board's potential values as we solve the sudoku. While adding units increases the number of checks (or iterations), it also increases the number of value constraints on the board, because we know that each diagonal must contain the values from 1 to 9.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.