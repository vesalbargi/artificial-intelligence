# Markov Decision Processes

This assignment explores **dynamic programming methods for decision-making under uncertainty**. It covers policy iteration for a Markov Decision Process (MDP) and compares value iteration with policy iteration in the Gambler's Problem.

## Part 1: Policy Iteration for an MDP

Implement policy iteration for a small MDP consisting of five states, two actions, state-dependent rewards, and probabilistic transitions.

**Key concepts:**

* Representing states, actions, rewards, and transition probabilities.
* Evaluating a policy using discounted future rewards.
* Improving a policy by comparing available actions.
* Detecting when the policy has converged.

## Part 2: The Gambler's Problem

Explore the Gambler's Problem, where an agent chooses how much capital to stake on a sequence of probabilistic bets, aiming to reach a target capital of 100.

**Key concepts:**

* Maximizing the probability of reaching the goal.
* Understanding how the probability of winning affects the optimal policy.
* Analyzing why optimal stakes may vary irregularly across capital levels.
* Understanding the difference between maximizing the probability of success and maximizing expected monetary profit.

## Part 3: Value Iteration and Policy Iteration

Implement both dynamic programming algorithms to calculate state values and optimal betting policies for different probabilities of winning.

**Experiments include:**

* Value iteration for winning probabilities of 0.25, 0.55, and 0.4.
* Policy iteration for a winning probability of 0.4.
* Visualizing optimal stakes across capital levels.
* Comparing the resulting value functions and policies to verify agreement between the algorithms.

## Learning Outcomes

* Understand the fundamentals of Markov Decision Processes.
* Implement policy evaluation and policy improvement.
* Apply value iteration and policy iteration to a stochastic decision problem.
* Interpret optimal policies and compare algorithmic results.
