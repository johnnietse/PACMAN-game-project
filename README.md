# Pac-Man Game

This project is a simple Pac-Man-style game. It involves Pac-Man navigating through a maze, collecting dots while avoiding ghosts. The project demonstrates fundamental C++ programming concepts, including file handling, arrays, and game mechanics such as collision detection and AI behavior.

## Features

- Pac-Man: Collect dots while navigating a 2D map.
- Ghosts: Two ghosts that track Pac-Man, attempting to catch him.
- Win/Loss Conditions: The game ends when Pac-Man collects all dots (win) or is caught by a ghost (loss).
- Randomized Ghost Movements: Ghosts either move randomly or towards Pac-Man if they have a clear sightline.
- Custom Map: The game map is read from a text file (map.txt), which defines the layout of walls, dots, and empty spaces.



## Game Controls
- Use W to move Pac-Man up.
- Use A to move Pac-Man left.
- Use S to move Pac-Man down.
- Use D to move Pac-Man right.


## Map File
The game reads the map layout from a file named map.txt. The map must be a 9x9 grid, surrounded by walls. Each character in the file represents a part of the game environment:

- P: Pac-Man
- G: Ghost
- .: Dot
- W: Wall
- ' ': Empty space


## Code Overview
- apsc143project.cpp: Main game logic including Pac-Man's movement, ghost behavior, win/loss conditions, and map printing.
- colours.cpp and colours.h: Placeholder files for additional features such as colorized output (optional for customization).
- CMakeLists.txt: CMake configuration for building the project.

## Key Functions
- importMap(): Loads the game map from map.txt.
- gameplay(): Main loop for handling game input and logic.
- printMap(): Displays the current state of the game board.
- winCheck(): Determines if all dots have been collected.
- loseCheck(): Checks if Pac-Man has been caught by a ghost.
- ghostSearch(): Controls ghost movement, including AI for chasing Pac-Man.