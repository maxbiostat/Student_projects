
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

A1) **Tornando o DATASUS mais acessível**

A crise da COVID-19 trouxe à tona a necessidade de dados públicos confiáveis e de fácil acesso para o auxílio à tomada de decisão.
Neste projeto o aluno vai utilizar a biblioteca [PySUS](https://github.com/AlertaDengue/PySUS) para extrair dados das bases públicas do Ministério da Saúde e do IBGE para gerar tabelas e visualizações de interesse.
Isso inclui dados de nascimentos, mortalidade, internações e atendimento ambulatorial.
O objetivo final é disponibilizar uma série de bancos de dados curados e consolidados que sejam de fácil consulta para profissionais de saúde e epidemiologistas.

Habilidades a serem desenvolvidas: Python, SQL (Big Query), visualização, Saúde Pública.

---

A2) **Medidas de diagnóstico para MCMC com variáveis binárias**

Métodos de cadeias de Markov Monte Carlo (MCMC) constituem uma classe extremamente útil de métodos numéricos, com aplicações todas as áreas da estatística. A correta aplicação destes métodos depende, no entanto, depende de diagnosticar problemas de convergência e performance. 
Conquanto para variáveis contínuas existam várias medidas diagnósticas bem estabelecidas, para variáveis binárias ou categóricas o conjunto de ferramentas disponíveis é muito menor.
Em [trabalho recente](https://github.com/maxbiostat/presentations/blob/master/PDF/Phylo_MCMC_diagnostics.pdf), novas medidas foram propostas para variáveis binárias. Neste projeto o aluno irá estender alguns resultados já encontrados ao derivar as características assintóticas de algumas medidas bem como suas distribuições amostrais.

Habilidades a serem desenvolvidas: MCMC, R, métodos numéricos, cadeias de Markov de tempo discreto. 

---

A3) **Processos gaussianos convexos e suas aplicações**

Neste projeto estamos interessados em explorar certas propriedades das derivadas de processos gaussianos que permitem a modelagem de funções de interesse a partir das suas derivadas.
Em particular, queremos estender resultados recentes que empregam emulação de funções para resolver os chamados problemas duplamente intratáveis.
Uma vez desenvolvidos os métodos, vamos investigar uma aplicação nas chamadas [normalised power priors](https://onlinelibrary.wiley.com/doi/10.1002/sim.9124), que são muito utilizadas na análise de ensaios clínicos.

Habilidades a serem desenvolvidas: processos gaussianos; Stan/C++; estatística bayesiana.

---

A4) **Aceleração e truncamento de séries infinitas**

Em [Carvalho & Moreira](https://github.com/maxbiostat/truncation_tests) investigamos estratégias de truncamento de séries infinitas para garantir aproximações de séries infinitas com erro controlado. Neste projeto, buscamos estender as técnicas desenvolvidas utilizando técnicas de aceleração de séries (ver pg 300, seção 8.6 de [Small, 2010](https://www.esalq.usp.br/departamentos/lce/arquivos/aulas/2011/LCE5866/Expansions%20and%20Asymptotics%20for%20Statistics.pdf)). Aplicações incluem a estimação do espectro de autocorrelação de uma cadeia de Markov e ainda muitos problemas de marginalização em Estatística.

Habilidades a serem desenvolvidas: análise numérica; R, C++.

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

A1) **Survival and reproductive analysis of _Rhodnius prolixus_, the Chagas disease vector**

Chagas disease continues to pose important challenges to Public Health in Brazil. With climate change and temperate zones potentially becoming warmer and more hospitable to the disease's vector, _Rhodnius prolixus_, this might become a global concern.
In this project the student will analyse an experimental data set of _Rhodnius prolixus_ mortality and fertility (egg production) in various temperatures and fit state-of-the-art survival and dynamic regression models in order to help understand the potential impact of climate change on the suitability of certain areas to the spread and stablishment of _Rhodnius_ populations.

This is joint work the [Professor Angela Hampshire](https://www.microbiologia.ufrj.br/portal/index.php/pt/43-pos-graduacao/corpo-docente/2017-2020/208-angela-hampshire-de-carvalho-santos-lopes) (UFRJ).

References: [Carvalho, Struchiner & Bastos (2015)](https://github.com/maxbiostat/papers/blob/master/PAPERS/Carvalho_et_al_2015_EBEB.pdf).

Skills to be developed: Applied Statistics, Bayesian statistics, survival analysis, R.

A2)  **Variable selection for spatial epidemiology studies**

A major problem in real-world applications is discerning which variables are associated (causally or otherwise) with an outcome.
When many covariates/features are available, the job of finding a set of covariates that parsimoniously "explain" the response is a difficult one.
In this project we are interested in implementing and evaluating variable selection strategies in the context of epidemiological studies, in order to understand the factors that influence the spatial dynamics of the disease.
For this, we will study a stochastic search variable selection strategy (SSVS) coupled to a Besag-York-Molié (BYM) spatial model.
In particular, we will adapt an efficient marginalized [implementation](https://mc-stan.org/users/documentation/case-studies/icar_stan.html) in the Stan language.
The project will analyze a rich set of epidemiological data from the Ebola epidemic in West Africa between 2013 and 2016.

References: [Morris et al. 2019](http://www.stat.columbia.edu/~gelman/research/published/bym_article_SSTEproof.pdf) and Chapter 4 of my [PhD thesis](https://github.com/maxbiostat/PhD_Thesis). 

Skills to be developed: JAGS, Stan/C++, spatial statistics.

A3) **PhyloPosteriorDB: a collection of curated phylogenetic data sets for method development**

Having a set of curated, well-studied and realistic data sets is a great asset for the development of new analytical methods. In particular, Markov Chain Monte Carlo (MCMC) can be challenge to develop and test without a reliable benchmark. Inspired by the [**posteriordb**](https://github.com/stan-dev/posteriordb) project, the student will improve and expand [**this**](https://github.com/maxbiostat/MEP_data) collection of rich, real-world data sets in order to provide the [Phylogenetics community](https://www.phylobabble.org/) with easy-to-use data to check their new methods against. The student will also develop novel memmory-efficient ways of storing large posterior samples of trees that can be accessed and used for further processing. 

Skills to be developed: [BEAST](https://github.com/beast-dev/beast-mcmc), Database programming, Statistical Phylogenetics.
