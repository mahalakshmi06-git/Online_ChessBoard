# Online_ChessBoard
# Mobile-Style Chess vs AI 🎯♟️

A fully functional, lightweight digital chessboard playable directly in your web browser. Built using a modern frontend stack, it features legal move validation, mobile-friendly touch/click controls (reminiscent of mobile carrom games), a built-in Minimax AI opponent, and an interactive victory celebration!

---

## 📸 Game Interface

Below is a preview of the interactive game board running live:

<!-- REPLACE THE LINK BELOW WITH YOUR ACTUAL COLAB SCREENSHOT URL -->
![Chess Game Gameplay](https://raw.githubusercontent.com/your-username/your-repo-name/main/screenshot.png)

---

## ✨ Features

*   **🎮 True Mobile/Carrom Style Controls:** Click a piece to highlight its path, then click any highlighted square to instantly glide it into position.
*   **🤖 Built-in Minimax AI:** Play offline against a self-contained chess engine with customizable difficulty levels (Easy, Medium, Hard).
*   **🎉 Victory Celebration:** Triggers an animated screen overlay blasting confetti and ribbon emojis (`🎉🎈💥`) upon a satisfying checkmate win!
*   **⚖️ Full Chess Rules:** Automatic enforcement of turns, check indicators (`⚠️`), illegal move blocking, and automatic draw/stalemate detection.
*   **🎨 Zero Asset Dependency:** Rendered dynamically using native HTML/CSS grids and sharp Unicode glyphs—no external heavy image files required.

---

## 🛠️ Tech Stack & Dependencies

*   **HTML5 / CSS3 Grid:** For rendering the adaptive $8 \times 8$ board layouts.
*   **JavaScript (ES6):** Handles core game loops, AI decision branching, and UI bindings.
*   **[Chess.js](https://github.com/jhlywa/chess.js):** The standard rule validation library managing board states, turn tracks, and check/draw evaluations.

---

## 🚀 How to Run the Project

### Option 1: Run in Google Colab (Recommended)
1. Open a new notebook in [Google Colab](https://colab.research.google.com).
2. Create a new code cell and paste the game code prefixed with the `%%html` magic command.
3. Click **Run Cell** (Play button) to render the board natively inside your workspace.

### Option 2: Local Deployment
1. Copy the source code and save it as an `index.html` file on your computer.
2. Double-click the file to open it instantly in any modern web browser (Chrome, Edge, Safari, Firefox). No local server installation needed!

---

## 🧠 How the AI Works

The computer opponent relies on a classic **Minimax Algorithm** enhanced with **Alpha-Beta Pruning**. 
* Every piece is assigned an exact positioning value (e.g., Pawns = 100, Knights = 320, Queens = 900).
* Selecting higher difficulty settings forces the algorithm to calculate deeper recursively into the turn tree ($1$ to $3+$ plies ahead) to minimize your material advantage and simulate human strategy.

---
<img width="904" height="487" alt="Screenshot 2026-07-05 135600" src="https://github.com/user-attachments/assets/81b55a03-f882-4e8b-aae6-7dbec5ab9741" />
<img width="844" height="640" alt="Screenshot 2026-07-05 134635" src="https://github.com/user-attachments/assets/4c7d1c38-de8f-41b9-b9c7-0172f84c9d5c" />
