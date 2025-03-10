# 5.Noughts_and_Crosses_with_Alpha-Beta_Pruning__202401100400138
This is a Python implementation of the classic Tic-Tac-Toe (also known as Noughts and Crosses) game where the AI (Player O) plays optimally using the Minimax algorithm and Alpha-Beta Pruning. The game allows a human player (Player X) to compete against an AI that uses game theory to decide the best moves.

Problem Statement:
The goal of this project is to develop an AI for the Tic-Tac-Toe game that plays optimally. The game is played on a 3x3 grid, and the objective is to get three of your marks (either 'X' or 'O') in a row, either horizontally, vertically, or diagonally.

In this implementation:

Player X is the human player.
Player O is controlled by the AI.
The AI uses the Minimax algorithm combined with Alpha-Beta Pruning to make optimal decisions in order to either win the game or force a draw. The AI tries to minimize the human player's chances of winning while maximizing its own chances.

Solution Overview:
This project implements a command-line version of the Tic-Tac-Toe game where the AI (Player O) plays optimally against a human player (Player X). The main components of the solution include:

Minimax Algorithm:

The Minimax algorithm recursively evaluates all possible moves to determine the best one. It assigns scores to possible board states and selects the move that maximizes the AI's chances of winning while minimizing the human player's chances.
Alpha-Beta Pruning:

Alpha-Beta Pruning is an optimization technique used to prune branches of the game tree that do not need to be explored further. This makes the algorithm more efficient by reducing the number of nodes evaluated.
Game Loop:

The game alternates between the AI (Player O) and the human player (Player X) until one of them wins or the board is full (a draw).
Evaluation Criteria:

The AI evaluates the board using scores:
+10 for a win by AI.
-10 for a win by the human.
0 for a draw.
