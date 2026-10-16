# My Tic-Tac-Toe AI Project

For my CodSoft internship task, I built a Tic-Tac-Toe game where a person can play against an AI. I wanted the game to be simple to start, so everything is included in one HTML file. You do not need to install anything.

## How to play

1. Open `index.html` in a modern web browser.
2. Play as **X** by clicking an empty square.
3. The AI responds as **O**.
4. Choose **New game** when you are ready for another round.

The game keeps track of wins and draws while the page stays open. It also highlights the winning squares at the end of a round.

## How I made the AI choose a move

I used the **Minimax algorithm**. For each available move, the AI looks ahead at the moves that could follow and scores the result. A win for the AI gets a positive score, a human win gets a negative score, and a draw gets zero. The AI chooses the move with the best score. It also favors winning sooner and postponing a loss.

To make the search more efficient, I added **alpha-beta pruning**. This lets the AI skip parts of the search when they cannot change which move is best. The final decision stays the same.

Tic-Tac-Toe is small enough for the AI to search all the way to the end of each game. That makes it unbeatable when it plays correctly. A player can still force a draw by also playing well.

## Project files

- `index.html` contains the game, its styling, and the AI code.
- `README.md` explains how to play and how the algorithm works.
- `Project_Report.pdf` is a short report for my project submission.

## What I learned

This project helped me understand how a search algorithm can compare possible future moves, and how alpha-beta pruning can make that search more efficient. I also practiced connecting the AI logic to an interactive game interface.
