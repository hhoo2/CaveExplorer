# GameCaveExplorer Read Me

## Introduction

Welcome to GameCaveExplorer, a text-based adventure game where you explore a mysterious cave, collect resources, and try to reach the exit. This README file provides information on how to use and understand the code in the GameCaveExplorer package.

## Package Overview

The GameCaveExplorer package includes Java classes that make up a simple text-based adventure game. Here's an overview of the key components:

- `GameMain.java`: The main class that runs the game loop and handles user input.
- `Map.java`: Represents the game map and provides methods to interact with it.
- `CaveExplorer.java`: Manages the player's actions, inventory, and game state.
- `Direction.java`: An enum representing cardinal directions (NORTH, SOUTH, EAST, WEST).
- `Status.java`: An enum representing cell statuses (e.g., PIT, WATER).

## Getting Started

Before you run the game, make sure you have Java installed on your system. You can compile and run the `GameMain.java` file to start the game. Here's a brief overview of the main components:

### Game Map

There are two predefined maps in the `GameMain` class: `MAP1` and `lARGE`. These maps are represented as arrays of strings, where each character represents a cell in the cave:

- `#`: Wall
- ` ` (space): Empty space
- `X`: Exit
- `D`: The player's starting position
- `W`: Water
- `P`: Pit
- `M`: Matches
- `F`: Food
- `K`: Jacket
- `J`: Jump Rope

You can add your own maps or modify existing ones.

### Gameplay

The game loop in the `main` method allows you to interact with the cave. Here are some key commands you can use:

- `l`: Look in a direction (e.g., `l e` to look east).
- `m`: Move in a direction (e.g., `m s` to move south).
- `j`: Jump in a direction (e.g., `j n` to jump north).
- `e`: Eat food if available.
- `c`: Check your inventory and resources.
- `r`: Rest to regain energy.
- `p`: Pick up items from your current cell.

### Debugging

There are two boolean variables, `printMap` and `useSeed`, that you can set to `true` for debugging purposes:

- `printMap`: Print the game map after each turn.
- `useSeed`: Use a specific random seed (set `seed` variable) for consistent random behavior.

### Winning and Losing

You win the game by reaching the exit (`X`) before running out of time or energy. If you fall into a pit (`P`) or water (`W`) without a jacket, you lose the game. Pay attention to your resources and plan your moves carefully.

## Additional Notes

- This game is text-based, so follow the prompts in the console to make choices.
- Make sure to enter valid commands and directions to avoid errors.
- You can customize the game by creating your own maps or adding new game elements.
- Feel free to explore and modify the code to add more features or improve the game.

Have fun exploring the cave and good luck on your adventure!
