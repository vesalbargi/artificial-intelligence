# Approximate Reinforcement Learning

## Overview

This assignment explores **approximate reinforcement learning** using the MountainCar environment. It implements value-based learning algorithms that estimate action values from state features instead of maintaining a separate value for every possible state.

The assignment includes a basic linear approximation approach and an improved implementation using radial basis function (RBF) features. Both notebooks investigate learning performance, state-value visualization, and comparisons between reinforcement learning algorithms.

## Objectives

* Implement approximate Q-learning for continuous state spaces.
* Compare Q-learning, SARSA, and Expected SARSA.
* Visualize the learned state-value function.
* Investigate how feature representations affect learning.
* Evaluate the effect of including acceleration-related information.
* Compare basic linear features with richer RBF-based representations.

## Notebooks

### 1. `approximate_q_learning.ipynb`

The basic implementation uses linear function approximation with position and velocity features.

It includes:

* Approximate Q-learning with epsilon-greedy action selection.
* Approximate SARSA and Expected SARSA.
* A three-dimensional state-value surface.
* Learning-curve comparisons across algorithms.
* An experiment examining an acceleration feature.

### 2. `approximate_q_learning_rbf.ipynb`

The improved implementation uses **radial basis function (RBF) features** to represent the continuous state space more flexibly. It standardizes state observations and combines multiple RBF feature mappings with different scales.

It includes:

* Feature-based approximate Q-learning.
* Approximate SARSA and Expected SARSA using the shared feature representation.
* State-value function visualization.
* Comparisons of algorithm learning curves.
* An acceleration-related state representation experiment.
* Saved plots for individual experiments and an overall comparison.

## Algorithms and Techniques

### Approximate Q-Learning

Updates action-value estimates using the maximum predicted value of the next state. This is an off-policy temporal-difference learning method.

### Approximate SARSA

Uses the next action selected by the current policy when computing the update target. This makes the learning process dependent on the agent's behavior policy.

### Approximate Expected SARSA

Uses the expected next-state action value under the epsilon-greedy policy rather than a single sampled next action.

### Feature Representation

The basic notebook uses a small set of linear features. The improved notebook uses standardized observations and multiple RBF feature mappings to capture more complex relationships between states and values.

## Visualizations

The notebooks produce learning curves, three-dimensional state-value surfaces, and comparisons of algorithm performance. The RBF notebook also saves plots for Q-learning performance, algorithm comparisons, acceleration features, and an overall summary.

## Key Takeaways

* Function approximation allows reinforcement learning to generalize across continuous states.
* The quality of the feature representation can strongly influence learning performance.
* Q-learning, SARSA, and Expected SARSA differ in how they estimate future rewards.
* RBF features can represent nonlinear value functions more flexibly than simple linear features.
* Additional features may help, but their benefit should be assessed empirically rather than assumed.
