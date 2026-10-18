# Q-Learning for MountainCar

## Overview

This assignment explores **reinforcement learning** through the MountainCar environment from Gymnasium. The goal is to train an agent to drive an underpowered car up a hill using tabular Q-learning, learning how to build momentum through trial and error.

The notebook implements state discretization, temporal-difference updates, and an epsilon-greedy action-selection strategy. It also evaluates how exploration and learning-rate choices affect the agent's performance.

## Objectives

* Understand the reward structure and continuous state space of MountainCar.
* Convert continuous position and velocity values into discrete states.
* Implement tabular Q-learning using the Bellman optimality update.
* Derive a state-value function and policy from a trained Q-table.
* Compare learning performance under different exploration settings and learning rates.

## Implementation

### 1. State Discretization

The continuous position and velocity dimensions are mapped into discrete bins using a **15 × 15 discretization**. This allows the agent to represent the environment using a finite Q-table while balancing state-space complexity and learning accuracy.

### 2. Tabular Q-Learning

The `QLearner` class maintains action-value estimates for each discrete state and available action. At every time step, it updates the selected Q-value using the immediate reward and the estimated best value of the next state.

An epsilon-greedy strategy balances exploration and exploitation, with epsilon gradually decreasing during training.

### 3. State Values and Policy

After training, the notebook derives the state-value function by taking the maximum Q-value across actions for each state. It also extracts a greedy policy and visualizes the state-value function as a three-dimensional surface.

### 4. Performance Evaluation

The notebook investigates three aspects of agent behavior:

* **Standard training:** Trains the agent over 5,000 episodes with a decreasing exploration rate.
* **Random exploration:** Evaluates performance when actions are selected randomly throughout training.
* **Learning-rate comparison:** Compares learning rates of 0.05, 0.1, 0.2, and 0.5 to examine their effects on learning performance.

## Visualizations

The notebook generates plots to analyze learning progress and the learned state values:

* `rewards.png` — average reward during standard training.
* `mountaincar_state_value_3d.png` — three-dimensional state-value surface.
* `random_rewards.png` — average reward under random exploration.
* `learning_rate_effect.png` — final average reward for different learning rates.

## Key Takeaways

* MountainCar's continuous state space can be approximated with discrete bins for tabular learning.
* Q-learning uses temporal-difference updates to improve action-value estimates without requiring a model of the environment.
* Exploration is essential, but purely random actions do not effectively exploit learned behavior.
* The learning rate influences the speed and stability of value updates.
* The state-value function and greedy policy provide complementary views of the agent's learned behavior.
