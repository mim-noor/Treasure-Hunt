# Treasure-Hunt



This C program is a Treasure Hunt Game with various features, rules, and challenges. Here's a concise yet detailed explanation of its main components:


---

1. Game Setup

The grid size is defined as 5x5 (GRID_SIZE) with hidden treasures, traps, and power-ups.

Constants are defined for game parameters:

MAX_MOVES: 20 moves per game

TREASURES: 5 treasures to collect

TRAPS: 5 traps

POWERUPS: 2 power-ups

GAME_TIME: 60-second time limit



2. Core Functions

Grid Initialization:

initializeGrid() and initializeVisibleGrid() create hidden and visible game boards.


Item Placement:

placeItems() randomly positions treasures, traps, and power-ups on the grid, avoiding occupied cells.


Grid Display:

displayGrid() prints the visible grid, showing the player's position.



3. Player and Trap Mechanics

Player Movement:

movePlayer() updates player position based on directional input (W, A, S, D), modifies game states, and handles interactions:

Treasure: Increases score by 10 points.

Trap: Decreases health by 1.

Power-Up: Adds 3 extra moves.



Dynamic Traps:

moveDynamicTraps() randomly relocates traps on the grid to keep the game unpredictable.



4. Game Flow

User Interaction:

Players enter a username and start the game by typing go.


Timed Game Loop:

The game continues until:

The player collects all treasures (win condition).

Moves are exhausted, health reaches zero, or time runs out (lose conditions).




5. Leaderboard Management

Updating Leaderboard:

updateLeaderboard() saves player names and scores.


Displaying Leaderboard:

displayLeaderboard() shows the top players.



6. Main Game Rules

Collect all treasures to win.

Avoid traps that reduce health.

Utilize power-ups to gain extra moves.

Complete the game within 60 seconds.



---

How It Works

When the game starts, the player navigates through a hidden grid, searching for treasures while avoiding traps. If all treasures are found before running out of time, moves, or health, the player wins. Otherwise, the game ends with a score summary.

This design combines strategic movement, time management, and dynamic gameplay, making it both challenging and engaging.
