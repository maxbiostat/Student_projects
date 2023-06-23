## A Stan interface to MultiBD 

[**MultiBD**](https://github.com/msuchard/MultiBD) is an R package to compute birth-death transition probabilities.
It can be used to fit epidemic models very efficiently. 
A fully Bayesian approach, however, necessitates Markov chain Monte Carlo methods.
In this project you will port the code in **MultiBD** for both the likelihood and its gradients which is written in C++  to the templated C++ required by the [Stan math library](https://github.com/stan-dev/math).
This will allow us to fit complex hierarchical models to epidemic data using HMC. 
The goal is to have the machinery in place to extend the analysis in Section 6 of 10.1214/18-AOAS1141](https://projecteuclid.org/journals/annals-of-applied-statistics/volume-12/issue-3/Direct-likelihood-based-inference-for-discretely-observed-stochastic-compartmental-models/10.1214/18-AOAS1141.full).


