# Sudoku Solver

This is a simple Sudoku Solver built using **HTML**, **CSS**, and **JavaScript**. The solver allows users to input a partially filled Sudoku puzzle, and it will automatically solve the puzzle for them.

## Features
- Interactive grid where users can input Sudoku values.
- Automatically solves the puzzle by applying a backtracking algorithm.
- Displays the solution or an error message if no solution exists.
- Responsive design that works well on both desktop and mobile devices.

## Project Structure
```
/sudoku-solver
├── index.html         # HTML file containing the structure of the page.
├── style.css          # CSS file to style the page and the Sudoku grid.
└── script.js          # JavaScript file to handle Sudoku logic and solving algorithm.
```

## Getting Started

To get started with the Sudoku Solver, follow these steps:

### 1. Download or Clone the Repository
You can download the project files or clone the repository:

```
git clone https://github.com/yourusername/sudoku-solver.git
```

### 2. Open the `index.html` File
Open the `index.html` file in your web browser. The application will load, displaying the Sudoku grid and the solver interface.

### 3. Input Puzzle
- In the Sudoku grid, enter the numbers you know into the cells. Empty cells should be left blank.
- You can click on any cell and type a number between 1 and 9 to fill in a number.

### 4. Solve the Puzzle
- After entering your Sudoku puzzle, click the **Solve** button.
- The puzzle will be solved using a backtracking algorithm, and the solution will be displayed in the grid.

### 5. Reset the Puzzle
- You can reset the puzzle by clicking the **Reset** button. This will clear all the numbers you entered and restore the grid to its initial empty state.

## Backtracking Algorithm
The Sudoku solver uses a **backtracking algorithm** to find the solution. It tries filling in numbers one by one in empty cells, and backtracks if a number does not lead to a valid solution. The process continues until the entire grid is filled correctly or it determines that the puzzle is unsolvable.

### Backtracking Steps:
1. Find an empty cell in the grid.
2. Try all numbers from 1 to 9 in the empty cell, checking if each number is valid.
3. If the number is valid, place it in the cell and move to the next empty cell.
4. If the puzzle is completely filled, the solution is found.
5. If a number doesn't work, backtrack by removing the last placed number and trying the next one.

## Dependencies
This project does not rely on any external libraries or frameworks. All the logic is written using **plain JavaScript**, **HTML**, and **CSS**.

## Usage Example

1. Open the browser and load the `index.html` file.
2. Enter the Sudoku puzzle (numbers from 1 to 9) into the grid.
3. Click **Solve** to get the solution.

## Example Input Grid
```
5 _ _ | _ _ _ | _ _ 8
_ _ _ | _ 3 _ | _ _ _
_ 1 _ | _ _ _ | 5 _ _
------+-------+------
_ _ 2 | 1 _ _ | _ _ 7
_ _ _ | _ _ _ | _ _ _
8 _ _ | _ _ 5 | 2 _ _
------+-------+------
_ _ 5 | _ _ _ | _ 1 _
_ _ _ | _ 7 _ | _ _ _
3 _ _ | _ _ _ | _ _ 9
```

### Example Output Grid
```
5 9 3 | 6 2 7 | 1 4 8
4 7 8 | 9 3 1 | 6 5 2
2 1 6 | 8 4 9 | 5 7 3
------+-------+------
9 5 2 | 1 6 8 | 4 3 7
6 8 7 | 4 9 3 | 9 2 5
8 4 1 | 2 5 7 | 2 9 6
------+-------+------
7 3 5 | 6 1 4 | 8 9 2
1 2 9 | 5 7 6 | 3 8 4
3 6 4 | 7 8 2 | 9 5 1
```

## Technologies Used
- **HTML**: Provides the structure for the Sudoku grid and the user interface.
- **CSS**: Styles the Sudoku grid and layout, making it visually appealing and user-friendly.
- **JavaScript**: Implements the logic for solving the Sudoku puzzle using a backtracking algorithm.

## Features to Implement (Future Enhancements)
- Input validation (to ensure users only input numbers between 1-9).
- Check for invalid Sudoku puzzles (those that cannot be solved).
- Option to choose different puzzle difficulty levels.
- Timer to track how long it takes to solve the puzzle.
- Highlighting for wrong entries or clues.
- Provide a "Hint" button to suggest a number for an empty cell.

## Credits
This project was created by [Your Name]. The backtracking algorithm was inspired by traditional Sudoku-solving methods.

## License
This project is open-source and available under the MIT License. Feel free to modify, distribute, and contribute!

---

Enjoy solving Sudoku!
