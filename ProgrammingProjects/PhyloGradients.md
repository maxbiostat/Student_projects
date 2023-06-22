## Efficient implementation of the phylogenetic likelihood and its gradients

Phylogenetics is awesome. But it is also a rather difficult problem, both statistically and computationally.
Somewhat recent advances have made efficient algorithms such as [Hamiltonian Monte Carlo (HMC)](https://mc-stan.org/docs/reference-manual/hamiltonian-monte-carlo.html) go mainstream.
While we can't do proper HMC for trees just yet, we can fix the tree and do HMC on branch lengths and other parameters.
But for that to work, we need the phylogenetic likelihood to be programmed efficiently. 

Your job is to take the implementation of the phylogenetic likelihood in [**phylostan**](https://github.com/4ment/phylostan) and code it directly in the templated C++ required by the [Stan math library](https://github.com/stan-dev/math).
You'll also need to code up the gradients of the likelihood.
For this project you might want to check out [my notes](https://github.com/maxbiostat/Statistical_Phylogenetics_resources) on learning phylogenetics. 

This is not a project for the faint of heart: there will be A LOT of work to get this working. Hopefully the speedups will be worth it. Nae guarantees. 
