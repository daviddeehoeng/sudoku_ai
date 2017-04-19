## Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: We use constraint propagation to solve the naked twins problem since we use the naked twins to exclude the possibilities or options in the other units within the same naked twins's units. Constraint propagation is defined as using local constraints, such as the naked twins, to reduce the possibilities of the other unit spaces. In the sudoku project, two boxes within the same unit had the values 2 and 3. By knowing this, we could eliminate the values 2 and 3 from the other boxes within the same unit as the naked twins since we knew for a fact that 2 and 3 could not be values for the boxes. 

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: As mentioned in the above answer, constraint propagation utilizes constraints to determine and reduce the possibilities of other sudoku squares. For example, in one diagonal, we could have definite answers of 1, 3, 5, and 6. The remaining units in that diagonal are unknown. However, we're able to deduce that the remaining unknown units are not 1, 3, 5, or 6 because those numbers are already known values for the definite units. As a result, we can start our processing with the possible values for the five unknown units--2, 4, 7, 8, and 9.

### Install

This project requires **Python 3**.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. 

(http://www.pygame.org/download.shtml).

### Code

* `solution.py`
* `solution_test.py`
* `PySudoku.py`
* `visualize.py`

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py
