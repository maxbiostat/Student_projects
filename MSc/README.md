# Master's projects

For most of the projects outlined here, you are expected to have taken [Probability](https://emap.fgv.br/disciplina/mestrado/probabilidade), [(Mathematical) Statistics](https://emap.fgv.br/disciplina/mestrado/inferencia-estatistica) and [Computational Statistics](https://emap.fgv.br/disciplina/doutorado/estatistica-computacional) by the time you start the project. 

## Theory

T1) **What ails the King?**

Concentration areas: Bayesian Statistics.

In [The King Must Die](https://statmodeling.stat.columbia.edu/2017/11/02/king-must-die/), Dan Simpson argues that the Bayesian least absolute shrinkage and selection operator (LASSO) cannot possibly work because its usual prior structure (the Laplace) prior cannot simultaneously accommodate sparsity and large signals. It is also argued that strategies such as the 'Finnish' horseshoe ([Piironen and Vehtari, 2017](https://doi.org/10.1214/17-EJS1337SI)) can remedy this issue. 
In this project, the student will give a rigorous and inclusive account of sparsity-inducing priors for Bayesian variable selection and will investigate how the claims about the Bayesian LASSO hold up in the correlated case, where covariates are colinear.

References:
- [Bai, Rockova & George (2021)](http://raybai.net/wp-content/uploads/2021/05/SSL_review.pdf).
- [Carvalho [not me!], Polson & Scott (2009)](http://proceedings.mlr.press/v5/carvalho09a.html).
- [Sparsity Blues](https://betanalpha.github.io/assets/case_studies/modeling_sparsity.html) by Michael Betancourt.

---

T2) **Combining densities under non-invertible transforms**

Concentration areas: Theoretical Statistics, Functional Analysis, Bayesian Statistics.

One of the questions left open by [Carvalho et al. (2022)](https://arxiv.org/abs/1502.04206) is: "what happens when your experts give you opinions about a quantity in the space `X` but you're interested in `g(X)` where `g` is non-invertible?". In this project we seek to investigate how one would go about combining probability densities in this situation. One approach is to minimise the KL distance in transformed space, but this needs theoretical grounding and also a study of the conditions necessary for the pushforward measure to have a density. The student will be required to prepare a thorough treatment of pushforward probability measures and then prove a few results concerning the interaction of measurable transformations and the logarithmic pooling operator.

References:
- Billingsley's [Probability and Measure](https://www.colorado.edu/amath/sites/default/files/attached-files/billingsley.pdf).
- Section 3.3 in [Poole and Raftery (2000)](https://www.stat.washington.edu/raftery/Research/PDF/poole2000.pdf).

---

## Applications

A1) **Prevalence estimation and causal inference through regression models with uncertain outcomes**

Concentration areas: Biostatistics, Epidemiology.

As the COVID-19 pandemic took the planet by storm, it became apparent the mass testing would be required in order to understand the extent of the virus's spread in the population.
However, as the diagnostic tests are imperfect, the outcome data (Infected/Not-infected) comes with observation error, which must be correctly modelled.
Whilst the general problem of prevalence estimation under outcome uncertainty has been studied for at least four decades, the interface with regression models saw a recent revival, in no small part due to COVID-19 (see [Gelman & Carpenter (2020)](http://www.stat.columbia.edu/~gelman/research/unpublished/specificity.pdf)).
There are however many open regression problems, such as for instance re-testing of positive cases, a routine procedure nowadays. 
The student will be expected to implement and extend the models in Section 7.3 of [Bastos, Carvalho & Gomes (2021)](https://github.com/maxbiostat/papers/blob/master/PAPERS/2021_Bastos_Carvalho_Gomes.pdf) using both simulated and real-world data. 

References:
- In addition to the references already given, Lucas Moschen's [honours thesis](https://github.com/lucasmoschen/rds-bayesian-analysis-tcc) is great resource.
- [This](https://github.com/epiforecasts/inc2prev) repository might come in handy.

---

A2) **Simultaneous nowcasting and Rt estimation for epidemic surveillance**

Concentration areas: Biostatistics, Epidemiology.

Timely inferences on the short term behaviour of epidemics is of crucial importance to effective decision-making.
Many statistical approaches have been developed for predicting COVID-19 cases, hospitalisations and deaths.
Disease reporting data in general and COVID-19 data in particular present a number of methodological challenges due to reporting issues such as underreporting and reporting delays.
These then need to be statistically corrected to give a better picture of the actual numbers of cases at any given moment ([Bastos, Carvalho & Gomes (2021)](https://github.com/maxbiostat/papers/blob/master/PAPERS/2021_Bastos_Carvalho_Gomes.pdf)).
Another aspect of epidemic surveillance is tracking the effective reproductive number (Rt) of the disease through time, as measure of risk of (exponential) disease spread. 
In this project, the student will couple the delay-correction nowcasting model of [Bastos et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/sim.8303) and the Rt estimation methods in the R package [EpiEstim](https://github.com/mrc-ide/EpiEstim) to create a unified framework for accurate Rt calculation by explicitly modelling data misreporting. 

This is joint work with Drs [Leo Bastos](https://lsbastos.github.io/) and [Marcelo Gomes](https://scholar.google.com/citations?user=b018FBIAAAAJ&hl=en&authuser=1&oi=ao). 

---

A3) **Parsimonious models of pathogen spatial spread: prior modelling and variable selection for phylogeography**

Concentration areas: Biostatistiscs, Statistical Phylogenetics.

Since its introduction in [Lemey et al (2009)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000520), Bayesian phylogeography has become a major tool for assessing the drivers of pathogen spatial spread. 
In this project the student will be expected to complete two tasks:
1. Compose a thorough review of the literature on Bayesian phylogeography, along with a curated collection of data sets to be used in further analyses and
2. Experiments investigating the effect of prior stringency on the resulting inferences, including the set of selected ('significant') covariates.

References:

- [Lemey et al. (2014)](https://journals.plos.org/plospathogens/article?id=10.1371/journal.ppat.1003932).
- [Dudas, Carvalho, et al (2017)](https://www.nature.com/articles/nature22040).
- Chapter 4 in my [PhD thesis](https://github.com/maxbiostat/PhD_Thesis).
