TRABALHO FINAL
================
Gabriela Silva, Guilherme Amasilis, Melissa Dias e Mylena Dias
02/08/2020

###### Relatório dinâmico contendo análise exploratória de base de dados

### 1 INTRODUÇÃO

O presente trabalho objetiva analisar os dados relacionados ao [**Exame
Nacional de Desempenho dos Estudantes
(Enade)**](http://portal.inep.gov.br/enade) do ano de 2018. Esse se
configura como um dos indicadores que integra o Sistema Nacional de
Avaliação da Educação Superior (Sinaes), uma vez que ele avalia os
cursos por meio dos desempenhos dos estudantes e se constitui como um
dos importantes insumos para a construção de um panorama da qualidade
dos cursos e das instituições de educação superior brasileiras.

As perguntas que orientarão a análise dos dados são:

1)  Dentre as diferentes Organizações Acadêmicas observadas, qual possui
    maior média de Conceito Enade Contínuo?

2)  Considerando a Universidade Federal de Minas Gerais, como se dá a
    distribuição do Conceito Enade Faixa para os cursos avaliados?

3)  Sob a perspectiva da distribuição do Conceito Enade Faixa no curso
    de administração pública no país, existe alguma diferença entre as
    duas modalidades de ensino (a distância/presencial)?

4)  Existe alguma correlação entre a proporção de participantes no exame
    (concluintes participantes/concluintes inscritos) e o Conceito Enade
    Faixa?

### 2 DESCRIÇÃO DA BASE DE DADOS

A base de dados utilizada é composta por 22 variáveis e se refere aos
resultados do Conceito Enade de 2018 relativos ao ano III de avaliação,
o qual abarca cursos das seguintes áreas de conhecimento:

  - Cursos de bacharelado nas Áreas de Conhecimento Ciências Sociais
    Aplicadas e áreas afins;
  - Cursos de bacharelado nas Áreas de Conhecimento Ciências Humanas e
    áreas afins que não tenham cursos também avaliados no âmbito das
    licenciaturas;
  - Cursos Superiores de Tecnologia nas áreas de Gestão e Negócios,
    Apoio Escolar, Hospitalidade e Lazer, Produção Cultural e Design.

(INEP, 2019)

Vale ressaltar os parâmetros de conversão da nota dos concluintes no
Enade do curso de graduação (NCc) em Conceito Enade Faixa:

O **conceito 1** do Enade Faixa diz respeito ao intervalo 0 ≤ NCc \<
0,945 do contínuo; O **conceito 2** do Enade Faixa diz respeito ao
intervalo 0,945 ≤ NCc \< 1,945 do contínuo; O **conceito 3** do Enade
Faixa diz respeito ao intervalo 1,945 ≤ NCc \< 2,945 do contínuo; O
**conceito 4** do Enade Faixa diz respeito ao intervalo 2,945 ≤ NCc \<
3,945 do contínuo; O **conceito 5** do Enade Faixa diz respeito ao
intervalo 3,945 ≤ NCc ≤ 5 do contínuo.

(INEP, 2018)

Além disso, a presente base de dados fornece informações que abarcam a
área de avaliação, o nome da Instituição de Ensino Superior (IES), o
município do curso, a organização acadêmica, o Conceito Enade Faixa,
dentre outras importantes dimensões e métricas para a conformação do
panorama de qualidade do Ensino Superior no Brasil.

### 3 ANÁLISE EXPLORATÓRIA

A **primeira pergunta** objetiva verificar qual das diferentes
organizações acadêmicas observadas possui maior média de Conceito
Enade Contínuo. Para isso foi construído o gráfico a seguir:

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/organizaçãoacademica-1.png)<!-- -->

**Figura 1: Média do Enade Contínuo por organização acadêmica**

A partir da visualização acima, percebeu-se que a organização acadêmica
que possui maior média de Conceito Enade Contínuo é **Centro Federal de
Educação Tecnológica (aproximamente 4.5)** seguida em ordem descrescente
dessa mesma média por: Instituto Federal de Educação, Ciência e
Tecnologia (3); Universidade (2,7); Centro Universitário (2,4);
Faculdade (2,2).

É importante destacar que as duas primeiras organizações acadêmicas com
maiores médias apresentam uma quantidade de cursos avaliados bem menor
que as outras 3 restantes. Isso, ao longo da análise, principalmente na
pergunta 4, será retratado de modo mais evidente.

A **segunda pergunta** analisada questiona acerca de como se dá a
distribuição do Conceito Enade (Faixa) para os cursos avaliados da
Universidade Federal de Minas Gerais (UFMG). O gráfico obtido a partir
da manipulação dos dados encontra-se a seguir:

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/pergunta2-1.png)<!-- -->

**Figura 2: Conceito Enade UFMG**

