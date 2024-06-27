# CMB with Mixed Do and De

Learning Causal Markov Boundaries with Mixed Observational and Experimental Data

This repository contains the code for the paper submitted to the international conference on Probabilistic Graphical Models (PGM) 2024:
Learning Causal Markov Boundaries with Mixed Observational and Experimental Data

Konstantina Lelova, Gregory F.Cooper, Sofia Triantafillou

## Overview
Our method extends the recent algorithm (FindIMB) proposed in [Triantafillou et al. (2021)](https://proceedings.mlr.press/v161/triantafillou21a.html) which is limited to categorical data, to ordinal and binary outcomes, binary treatments, and mixed covariates. 

FindIMB extended algorithm, uses Bayesian regression models and approximate inference for combining observational and experimental data to learn causal and interventional Markov boundaries and improve causal estimation. 

It can be applied in scenarios where we synthetically introduce a set of confounding variables, C, between treatment and outcome, O, in three ways:

* Measured confounders only
* Unmeasured confounders only
* Measured and unmeasured confounders

### Implementation

We simulate Experimental (De) and Observational (Do) data, where Do>>De in two scenarios: 

1. When an unmeasured confounder, C, exists and another measured confounder is present in the data, and when there is no unmeasured confounding variable, in the case of both binary and ordinal outcomes. In the code given, you can adjust the confounding coefficient, b4, the number of experimental data, ne, and the number of different datasets you want to test the algorithm, N_D_test.

We evaluate our methods in how well they predict the outcome in a new experimental data set with 1000 samples.

## Getting Started
### Prerequisites
This project uses several Python packages to perform probabilistic programming, Bayesian inference, and efficient array computations:

* JAX and JAX.numpy
* NumPyro
* itertools
* pandas

You can also visualize the posterior distributions of regression parameters using the ArviZ and Matplotlib packages by uncommenting the corresponding lines in the function "sample_posterior".
  
