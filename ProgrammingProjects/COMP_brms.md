## Principled and efficient truncation of the Conway-Maxwell Poisson distribution in brms

In this project you will take the (Stan) implementations of the techniques in [this](https://arxiv.org/abs/1308.2045) paper, which are [here](https://github.com/GuidoAMoreira/stan_summer) and port them to [brms](https://github.com/paul-buerkner/brms).
In particular, you will improve the implementation of the [Conway-Maxwell Poisson](https://en.wikipedia.org/wiki/Conway%E2%80%93Maxwell%E2%80%93Poisson_distribution) pmf in [here](https://github.com/paul-buerkner/brms/blob/master/inst/chunks/fun_com_poisson.stan) by adding adaptive truncation.
You will have to run correctness tests as well as ensure that the implementation is stable enough to be used in general regression problems. 
