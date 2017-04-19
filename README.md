# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: We use constraint propagation to solve the naked twins problem since we use the naked twins to exclude the possibilities or options in the other units within the same naked twins's units. Constraint propagation is defined as using local constraints, such as the naked twins, to reduce the possibilities of the other unit spaces. In the sudoku project, two boxes within the same unit had the values 2 and 3. By knowing this, we could eliminate the values 2 and 3 from the other boxes within the same unit as the naked twins since we knew for a fact that 2 and 3 could not be values for the boxes. 

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: As mentioned in the above answer, constraint propagation utilizes constraints to determine and reduce the possibilities of other sudoku squares. For example, in one diagonal, we could have definite answers of 1, 3, 5, and 6. The remaining units in that diagonal are unknown. However, we're able to deduce that the remaining unknown units are not 1, 3, 5, or 6 because those numbers are already known values for the definite units. As a result, we can start our processing with the possible values for the five unknown units--2, 4, 7, 8, and 9.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solution.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Submission
Before submitting your solution to a reviewer, you are required to submit your project to Udacity's Project Assistant, which will provide some initial feedback.  

The setup is simple.  If you have not installed the client tool already, then you may do so with the command `pip install udacity-pa`.  

To submit your code to the project assistant, run `udacity submit` from within the top-level directory of this project.  You will be prompted for a username and password.  If you login using google or facebook, visit [this link](https://project-assistant.udacity.com/auth_tokens/jwt_login for alternate login instructions.

This process will create a zipfile in your top-level directory named sudoku-<id>.zip.  This is the file that you should submit to the Udacity reviews system.

