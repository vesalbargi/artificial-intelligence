# Linear Regression and Gradient Descent

## Overview

This assignment explores **linear regression** and two approaches to finding optimal model parameters: gradient descent and the Normal Equation. It begins with a single-feature dataset and extends the implementation to a two-feature regression problem.

The notebook implements the hypothesis function, mean squared error cost function, and gradient descent algorithm, then compares optimization behavior and visualizes fitted models.

## Objectives

* Implement a vectorized linear regression hypothesis function.
* Calculate the cost function using training prediction errors.
* Optimize model parameters using gradient descent.
* Analyze how the learning rate affects convergence.
* Implement the Normal Equation and compare its results with gradient descent.
* Extend linear regression to multiple features and visualize a fitted regression plane.

## Implementation

### 1. One-Feature Linear Regression

The notebook prepares the dataset by adding an intercept column to the feature matrix. It implements the hypothesis function and cost function, then uses gradient descent to learn the intercept and slope parameters.

A cost-history plot illustrates how the optimization objective changes during training.

### 2. Learning Rate Comparison

Several learning rates are evaluated over the same number of iterations:

* `0.1`
* `0.01`
* `0.001`
* `0.0001`

The resulting plots demonstrate how the learning rate influences convergence speed and stability. The assignment identifies `0.01` as a suitable balance for the given experiment.

### 3. Normal Equation

The Normal Equation provides a direct solution for the least-squares regression parameters. The implementation uses the pseudoinverse to improve numerical robustness and compares its predictions with those produced by gradient descent.

The resulting regression lines are plotted alongside the training data.

### 4. Two-Feature Linear Regression

The notebook extends the model to two input features. It trains the model using gradient descent, tracks the cost history, and visualizes the predictions as a three-dimensional regression plane.

The final discussion explains why gradient magnitudes and parameter updates naturally decrease as gradient descent approaches a minimum of the least-squares cost function, provided the learning rate is appropriate.

## Visualizations

The notebook includes:

* A scatter plot of the original one-feature dataset.
* Cost-history plots for gradient descent and different learning rates.
* A comparison of regression lines obtained from gradient descent and the Normal Equation.
* A cost-history plot for the two-feature model.
* A three-dimensional plot of the training data and fitted regression plane.

## Key Takeaways

* Gradient descent iteratively minimizes the regression cost function.
* Learning rate selection affects both convergence speed and stability.
* The Normal Equation provides a direct least-squares solution without iterative updates.
* Both methods can produce similar fitted parameters when gradient descent converges sufficiently.
* Multiple linear regression extends the model to additional features, while feature scaling can improve optimization behavior when features have very different scales.
* For a reasonable fixed learning rate, gradient magnitudes typically shrink as the parameters approach a minimum.
