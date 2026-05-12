# Sudoku-Solver
Paired university project: Java Swing Sudoku solver using a constraint-based backtracking algorithm to solve 9x9 puzzles. Includes CSV loading, real-time solving visualisation, and performance metrics (recursion, backtracking, execution time). Demonstrates recursion, data structures, and algorithmic efficiency.

Sudoku Solver (Java Swing)

This project was developed as a paired university coursework project. It is a Java-based Sudoku solver with a graphical user interface built using Swing. The system uses a constraint-based backtracking algorithm to solve 9x9 Sudoku puzzles, with real-time visualisation and performance tracking.

Project Structure & File Overview
Main.java

Entry point of the application. Launches the GUI using SwingUtilities.invokeLater to ensure thread-safe execution of the Swing interface.

SudokuGUI.java

Handles the main graphical user interface:

Creates the application window
Sets up buttons (Solve, Load CSV, Clear)
Manages user interactions
Connects the board, solver, validator, and visualiser
Runs the solver on a separate thread for smooth UI performance
SudokuBoard.java

Represents the core 9×9 Sudoku grid:

Stores the puzzle state in a 2D array
Provides methods to get, set, and clear cells
Validates coordinates and values
Acts as the central data model for the application
SudokuSolver.java

Implements the backtracking algorithm:

Recursively attempts to solve the puzzle
Uses the validator to ensure valid moves
Tracks recursion depth and backtracking count
Supports real-time visualisation of the solving process
Outputs performance statistics (execution time, recursion calls, backtracks)
SudokuValidator.java

Ensures Sudoku rules are maintained:

Checks row constraints
Checks column constraints
Checks 3×3 subgrid constraints
Used by the solver to validate each move
Visualiser.java

Manages the GUI grid display:

Builds a 9×9 interactive Swing grid
Updates board state visually in real time
Allows user input directly into cells
Syncs GUI input with the internal board model
Adds grid styling and 3×3 box separation
SudokuLoader.java

Handles external puzzle input:

Loads Sudoku puzzles from CSV files
Parses comma-separated values into the board
Supports empty cells as zeros
Allows users to load custom puzzles dynamically
Key Features
Constraint-based backtracking solver
Real-time solving visualisation
CSV puzzle loading
Interactive GUI input
Performance metrics tracking
Technologies Used
Java
Swing (GUI)
Object-Oriented Programming
Recursive algorithms
