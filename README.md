# Posterior Concentration in Sparse Sequence Models

This project reproduces the main posterior concentration results in Castillo & van der Vaart (2012), *Needles and Straw in a Haystack: Posterior Concentration for Possibly Sparse Sequences*.

## Overview

We implement the hierarchical Bayesian model proposed in the original paper and investigate its behavior through simulations.

The project includes:
- implementation of posterior functionals (posterior mean and median)  
- simulation studies illustrating posterior concentration behavior  
- empirical comparison with empirical Bayes methods  

## Key Observations

Consistent with the theoretical results in the original paper:

- Posterior median exhibits thresholding behavior, while posterior mean provides a continuous shrinkage estimator
- Prior choices on model dimension affect estimator sparsity and false discovery  
- Heavy-tailed priors, e.g. Laplace, perform better than Gaussian priors especially in strong signal regimes  
- Fully Bayesian methods are more adaptive but computationally more expensive than empirical Bayes  

## Contents

- `Reproduction_NSHPC_SparseSeq.Rmd`  
  Code for posterior computation and simulation  

- `Simulation-Report.pdf`  
  Brief review of the model specification, theoretical results, and simulation analysis  
