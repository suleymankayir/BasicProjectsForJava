# Sudoku Solver

This Java program is a Sudoku solver that uses a backtracking algorithm to find a solution for a given Sudoku puzzle. The Sudoku puzzle is represented as a 9x9 grid, and the goal is to fill in the grid with numbers from 1 to 9 according to certain rules:

1. Each row must contain all numbers from 1 to 9 with no repetition.
2. Each column must contain all numbers from 1 to 9 with no repetition.
3. Each of the nine 3x3 subgrids (boxes) must contain all numbers from 1 to 9 with no repetition.

## Components:

- **Main Class (`Main`):** The main class contains the `main` method where the Sudoku puzzle is defined and printed before and after solving. It also outputs whether the puzzle is solvable or not.

- **Print Board Method (`printBoard`):** This method is responsible for printing the Sudoku board in a visually readable format, with horizontal and vertical separators to represent the 3x3 subgrids.

- **Solve Board Method (`solveBoard`):** The core backtracking algorithm is implemented in this method. It recursively attempts to fill in the Sudoku grid, making sure that the numbers chosen comply with the Sudoku rules. If a valid solution is found, the method returns `true`. If no solution is possible, it returns `false`.

- **Helper Methods (`isNumberInRow`, `isNumberInColumn`, `isNumberInBox`, `isValidPlacement`):** These methods are used by the `solveBoard` method to check if a particular number can be placed in a given row, column, or 3x3 box without violating Sudoku rules.

## How to Use:

1. Copy the code into a Java environment or a file with a `.java` extension.
2. Compile and run the program.
3. The initial Sudoku board will be displayed, followed by the solved board (if solvable) or an indication that the board is unsolvable.

Feel free to modify the initial Sudoku board in the `main` method to test the solver with different puzzles.

**Note:** This Sudoku solver uses a simple backtracking algorithm and may not be optimized for larger puzzles. It's designed for educational purposes and can be enhanced for improved performance.
