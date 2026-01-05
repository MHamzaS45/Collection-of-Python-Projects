# 💣 Minesweeper Board Generator (Python)

**Minesweeper Board Generator** is a Python console application that creates valid Minesweeper-style boards using deterministic randomization.
It focuses on **board generation logic**, **neighbor mine calculation**, and **simple persistence**, rather than gameplay interaction.

This project serves as a practical exercise in **2D arrays**, **randomized placement**, and **clean procedural design**.

---

## 🧩 Project Overview

The program allows users to generate a minesweeper board of arbitrary size and mine count, display it in the console, and save it to a file for later use.

Each board:

* Uses `9` to represent a mine
* Uses numbers `0–8` to represent the count of adjacent mines
* Is generated deterministically using a fixed random seed

---

## ⚙️ Features

* **Custom board dimensions**
  Choose any number of rows and columns.

* **Configurable mine count**
  Validated to prevent impossible configurations.

* **Accurate neighbor calculation**
  Each non-mine cell correctly reflects surrounding mines.

* **Deterministic randomness**
  A fixed seed (`random.seed(1234)`) ensures reproducible boards.

* **Board persistence**
  Save generated boards as plain-text files for inspection or reuse.

---

## 🧠 Core Concepts

This project demonstrates:

* **2D list (matrix) manipulation**
* **Randomized but controlled placement**
* **Boundary-safe neighbor scanning**
* **Separation of responsibilities**
  (generation, printing, saving)
* **Menu-driven CLI design**

---

## 📁 Output Format

Saved boards are written as comma-separated rows:

```
0,1,9,1,0
1,2,2,1,0
9,1,0,0,0
```

Where:

* `9` = mine
* `0–8` = number of adjacent mines

---

## ▶️ How to Run

1. Ensure **Python 3** is installed.
2. Run the script:

   ```bash
   python main.py
   ```
3. Use the menu to:

   * Generate a board
   * Display it
   * Save it to a file

---

## 🛑 Input Validation

The program safely handles:

* Non-numeric input
* Negative values
* Excessive mine counts
* Attempts to print or save before generation

---

## 🧪 Design Notes

* Mines are laid **before** calculating nearby values.
* Neighbor scanning includes all eight surrounding directions.
* The board is stored internally as a mutable 2D list passed between functions.
* The random seed ensures identical boards for identical inputs—useful for testing and debugging.

---

## 📌 Purpose

This is a **learning-focused project**, created to practice:

* Algorithmic thinking
* Matrix traversal
* Defensive input handling
* File I/O
* Clean procedural Python design

It can serve as a foundation for a full Minesweeper game, solver, or GUI-based extension.

---

Happy mining—carefully. 💥🟦
