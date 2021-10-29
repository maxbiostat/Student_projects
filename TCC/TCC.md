1) **Power law and difference functions**
Para tanto, vamos rever e estender as abordagens de Gillespie (Annals of Applied Statistics, 2017).
In this project we are interested in developing a Bayesian approach that uses all of the available data to estimate the parameters of a power law distribution (in particular its scale, `alpha`).
Often times the data do not look like a power law for small values and this compromises the overall fit.
One simple idea is to introduce a difference function that quantifies how different the distribution is from a power law.
We will extend the ideas of Gillespie (2017) and explore a plethora difference functions. 
References: [Gillespie (2017)](https://www.jstor.org/stable/26362189) and the [poweRlaw](https://github.com/csgillespie/poweRlaw) package.
Abilities: Stan/C++, Bayesian statistics.

2) **Making Public Health Data sets truly available**
O Ministério da Saúde disponibiliza uma quantidade enorme de dados através do DATASUS (http://www2.datasus.gov.br/). Esses dados estão muitas vezes disponíveis em estado bruto (sem nenhuma limpeza) num  formato difícil de usar.
Neste projeto queremos utilizar a biblioteca PySUS (https://github.com/AlertaDengue/PySUS) para produzir alguns bancos e respectivas visualizações  que auxiliem pesquisadores na área de Saúde Pública a terem acesso a dados confiáveis e fáceis de utilizar.
Referências: links acima
Habilidades: Python/SQL, bancos de dados, visualização.

3) **Variable selection for spatial epidemiology studies**
Neste projeto estamos interessados em implementar e avaliar estratégias de seleção de variáveis no contexto de estudos epidemiológicos, com o objetivo de entender os fatores que influenciam a dinâmica espacial da doença.
Para isso, vamos estudar uma estratégia de seleção de variáveis por busca estocástica (SSVS na sigla em inglês) acoplada a um modelo espacial do tipo BYM.
Vamos buscar uma implementação marginalizada eficiente na linguagem Stan.
O projeto vai analisar um rico conjunto de dados epidemiológicos da epidemia de Ebola na África ocidental entre 2013 e 2016.
Habilidades: Stan/C++, estatística espacial.

4) **Adaptive truncation for effective sample size estimation**
Neste projeto queremos utilizar as técnicas de Carvalho & Moreira (2021) para determinar o truncamento da série de autocorrelações.
Comparar com o positive sequence do Geyer e com o que é feito no Stan.

5) **Acceleration methods for infinite series in Statistics**
Here we are interested in 
See Chapter 8 (pg. 300) in [Expansions and Asymptotics for Statistics](https://www.esalq.usp.br/departamentos/lce/arquivos/aulas/2011/LCE5866/Expansions%20and%20Asymptotics%20for%20Statistics.pdf)
