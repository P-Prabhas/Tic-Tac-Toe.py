# Tic-Tac-Toe 


An unbeatable, command-line Tic-Tac-Toe game featuring an AI opponent powered by the **Minimax Algorithm** optimized with **Alpha-Beta Pruning**. Built strictly in Python with no external dependencies.

##  Features

- **Unbeatable AI:** The computer evaluates all future states to guarantee a win or a draw.
- **Alpha-Beta Pruning:** Optimizes search depth by skipping unpromising board branches, reducing processing time to fractions of a millisecond.
- **Depth-Weighted Scoring:** AI prioritizes the fastest route to victory and delays its losses as long as possible.
- **Dynamic Play:** When faced with multiple equally perfect moves, the AI picks one at random to keep gameplay varied.

##  How It Works
This project implements fundamental game theory and adversarial search concepts:

1. **Minimax Matrix:** The AI plays as the *Maximizer* (assigning positive value to wins) and assumes the human plays perfectly as the *Minimizer* (assigning negative value to AI losses).
2. **Alpha-Beta Cutoffs:** Two bounds, `alpha` (the maximum score the maximizer is assured of) and `beta` (the minimum score the minimizer is assured of), track game states. If a branch is found to be mathematically worse than a previously explored path, it is pruned immediately.

##  Prerequisites

To run this game, you only need Python 3 installed on your system. 

```bash
python --version
```

##  Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com
cd tic-tac-toe-ai
```

### 2. Run the Game
Execute the script directly from your terminal:
```bash
python tictactoe.py
```

##  How to Play

1. Choose whether you want to move first (`y/n`).
2. The board grid maps exactly to the numbers **1 through 9** on your keyboard:

```text
 1 | 2 | 3 
---+---+---
 4 | 5 | 6 
---+---+---
 7 | 8 | 9 
```

3. Type a position number and press `Enter` to make your move.

##  File Structure

```text
├── README.md          # Project documentation
└── tictactoe.py       # Core game loop and Minimax algorithm
```

##  License

Distributed under the MIT License. See `LICENSE` for more information.
