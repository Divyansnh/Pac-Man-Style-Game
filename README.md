# Simple Game in Scala

## Overview

This project implements a simple game in Scala where a player navigates a board, collects coins, and avoids walls. The player starts at an initial position and can move around the board to collect points.

## Features

- **10x10 Board**: The game board is a 10x10 grid where each cell can be empty, a wall, or contain a coin.
- **Player Movement**: The player can move around the board from an initial position.
- **Coins**: Coins are placed at specific positions on the board and have different values.
- **Walls**: Certain positions on the board are designated as walls, which the player cannot pass through.
- **Score Tracking**: The player's score increases as they collect coins.

## Getting Started

### Prerequisites

- Scala 2.13.x or higher
- sbt (Scala Build Tool)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/simple-game-scala.git
    cd simple-game-scala
    ```

2. Compile the project using sbt:

    ```bash
    sbt compile
    ```

3. Run the game:

    ```bash
    sbt run
    ```

## Usage

### Game Initialization

The game is initialized with the following parameters:

- `wall`: A list of coordinates (tuples) where walls exist.
- `coin`: A list of coins, each defined by a position and value (a 3-tuple).
- `initialX`: The initial x position of the player.
- `initialY`: The initial y position of the player.

Example initialization:

```scala
val game = new Game(
    wall = List((0, 0), (0, 1)),
    coin = List((1, 1, 50), (2, 2, 100)),
    initialX = 0,
    initialY = 0
)
