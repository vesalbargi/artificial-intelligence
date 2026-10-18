# Bayesian Networks and Probabilistic Inference

## Overview

This assignment explores **Bayesian networks** as a way to represent probabilistic relationships between variables and reason under uncertainty. Using a credit-card fraud scenario, it builds a directed graphical model, defines conditional probability tables, and calculates fraud probabilities given different observations.

The notebook also investigates how new evidence changes a prediction and how related observations influence the inferred probability of fraud.

## Objectives

* Represent dependencies between binary variables using a directed acyclic graph (DAG).
* Define prior probabilities and conditional probability tables (CPTs).
* Apply the law of total probability to calculate prior probabilities.
* Perform probabilistic inference using variable elimination and evidence.
* Analyze how additional observations affect the posterior probability of fraud.

## Bayesian Network Structure

The model contains six binary variables:

* **OC:** Owns a computer, tablet, or smartphone.
* **Fraud:** Indicates whether the current transaction is fraudulent.
* **Trav:** Indicates whether the cardholder is traveling.
* **FP:** Indicates whether the purchase is foreign.
* **IP:** Indicates whether the purchase is online.
* **CRP:** Indicates whether a computer-related purchase occurred during the previous week.

The network represents dependencies through the following directed edges:

* `Trav → Fraud`
* `Trav → FP`
* `Fraud → FP`
* `Fraud → IP`
* `OC → IP`
* `OC → CRP`

The graph and probability tables together define the joint probability distribution used for inference.

## Conditional Probability Tables

The assignment specifies prior probabilities for travel and device ownership, along with conditional probabilities for fraud, foreign purchases, internet purchases, and recent computer-related purchases.

These tables describe how the probability of each variable depends on its parent variables in the network.

## Probabilistic Inference

### 1. Prior Probability of Fraud

Calculate the overall probability of fraud by marginalizing over whether the cardholder is traveling. Using the provided probabilities, the prior probability is **0.43%**.

### 2. Inference from Transaction Evidence

Estimate the probability of fraud given evidence that the transaction is foreign, is not an internet purchase, and follows a recent computer-related purchase.

The calculation uses the network's joint factorization, incorporates the observed evidence, sums over hidden variables, and normalizes the results.

### 3. Updating Beliefs with New Evidence

Recalculate the posterior probability when the cardholder is known to be traveling. This illustrates how evidence can change the interpretation of a foreign transaction and affect the inferred likelihood of fraud.

### 4. Evidence and Fraud Suspicion

Explore how a recent computer-related purchase changes the inferred relationship between device ownership and an internet transaction. This section demonstrates how observations can influence predictions through dependencies in the network.

## Key Takeaways

* Bayesian networks provide a compact representation of conditional dependencies.
* Conditional probability tables define the quantitative relationships in the model.
* Variable elimination supports inference by summing over unobserved variables.
* Posterior probabilities change as new evidence becomes available.
* The interpretation of evidence depends on the relationships encoded in the network.
