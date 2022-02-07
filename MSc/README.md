# Master's projects

For most of the projects outlined here, you are expected to have taken [Probability](https://emap.fgv.br/disciplina/mestrado/probabilidade), [(Mathematical) Statistics](https://emap.fgv.br/disciplina/mestrado/inferencia-estatistica) and [Computational Statistics](https://emap.fgv.br/disciplina/doutorado/estatistica-computacional) by the time you start the project. 

## Theory

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
