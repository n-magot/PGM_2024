# CMB with Mixed Do and De

Learning Causal Markov Boundaries with Mixed Observational and Experimental Data

This repository contains the code for the paper submitted to the international conference on Probabilistic Graphical Models(PGM) 2024:
Learning Causal Markov Boundaries with Mixed Observational and Experimental Data

Konstantina Lelova, Gregory F.Cooper, Sofia Triantafillou

# Overview
Our method extends the recent algorithm (FindIMB) proposed in [Triantafillou et al. (2021)](https://proceedings.mlr.press/v161/triantafillou21a.html) which is limited to categorical data to ordinal and binary outcomes, binary treatments, and mixed covariates. 

FindIMB extended algorithm uses Bayesian regression models and approximate inference for combining observational and experimental data to learn causal and interventional Markov boundaries and improve causal estimation. 

It can be applied in scenarios when we synthetically introduce into the observational data a set of confounder variables C between treatment and outcome O in three ways: 

◦ Measured confounders only
◦ Unmeasured confounders only
◦ Measured and unmeasured confounders

