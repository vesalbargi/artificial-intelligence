# Artificial Intelligence

This repository contains a collection of artificial intelligence and machine learning assignments implemented in Python using Jupyter Notebooks. The assignments explore optimization, search algorithms, game theory, probabilistic reasoning, and reinforcement learning through practical implementations and experiments.

## Repository Structure

| # | Assignment | Description |
|---|---|---|
| 01 | Linear Programming and Optimization | Solving linear optimization problems using the corner point method and exploring online advertising allocation. |
| 02 | Multi-Armed Bandits | Implementing and comparing exploration strategies, including Epsilon-Greedy, UCB, Thompson Sampling, and optimistic initialization. |
| 03 | Sliding Puzzle Search | Implementing BFS, DFS, Uniform Cost Search, Iterative Deepening, and A* for the 8-puzzle problem. |
| 04 | Constraint Satisfaction and Search | Exploring Hill Climbing, Simulated Annealing, Genetic Algorithms, Min-Conflicts, Beam Search, and Backtracking. |
| 05 | Adversarial Game Search | Implementing Minimax, Alpha-Beta Pruning, and Expectimax for a Connect-style game. |
| 06 | Game Theory and Nash Equilibrium | Analyzing strategic games, iterated elimination of dominated strategies, best responses, and mixed-strategy Nash equilibria. |
| 07 | Markov Decision Processes and Reinforcement Learning | Implementing policy iteration and value iteration, including experiments with the Gambler’s Problem. |
| 08 | Q-Learning for MountainCar | Applying tabular Q-learning to the MountainCar environment and analyzing learned policies and state values. |
| 09 | Bayesian Networks and Probabilistic Inference | Modeling dependencies between variables and performing inference for fraud detection using variable elimination. |
| 10 | Particle Filtering and Localization | Implementing a particle filter to estimate location from movement and sensor observations. |
| 11 | Linear Regression and Gradient Descent | Implementing linear regression, gradient descent, learning-rate comparisons, and the Normal Equation. |
| 12 | Approximate Reinforcement Learning | Comparing approximate Q-learning, SARSA, and Expected SARSA using linear and radial basis function features. |

Each assignment is stored in its own numbered folder. Supporting datasets and other required files are kept alongside the corresponding notebooks.

## Technologies Used

- **Python** — primary programming language.
- **Jupyter Notebook** — interactive development, experimentation, and visualization.
- **NumPy** — numerical computations and array operations.
- **pandas** — loading and processing tabular data.
- **Matplotlib** — plotting results, learning curves, and state-value visualizations.
- **SciPy** — probability distributions and statistical calculations.
- **Gymnasium** — reinforcement learning environments, including MountainCar.
- **scikit-learn** — feature scaling and radial basis function feature generation.

Not every assignment requires every library. The required dependencies depend on the notebook being used.

## Getting Started

### Requirements

Install Python and Jupyter Notebook or JupyterLab. Python dependencies used across the repository include NumPy, pandas, Matplotlib, SciPy, Gymnasium, and scikit-learn.

### Installation

Clone the repository

```bash
git clone https://github.com/vesalbargi/artificial-intelligence.git
```

Create a Python virtual environment

```bash
python -m venv .venv
```

Activate the virtual environment

- On Windows:

  ```bash
  .venv\Scripts\Activate.ps1
  ```

- On macOS/Linux:

  ```bash
  source .venv/bin/activate
  ```

Install required packages

```bash
pip install notebook numpy pandas matplotlib scipy gymnasium scikit-learn
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the desired assignment folder and run its notebook. Make sure any required datasets or supporting files are kept in the locations expected by the notebook.

## Learning Objectives

Through these assignments, the repository explores:

- Formulating and solving optimization problems.
- Understanding search strategies and heuristic evaluation.
- Modeling constraint satisfaction problems.
- Developing adversarial decision-making algorithms.
- Analyzing strategic interactions and Nash equilibria.
- Modeling sequential decisions using Markov decision processes.
- Implementing reinforcement learning algorithms and function approximation.
- Performing probabilistic inference with Bayesian networks.
- Estimating hidden states using particle filtering.
- Training and evaluating regression models using numerical optimization.

## License

This project is licensed under the MIT License.

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)