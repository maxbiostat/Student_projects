## Efficiently computing covariance matrices for binary data  

Let **X** be P-dimensional binary vector. Now suppose you have a sample **D** = (**X1**, **X2**, ..., **Xn**). The task is to compute the P x P covariance matrix of **X** from the sample. 

In R you could presumably do
```R
cov(D) 
```
The problem is that in many cases this will give you a matrix that is not positive-definite. One way to fix the problem is to realise that for binary variable we can compute the covariance between Xi and Xj by computing
```
cov_ij = p_ij - p_i*p_j.
```
The problem then becomes doing this efficiently. The task is embarrassingly parallelisable, but coding in R is still slow.

Your job is to take the implementation  of `binary_cov_matrix()` in [here](https://github.com/maxbiostat/BinaryMarkovChains/blob/main/R/binary_multiESS.R) and make it go vrum vrum. I reckon a simple re-coding in Rcpp should do the trick.

**Applications**: this can be used in estimating the efficiency of Markov chain Monte Carlo algorithms in binary spaces. 
