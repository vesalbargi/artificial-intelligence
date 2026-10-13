# Multi-Armed Bandits

This assignment explores the **multi-armed bandit problem**, a fundamental concept in reinforcement learning. It focuses on balancing exploration of unknown actions with exploitation of actions that have previously produced better rewards.

## Part 1: Exploration Strategies

Implement and compare different strategies for selecting actions in a Bernoulli bandit environment, where each action has an unknown probability of producing a reward.

**Implemented strategies:**

* **Random Agent:** Selects actions randomly.
* **Epsilon-Greedy:** Balances random exploration with choosing the action with the highest estimated reward.
* **UCB (Upper Confidence Bound):** Uses reward estimates and uncertainty to guide action selection.
* **Thompson Sampling:** Uses Beta distributions to sample action values and select promising actions.
* **Adaptive Epsilon-Greedy:** Gradually reduces exploration over time.
* **Optimistic Initial Values:** Encourages exploration by starting with optimistic reward estimates.

The strategies are evaluated by tracking and plotting cumulative regret over multiple trials to compare their performance.

## Part 2: Theoretical Questions

Explore the theoretical behavior of bandit algorithms and how their parameters affect decision-making.

**Topics covered:**

* Expected regret of the epsilon-greedy strategy.
* Effects of modifying exploration terms and confidence bounds in UCB.
* Influence of prior distributions and initial values on Thompson Sampling.
* Impact of changing epsilon on exploration and exploitation.
* Comparison of the long-term regret behavior of different strategies.

## References

1. Clinical Trials Research — [Thompson Sampling for Clinical Trials](https://arxiv.org/pdf/1507.08025.pdf)
2. Machine Learning Research — [Upper Confidence Bounds for Multi-Armed Bandits](https://homes.di.unimi.it/~cesabian/Pubblicazioni/ml-02.pdf)
3. Stanford University — [A Tutorial on Thompson Sampling](https://web.stanford.edu/~bvr/pubs/TS_Tutorial.pdf)