A base de dados apresenta o Conceito Enade (Faixa) para doze diferentes
áreas de avaliação: Administração (Campus Belo Horizonte),
Administração (Campus Montes Claros), Administração Pública, Ciências
Contábeis, Ciências Econômicas, Comunicação Social – Jornalismo,
Comunicação Social – Publicidade e Propaganda, Design, Direito,
Psicologia, Relações Internacionais e Turismo. Destes, 8 cursos (66,67%)
obtiveram nota máxima (5) no conceito Enade, enquanto os outros 4 cursos
(33,33%) obtiveram nota 4. Dessa forma, observa-se que a UFMG alcançou
notas altas na avaliação realizada.

A **terceira pergunta** se refere ao comparativo do Conceito Enade
Faixa, entre as duas modalidades de ensino (a distância/presencial), no
curso de administração pública. A priori, para se esboçar um gráfico de
distribuição, torna-se mais apropriado utilizar a variável Conceito
Enade Contínuo, como foi feito no gráfico abaixo:

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/pergunta3-1.png)<!-- -->

**Figura 3: Distribuição Conceito Enade (Contínuo) no curso de Adm.
Pública**

Apesar de possuir alguns pontos sobrepostos na região central,
consegue-se perceber, com clareza, que existe uma tendência da
modalidade de ensino presencial, no curso de Administração Pública,
possuir maiores pontuações no Conceito Enade (Contínuo) do que a
modalidade de ensino à distância, haja vista que a grande maioria dos
cursos à distância estão concentrados na metade para baixo do gráfico e
a grande maioria dos cursos presenciais estão concentrados na metade
para cima.

Contudo, uma vez que a intenção inicial era manipular dados do Conceito
Enade (Faixa), pode-se, pois, calcular a média obtida, para esse
conceito, para cada uma das duas modalidades de ensino. O gráfico abaixo
ilustra os resultados obtidos:

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/pergunta3.1-1.png)<!-- -->

**Figura 4: Média do Enade (Faixa) por modalidade de ensino no curso de
Adm. Pública**

Vê-se que existe, de fato, uma diferença considerável nas médias das
pontuações obtidas para cada uma das modalidades de ensino,
correspondendo a média do Conceito Enade (Faixa) para a modalidade à
distância 2,03 e para modalidade presencial 3,44.

A fim de investigar se essa tendência, observada para o curso de
Administração Pública, também se aplica para os demais cursos
apresentados na tabela, foi construído o gráfico a seguir:

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/pergunta3.2-1.png)<!-- -->

**Figura 5: Média do Enade (Faixa) por modalidade de ensino nos diversos
cursos**

Como pode ser visto, a mesma tendência se aplica para os cursos de
Relações Internacionais (média de 2,00 para modalidade à distância e
de 3,17 para presencial) e Serviço Social (média de 1,90 para modalidade
à distância e de 2,98 para presencial). Em contrapartida, os cursos de
Direito (média de 4,00 para modalidade à distância e de 2,87 para
presencial) e Ciências Econômicas (média de 3,29 para modalidade à
distância e de 2,62 para presencial) seguem o caminho inverso, ou seja,
há uma maior pontuação para os cursos à distância ante os presenciais.
Os demais cursos não possuem diferenças consideráveis entre as médias,
já que as colunas de seus respectivos gráficos possuem alturas
similares.

A **quarta pergunta** diz respeito à investigação se existe alguma
correlação entre a proporção de participantes no exame (concluintes
participantes/concluintes inscritos) e o Conceito Enade Faixa. O gráfico
a seguir objetiva responder tal questionamento:

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/pergunta4-1.png)<!-- -->

**Figura 6: Percentual de participação e Conceito Enade Faixa**

Pode-se observar que essa visualização apresenta alguns problemas, uma
vez que o Conceito Enade Faixa não envolve números decimais, o que
acarreta a concentração dos pontos na linha verticalmente. Entretanto,
pode-se observar que um menor percentual de participantes (entre 0% e
25%) não está, necessariamente, apenas relacionado a notas baixas como a
nota 1. Nota-se que os menores percentuais de participação estão
associados às notas 2, 3 e 4 com destaque para a 3 e a 4 (maiores
concentrações de pontos abaixo de 25%)

Com o objetivo de melhorar a visualização e tentar extrair mais
informações dos dados, abaixo se encontra outro gráfico que não estava
no escopo inicial das perguntas, porém foi uma alternativa encontrata
visando compreender melhor os dados. Nesse caso, foi utilizado o
Conceito Enade Contínuo como um dos eixos.

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/pergunta4.1-1.png)<!-- -->

**Figura 7: Proporção de participantes e Conceito Enade Contínuo**

