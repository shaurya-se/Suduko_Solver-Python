# Suduko_Solver-Python
A Python script designed to both solve and generate Sudoku puzzles. It utilizes the Backtracking algorithm to efficiently find solutions. Feel free to customize and improve the script as needed!

## Demo
```
>>> import SudokuMaster

>>> board = SudokuMaster.makeBoard()
>>> SudokuMaster.printBoard(board)
>>>
[4, 5, 1, 7, 3, 8, 6, 9, 2]
[2, 6, 9, 4, 5, 1, 3, 8, 7]
[7, 3, 8, 2, 6, 9, 5, 1, 4]
[5, 9, 2, 3, 1, 4, 8, 7, 6]
[3, 1, 4, 6, 8, 7, 9, 2, 5]
[6, 8, 7, 5, 9, 2, 1, 4, 3]
[8, 4, 3, 9, 7, 6, 2, 5, 1]
[1, 2, 5, 8, 4, 3, 7, 6, 9]
[9, 7, 6, 1, 2, 5, 4, 3, 8]

>>> puzzle = SudokuMaster.makePuzzleBoard(board, "moderate")
>>> # Difficulty levels: "easy", "moderate", "difficult"
>>> SudokuMaster.printBoard(puzzle)
>>>
[0, 0, 0, 0, 0, 0, 0, 0, 2]
[0, 6, 9, 4, 0, 1, 0, 8, 0]
[0, 0, 0, 2, 6, 0, 5, 0, 0]
[5, 0, 0, 0, 0, 0, 8, 7, 6]
[0, 1, 0, 6, 8, 7, 0, 0, 0]
[0, 0, 0, 0, 9, 2, 0, 4, 3]
[8, 0, 3, 0, 0, 6, 2, 5, 0]
[0, 0, 0, 8, 4, 3, 0, 6, 0]
[0, 7, 6, 1, 2, 0, 4, 0, 0]

>>> if SudokuMaster.solveBoard(puzzle):
        print("\n\n\nSolved Solution is: ")
        SudokuMaster.printBoard(puzzle)
    else:
        print("No Solution Exists")

Solved Solution is: 
[4, 5, 1, 7, 3, 8, 6, 9, 2]
[2, 6, 9, 4, 5, 1, 3, 8, 7]
[7, 3, 8, 2, 6, 9, 5, 1, 4]
[5, 9, 2, 3, 1, 4, 8, 7, 6]
[3, 1, 4, 6, 8, 7, 9, 2, 5]
[6, 8, 7, 5, 9, 2, 1, 4, 3]
[8, 4, 3, 9, 7, 6, 2, 5, 1]
[1, 2, 5, 8, 4, 3, 7, 6, 9]
[9, 7, 6, 1, 2, 5, 4, 3, 8]

>>> newBoardToSolve = [
    [0, 0, 0, 0, 0, 0, 0, 0, 0],
    [0, 8, 3, 0, 4, 2, 0, 1, 6],
    [2, 4, 0, 0, 7, 6, 3, 0, 0],
    [4, 5, 2, 0, 0, 7, 0, 8, 0],
    [0, 3, 9, 2, 0, 4, 1, 0, 0],
    [0, 7, 0, 9, 3, 0, 0, 0, 4],
    [7, 1, 6, 0, 0, 3, 2, 0, 0],
    [3, 0, 0, 4, 2, 5, 0, 7, 0],
    [5, 0, 4, 0, 6, 0, 0, 0, 9]
]

>>> if SudokuMaster.solveBoard(newBoardToSolve):
        print("\n\n\nSolved Solution is: ")
        SudokuMaster.printBoard(newBoardToSolve)
    else:
        print("No Solution Exists")

Solved Solution is: 
[1, 6, 7, 3, 8, 9, 4, 5, 2]
[9, 8, 3, 5, 4, 2, 7, 1, 6]
[2, 4, 5, 1, 7, 6, 3, 9, 8]
[4, 5, 2, 6, 1, 7, 9, 8, 3]
[8, 3, 9, 2, 5, 4, 1, 6, 7]
[6, 7, 1, 9, 3, 8, 5, 2, 4]
[7, 1, 6, 8, 9, 3, 2, 4, 5]
[3, 9, 8, 4, 2, 5, 6, 7, 1]
[5, 2, 4, 7, 6, 1, 8, 3, 9]
```
