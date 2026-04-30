
# Battleship Game Guide (Java Project)

# How to Play

# Objective
The goal of Battleship is to sink all of the enemy ships before they sink yours.

---

# Game Modes

# Player vs Computer (AIGame)
- You choose a preset ship layout
- The computer randomly places its ships
- You take turns attacking coordinates
- First to sink all enemy ships wins

---

# Player vs Player (GameDriver)
- Both players use the same board setup
- Players take turns entering coordinates
- First player to sink all ships wins

---

# How to Enter Moves

You attack using grid coordinates:

A1, B5, J10


# Format:
- Letter (A–J) = Column
- Number (1–10) = Row

Example:

B3 → Column B, Row 3

---

# Game Feedback

When you attack, you will see:

- **Hit!** → You hit part of a ship
- **Miss!** → No ship at that location
- **Hit and sunk!** → You destroyed an entire ship
- **Already attacked!** → You picked that spot before
- **Out of bounds!** → Invalid coordinate
---
## Winning the Game

You win when: All enemy ships are destroyed
The game will display: You win!

```

---

# 🧩 Class Overview

---

## 📦 Board
Handles the game grid and core logic.

### Responsibilities:
- Stores the 10x10 grid
- Tracks ship positions
- Handles attacks
- Checks win condition
- Prints the board

---

## 🚢 Ship
Represents a single ship on the board.

### Responsibilities:
- Stores size and position
- Tracks hits
- Determines if ship is sunk
- Checks if a coordinate is part of the ship

---

## ⚙️ ShipLogic
Base class for Ship.

### Responsibilities:
- Stores starting position
- Provides shared ship data structure

---

## 👤 HumanPlayer
Handles player input.

### Responsibilities:
- Reads user input (A1–J10)
- Converts input into coordinates
- Validates moves

---

## 🤖 AIPlayer
Controls computer moves.

### Responsibilities:
- Generates random attacks
- Avoids repeating moves

---

## 🧱 PresetBoards
Creates predefined ship layouts.

### Responsibilities:
- Loads ships into the board
- Provides multiple difficulty/layout options

---

## 🎮 AIGame
Main driver for Player vs Computer mode.

### Responsibilities:
- Runs full game loop
- Alternates player and AI turns
- Displays results and win condition

---

## 🎮 GameDriver
Main driver for Player vs Player mode.

### Responsibilities:
- Runs PvP game loop
- Handles player input turns
- Checks win condition

---

# 🧠 Summary

This project demonstrates:
- Object-oriented programming
- 2D array grid systems
- Input validation
- Game loop design
- Turn-based mechanics

---
```

---

If you want, I can also:

* turn this into a **PDF formatted report**
* or make a **short 1-page submission version for class**
* or help you add **diagrams of the board + ship placement**
