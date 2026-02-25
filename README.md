# 🔴 Pro Checkers AI

A modern, responsive, single-file Checkers game built with **HTML5**, **Tailwind CSS**, and **Vanilla JavaScript**. Play against a friend locally or challenge a custom-built **Minimax AI** with three difficulty levels.

![Checkers Preview](https://img.shields.io/badge/Game-Checkers-red)
![AI-Powered](https://img.shields.io/badge/AI-Minimax-blue)
![Tech](https://img.shields.io/badge/Tech-TailwindCSS-06B6D4)

## ✨ Features

-   **Smart AI**: Features a Minimax algorithm with **Alpha-Beta Pruning** for efficient move calculation.
-   **3 Difficulty Levels**:
    *   **Easy**: AI looks 1 move ahead (plays mostly randomly).
    *   **Medium**: AI looks 3 moves ahead (balanced play).
    *   **Hard**: AI looks 5 moves ahead (strategic and defensive).
-   **Modern UI**: Built with Tailwind CSS, featuring smooth transitions, piece animations, and a glassmorphism aesthetic.
-   **Zero Dependencies**: Everything is contained in a single HTML file. No installation or local server required.
-   **Mobile Friendly**: Responsive design that works on phones, tablets, and desktops.

## 🕹️ How to Play

1.  **Run the Game**: Simply open the `checkers.html` file in any modern web browser (Chrome, Firefox, Safari, Edge).
2.  **Select Mode**: Use the dropdown menu to choose between "Player vs Player" or one of the AI levels.
3.  **Moving**: Click a piece to select it. Valid moves will be highlighted with a pulsing golden dot. Click the dot to move.
4.  **The Goal**: Capture all of your opponent's pieces or trap them so they have no legal moves left.

## 📏 Game Rules

This version uses a specific rule set tailored for casual play:

-   **Movement**: Standard pieces move diagonally forward one square.
-   **Jumps**: Jumps are **NOT mandatory**. You may choose to capture an opponent's piece or take a different strategic move.
-   **Multi-Jumps**: If you choose to capture and that piece is capable of another jump immediately after, you **must** complete the jump sequence.
-   **Kings**: Reaching the furthest row promotes your piece to a King (♔). Kings can move and jump both forward and backward.
-   **Winning**: A player wins when the opponent has no pieces left or cannot make any legal moves.

## 🧠 Technical Overview

### The AI (Minimax)
The AI simulates thousands of possible future board states to determine the best move. 
-   **Heuristics**: The AI evaluates the board based on piece count, King count, and board positioning (valuing the center and forward advancement).
-   **Optimization**: It uses **Alpha-Beta Pruning** to "cut off" branches of the move tree that are guaranteed to be worse than previously explored options, allowing it to look deeper into the future without slowing down.

### Performance
The game uses a 1D array representation of the 8x8 board for high-speed calculations during the AI's recursive search.

## 🛠️ Built With

-   **HTML5/CSS3**
-   **Tailwind CSS** (via CDN)
-   **Vanilla JavaScript** (ES6+)
