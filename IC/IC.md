1) Tornando o DATASUS mais acessível

A crise da COVID-19 trouxe à tona a necessidade de dados públicos confiáveis e de fácil acesso para o auxílio à tomada de decisão.
Neste projeto o aluno vai utilizar a biblioteca PySUS para extrair dados das bases públicas do Ministério da Saúde e do IBGE para gerar tabelas e visualizações de interesse.
Isso inclui dados de nascimentos, mortalidade, internações e atendimento ambulatorial.
O objetivo final é disponibilizar uma série de bancos de dados curados e consolidados que sejam de fácil consulta para profissionais de saúde e epidemiologistas.
Habilidades a serem desenvolvidas: Python, SQL (Big Query), visualização, Saúde Pública.

2) A posteriori de Jeffreys para o tamanho de população é própria? 

Em genética de populações, o tamanho de população, Ne(t), é uma quantidade central para entender a dinâmica evolutiva de uma população natural.
Em uma análise bayesiana, é preciso estipular uma distribuição _a priori_ para Ne(t) e, no caso constante, Ne(t) = a, usualmente se utiliza uma priori de Jeffreys, p(a) ~ 1/a.
É possível mostrar que esta priori imprópria leva a uma posteriori também imprópria para o caso de um modelo Jukes-Cantor de evolução.
Neste projeto o aluno vai mostrar rigorosamente este primeiro resultado e também avaliar como/se ele se generaliza para outros modelos da mesma classe.
Habilidades a serem desenvolvidas: filogenética estatística, estatística bayesiana.

3) A conexão entre regras de pontuação próprias e o teorema da proporcionalidade de verossimilhanças

Regras de pontuação próprias (proper scoring rules, PSR) são dispositivos matemáticos para avaliar predições probabilísticas que incentivam a honestidade do analista ("forecaster").
São largamente utilizadas na avaliação de predições ("forecasts") de modelos em finanças, metereologia e epidemiologia.
Gonçalves e Franklin (2019) recentemente provaram uma versão geral do chamado teorema da proporcionalidade de verossimilhanças (TPV), que diz que sob condições de regularidade, é sempre possível encontrar duas funções mensuráveis que representam a verossimilhança e diferem apenas por uma constante. 
Neste projeto, o aluno vai explorar a conexão entre as chamadas regras de pontuação próprias _locais_ e o TPV, e investigar se é possível provar alguns resultados clássicos da teoria de PSR utilizando esse novo teorema. 
Habilidades a serem desenvolvidas: estatística teórica.

4) Medidas de diagnóstico para MCMC com variáveis binárias

Métodos de cadeias de Markov Monte Carlo (MCMC) constituem uma classe extremamente útil de métodos numéricos, com aplicações todas as áreas da estatística. A correta aplicação destes métodos depende, no entanto, depende de diagnosticar problemas de convergência e performance. 
Conquanto para variáveis contínuas existam várias medidas diagnósticas bem estabelecidas, para variáveis binárias ou categóricas o conjunto de ferramentas disponíveis é muito menor.
Em trabalho recente, novas medidas foram propostas para variáveis binárias. Neste projeto o aluno irá estender alguns resultados já encontrados ao derivar as características assintóticas de algumas medidas bem como suas distribuições amostrais.
Habilidades a serem desenvolvidas: MCMC, R, métodos numéricos, cadeias de Markov de tempo discreto. 

5) Processos gaussianos convexos e suas aplicações

Neste projeto estamos interessados em explorar certas propriedades das derivadas de processos gaussianos que permitem a modelagem de funções de interesse a partir das suas derivadas.
Em particular, queremos estender resultados recentes que empregam emulação de funções para resolver os chamados problemas duplamente intratáveis.
Uma vez desenvolvidos os métodos, vamos investigar uma aplicação nas chamadas "normalised power priors", que são muito utilizadas na análise de ensaios clínicos.
Habilidades a serem desenvolvidas: processos gaussianos; Stan/C++; estatística bayesiana.