Nesse gráfico, o que se pode perceber é a maior concentração dos pontos
entre os Conceitos 1 e 3 e acima do percentual de 75% de participação.
Dos Conceitos 3 a 4 também há elevada concentração de pontos, porém em
menor medida comparado ao intervalo de 1 a 3, de modo que uma das razões
que pode estar relacionada à maior quantidade de pontos estarem entre os
Conceitos 1 a 3 seria o fato da maioria dos cursos obterem notas nesse
intervalo. Além disso, nota-se que há cursos avaliados em todo o
intervalo do Conceito Enade Contínuo.

![](hw99-analise-viz-dados-grupo08_files/figure-gfm/pergunta4.2-1.png)<!-- -->

**Figura 8: Participação e Enade Contínuo por Organização Acadêmica**

Esse gráfico também não estava envolvido nas perguntas iniciais, mas
devido à possibilidade de abordar essa questão de diversos modos, tal
visualização foi construída. O que se pode perceber a partir dessa é
que, em geral, faculdade e centro universitário possuem mais pontos em
menores percentuais de participação. Vale ressaltar que os Institutos
Federais de Educação, Ciência e Tecnologia e os Centros Federais de
Educação Tecnológica existem em menor quantidade comparada às outras
formas de organização acadêmica além de apresentarem maiores níveis de
participação, principalmente no caso dos segundos.

### 4 CONSIDERAÇÕES FINAIS

No âmbito da análise exploratória dos dados, algumas observações,
limitações e alternativas foram encontradas, de modo que, em cada
pergunta, objetivou-se permitir as visualizações propostas por meio das
perguntas bem como extrair informações relevantes com os dados
disponíveis.

Em relação à pergunta 1, a primeira visualização gerada apresentou
problemas, uma vez que, com exceção de uma organização acadêmica, as
outras retornaram NA para a média do Conceito Enade Contínuo. Isso
aconteceu, provavelmente, devido a células em branco de modo que, por
meio do summarise, a média não era calculada. Entretanto, foi possível
resolver essa questão retirando da conta os NAs. Assim foi possível
apresentar tal visualização.

No dataframe analisado, existem dois cursos com o nome Administração na
UFMG, diferenciando-se pelos campus em que são ofertados (um em Belo
Horizonte e outro em Montes Claros). Nesse sentido, ao realizar a
análise da questão 2, a plotagem do gráfico entendia que ambos os
valores de conceito Enade para Adminstração se referiam a apenas uma
área de atuação, levando à soma dos dois conceitos Enade na plotagem do
gráfico. Esse erro foi corrigido alterando-se o nome do curso de
Adminstração de Montes Claros, especificando que este era seu campus de
oferta.

Uma outra dificuldade encontrada na questão 2 refere-se ao tamanho dos
valores do eixo x – área de atuação – após a plotagem do gráfico. Por se
tratar de valores em caracteres, ao serem plotados automaticamente,
acabavam se sobrepondo uns aos outros, impedindo a visualização dos
valores do eixo x. Assim, realizou-se a mudança na orientação dos
valores do eixo x, dispondo-os na vertical, além de reduzir o tamanho de
sua fonte, de modo a permitir a visualização correta do gráfico.

Na questão 3, observa-se um problema na formulação inicial da pergunta,
que, por sua vez, foi abordada no trabalho de uma forma mais apropriada.
Ao se solicitar a distribuição do Conceito Enade Faixa, existe o
enquadramento das pontuações, obtida para os diversos cursos, em apenas
5 conceitos, o que geraria uma gráfico de distribuição nenhum pouco
esclarecedor, tendo em vista a sobreposição de pontos. Assim, a
alternativa foi trabalhar com a distribuição do Conceito Enade Contínuo,
que gerou pontos diversos e, em seguida, utilizar a média do Conceito
Enade Faixa.

Um problema encontrado na resolução da questão 4 diz respeito à
utilização do Conceito Enade Faixa no primeiro gráfico. Desse modo,
visando superar esse obstáculo, foi construído outro gráfico com o
Conceito Enade Contínuo que, devido ao elevado número de cursos e
universidades avaliados, a visualização apresentou grande quantidade de
pontos concentrados em determinado intervalo. Tal pergunta ainda poderia
se desdobrar, caso fosse o objetivo, no sentido de verificar,
especificamente, o cenário de uma universidade específica, curso ou
organização acadêmica, por exemplo. Sendo assim, foi escolhida mais uma
forma de visualização por organização acadêmica, porém vale ressaltar
que várias são as possibilidades de se explorar tais dados.

### 5 REFERÊNCIAS

Brasil. Ministério da Educação - Instituto Nacional de Estudos e
Pesquisas Educacionais Anísio Teixeira (INEP). **Exame Nacional de
Desempenho dos Estudantes (Enade)**. Disponível em:
<http://portal.inep.gov.br/enade>. Acesso em: 18 jul. 2020.
