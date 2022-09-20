
# Iniciação Científica

## Teoria

T1) **A posteriori de Jeffreys para o tamanho de população é própria?**

Em genética de populações, o tamanho de população, Ne(t), é uma quantidade central para entender a dinâmica evolutiva de uma população natural.
Em uma análise bayesiana, é preciso estipular uma distribuição _a priori_ para Ne(t) e, no caso constante, Ne(t) = a para todo t, usualmente se utiliza uma priori de Jeffreys, p(a) ~ 1/a.
É possível mostrar que esta priori imprópria leva a uma posteriori também imprópria para o caso de um modelo Jukes-Cantor de evolução.
Neste projeto o aluno vai mostrar rigorosamente este primeiro resultado e também avaliar como/se ele se generaliza para outros modelos da mesma classe (modelos Markov diagnonalizáveis).

Habilidades a serem desenvolvidas: filogenética estatística, estatística bayesiana.

---

T2) **A conexão entre regras de pontuação próprias e o teorema da proporcionalidade de verossimilhanças**

Regras de pontuação próprias ([proper scoring rules](https://github.com/maxbiostat/proper_scoring_rules), PSR) são dispositivos matemáticos para avaliar predições probabilísticas que incentivam a honestidade do analista ("forecaster").
São largamente utilizadas na avaliação de predições ("forecasts") de modelos em finanças, metereologia e epidemiologia.
[Gonçalves e Franklin (2019)](https://arxiv.org/abs/1906.10733) recentemente provaram uma versão geral do chamado teorema da proporcionalidade de verossimilhanças (TPV), que diz que sob condições de regularidade, é sempre possível encontrar duas funções mensuráveis que representam a verossimilhança e diferem apenas por uma constante. 
Neste projeto, o aluno vai explorar a conexão entre as chamadas regras de pontuação próprias _locais_ e o TPV, e investigar se é possível provar alguns resultados clássicos da teoria de PSR utilizando esse novo teorema. 

Habilidades a serem desenvolvidas: estatística teórica.

## Aplicações

A1) **Medidas de diagnóstico para MCMC com variáveis binárias**

Métodos de cadeias de Markov Monte Carlo (MCMC) constituem uma classe extremamente útil de métodos numéricos, com aplicações todas as áreas da estatística. A correta aplicação destes métodos depende, no entanto, depende de diagnosticar problemas de convergência e performance. 
Conquanto para variáveis contínuas existam várias medidas diagnósticas bem estabelecidas, para variáveis binárias ou categóricas o conjunto de ferramentas disponíveis é muito menor.
Em [trabalho recente](https://github.com/maxbiostat/presentations/blob/master/PDF/Phylo_MCMC_diagnostics.pdf), novas medidas foram propostas para variáveis binárias. Neste projeto o aluno irá estender alguns resultados já encontrados ao derivar as características assintóticas de algumas medidas bem como suas distribuições amostrais.

Habilidades a serem desenvolvidas: MCMC, R, métodos numéricos, cadeias de Markov de tempo discreto. 

---

A2) **Aceleração e truncamento de séries infinitas**

Em [Carvalho & Moreira (2022)](https://arxiv.org/abs/2202.06121) investigamos estratégias de truncamento de séries infinitas para garantir aproximações de séries infinitas com erro controlado. Neste projeto, buscamos estender as técnicas desenvolvidas utilizando técnicas de aceleração de séries (ver pg 300, seção 8.6 de [Small, 2010](https://www.esalq.usp.br/departamentos/lce/arquivos/aulas/2011/LCE5866/Expansions%20and%20Asymptotics%20for%20Statistics.pdf)). Aplicações incluem a estimação do espectro de autocorrelação de uma cadeia de Markov e ainda muitos problemas de marginalização em Estatística.

Trabalho em conjunto com [Guido Moreira](https://github.com/GuidoAMoreira).

Habilidades a serem desenvolvidas: análise numérica; R, C++.

---

A3) **sumPy: truncamento numericamente estável de séries infinitas em Python**

Neste projeto queremos portar e expandir as funcionalidades do pacote do R [**sumR**](https://github.com/GuidoAMoreira/sumR) na linguagem Python. A ideia é reproduzir a estrutura do pacote R, criando _wrappers_ para as funções em baixo nível (já implementadas em C). Queremos também adicionar _features_ como a capacidade de tratar séries que podem ser negativas.

Trabalho em conjunto com [Guido Moreira](https://github.com/GuidoAMoreira).

Habilidades a serem desenvolvidas: programação científica em Python e C.

---

# Honours thesis (TCC)

I prefer that the student writes their project in English for practice.  Here are a few suggestions of projects:

T1)  **Power law and difference functions**

Power law distributions are an important class of statistical models, allowing us to model fenomena which take values over orders of magnitude.
In this project we are interested in developing a Bayesian approach that uses all of the available data to estimate the parameters of a power law distribution (in particular its scale, `alpha`).
Often times the data do not look like a power law for small values and this compromises the overall fit.
One simple idea is to introduce a difference function that quantifies how different the distribution is from a power law.
We will extend the ideas of Gillespie (2017) and explore a plethora difference functions. 

References: [Gillespie (2017)](https://www.jstor.org/stable/26362189) and the [poweRlaw](https://github.com/csgillespie/poweRlaw) package.

Skills to be developed: Stan/C++, Bayesian statistics.

---

T2)  **Elicitation and prior modelling for rate variation in phylogenetics**

Phylogenetics is a central tool to modern biology and operates by modelling variation in molecular sequences (RNA/DNA/proteins) in order to infer patterns of ancestry between organisms and pathogen variants.
A crucial model component is  variation in the evolutionary rate across sites in the genome. Moreover, an important but overlooked aspect is that of how to construct prior distributions for quantities of interest in the so-called rate-heterogeneity models. In this project the student will exploit some ideas on principled prior elicitation and will also test the empirical performance of these approaches on real and simulated data. 

References: [Chira & Thomas (2016)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5217074/) and the [SHELF](http://www.tonyohagan.co.uk/shelf/) package. 

Skills to be developed: Statistical phylogenetics, Bayesian statistics, JAVA.

T3) **Studying phylogenetic distances for time-calibrated trees**
Time-calibrated phylogenies are central objects in Molecular Epidemiology and Phylodynamics.
Computing distances between trees is fundamental task in the analysis of samples of trees ([Smith, 2022](https://academic.oup.com/sysbio/article/71/5/1255/6486431)), but there is no canonical distance in the space of phylogenies.
Faced with many choices of metric, what is the analyst to do? In this project the student will start by investigating an easily computable metric on phylogenies proposed by [Kendall & Coljin (2015)](https://arxiv.org/abs/1507.05211). The KC metric takes a convex combination `lambda*TD + (1-lambda)*BD`, where `TD` and `BD`are "topological" and "branch length" distances, respectively. The task is to figure out how to calibrate the free parameter `lambda` automatically such that distances capture important features.

Skills to be developed: Computational statistics, Statistical phylogenetics.


A1) **Survival and reproductive analysis of _Rhodnius prolixus_, the Chagas disease vector**

Chagas disease continues to pose important challenges to Public Health in Brazil. With climate change and temperate zones potentially becoming warmer and more hospitable to the disease's vector, _Rhodnius prolixus_, this might become a global concern.
In this project the student will analyse an experimental data set of _Rhodnius prolixus_ mortality and fertility (egg production) in various temperatures and fit state-of-the-art survival and dynamic regression models in order to help understand the potential impact of climate change on the suitability of certain areas to the spread and stablishment of _Rhodnius_ populations.

This is joint work with [Professor Angela Hampshire](https://www.microbiologia.ufrj.br/portal/index.php/pt/43-pos-graduacao/corpo-docente/2017-2020/208-angela-hampshire-de-carvalho-santos-lopes) (UFRJ).

References: [Carvalho, Struchiner & Bastos (2015)](https://github.com/maxbiostat/papers/blob/master/PAPERS/Carvalho_et_al_2015_EBEB.pdf).

Skills to be developed: Applied Statistics, Bayesian statistics, survival analysis, R.

A2) **PhyloPosteriorDB: a collection of curated phylogenetic data sets for method development**

Having a set of curated, well-studied and realistic data sets is a great asset for the development of new analytical methods. In particular, Markov Chain Monte Carlo (MCMC) can be challenge to develop and test without a reliable benchmark. Inspired by the [**posteriordb**](https://github.com/stan-dev/posteriordb) project, the student will improve and expand [**this**](https://github.com/maxbiostat/MEP_data) collection of rich, real-world data sets in order to provide the [Phylogenetics community](https://www.phylobabble.org/) with easy-to-use data to check their new methods against. The student will also develop novel memmory-efficient ways of storing large posterior samples of trees that can be accessed and used for further processing. 

Skills to be developed: [BEAST](https://github.com/beast-dev/beast-mcmc), Database programming, Statistical Phylogenetics.

A3) **Rao-Blackwellising Bayesian Stochastic Search Variable Selection**

In statistical applications with limited data, it is important to enforce _regularisation_, that is to encode parsimony into the modelling process so that our models do not overfit the data and lose predictive power. Moreover, it is important to encode _sparsity_, that is the notion that big effects are few and far between, floating in a sea of irrelevance. In this project, we will return to basics and give the **Bayesian Stochastic Search Variable Selection (BSSVS)** model of [George & Mcculloch (1993)](https://people.eecs.berkeley.edu/~russell/classes/cs294/f05/papers/george+mcculloch-1993.pdf) a modern spin. In particular, we will marginalise over the discrete predictor assigments, effectively providing a Rao-Blackwellised version of the model. Implementation will be done in the [Stan](https://mc-stan.org/) probabilistic programming language. In particular, we will investigate how to exploit massive parallelisation in the form of the [`reduce_sum`](https://mc-stan.org/docs/2_23/stan-users-guide/reduce-sum.html) in order to speed things up.

Skills to be developed: Stan and C++ programming, Bayesian statistics. 


