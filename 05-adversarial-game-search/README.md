# Adversarial Game Search

This assignment explores **adversarial search algorithms** by implementing AI players for a Connect-style game played on a 6 × 10 board. Players take turns dropping pieces into columns, aiming to connect five consecutive pieces horizontally, vertically, or diagonally.

## Part 1: Minimax Search

Implement the **Minimax algorithm** to select moves by exploring possible game states to a search depth of four.

**Key concepts:**

* Maximizing and minimizing player decisions.
* Recursive game-tree exploration.
* Evaluating board positions with a scoring function.
* Detecting terminal states and winning configurations.

## Part 2: Alpha–Beta Pruning

Enhance Minimax with **alpha–beta pruning** to reduce the number of game-tree branches explored without changing the optimal result of the search.

**Key concepts:**

* Alpha and beta bounds.
* Pruning branches that cannot improve the current decision.
* Improving search efficiency.

## Part 3: Expectimax Search

Implement **Expectimax** to model an opponent whose moves are chosen randomly. The algorithm evaluates chance nodes using the expected scores of possible opponent moves.

**Key concepts:**

* Maximizing decisions for the AI player.
* Chance nodes representing random opponent behavior.
* Expected utility across possible outcomes.
* Differences between adversarial and probabilistic decision-making.

## Learning Outcomes

* Implement game-tree search for a two-player game.
* Compare Minimax, alpha–beta pruning, and Expectimax.
* Understand the role of evaluation functions and search depth.
* Model both strategic opponents and random behavior.
