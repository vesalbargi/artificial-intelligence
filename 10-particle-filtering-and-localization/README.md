# Particle Filtering and Location Tracking

## Overview

This assignment explores **particle filtering**, a probabilistic technique for estimating the location of a moving individual when observations are noisy and the true position is unknown.

Using simulated movement and sensor-distance measurements, the notebook implements a particle filter from basic utility functions. It estimates the individual's position over time and evaluates the predictions against ground-truth data.

## Objectives

* Understand particle filtering for sequential state estimation.
* Model movement using stochastic particle transitions.
* Calculate particle-to-sensor distances and observation likelihoods.
* Normalize particle weights and perform weighted resampling.
* Evaluate localization accuracy and uncertainty over time.
* Investigate how the movement parameter affects prediction quality.

## Implementation

### 1. Particle Movement

Particles represent possible locations of the individual. At each time step, each particle moves in a randomly selected direction, with its travel distance sampled from an exponential distribution. The movement parameter is updated using the scaling factor \(k\), and particle positions are constrained to the allowed coordinate range.

### 2. Sensor Measurements and Weighting

The notebook calculates Euclidean distances between particles and sensors. Gaussian probability density functions model the likelihood of the observed distances, accounting for sensor-specific error means and standard deviations.

The sensor likelihoods are combined to calculate a normalized weight for each particle. Particles that better explain the observations receive higher weights.

### 3. Resampling and Position Estimation

Weighted resampling selects particles for the next iteration, favoring those with higher observation likelihoods. The estimated position is calculated as the weighted mean of particle coordinates, while coordinate-wise standard deviations provide an indication of uncertainty.

### 4. Performance Evaluation

The estimated trajectory is compared with the ground-truth locations. The notebook examines:

* Mean absolute position error over time.
* Particle-position standard deviations along the X and Y axes.
* The estimated trajectory compared with the true trajectory.
* The influence of different movement scaling factors on prediction accuracy.

## Visualizations

The notebook produces plots showing estimation error, particle spread, and the estimated and ground-truth trajectories. Together, these visualizations help assess tracking accuracy and uncertainty throughout the simulation.

## Key Takeaways

* Particle filtering represents uncertainty through a collection of weighted candidate states.
* Sensor observations update the relative plausibility of each particle.
* Resampling focuses computation on more likely locations but can reduce particle diversity.
* Prediction quality depends on the movement model, sensor noise, particle initialization, and particle count.
* The movement scaling factor \(k\) should be selected based on how well it reflects the underlying motion and performs against validation data.
