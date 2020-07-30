Trabalho Final
================
Gabriela Silva, Guilherme Amasilis, Melissa Dias e Mylena Dias
18/07/2020

### Introdução

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

<!-- end list -->

    ## tibble [8,821 × 22] (S3: tbl_df/tbl/data.frame)
    ##  $ Ano                             : num [1:8821] 2018 2018 2018 2018 2018 ...
    ##  $ Código da Área                  : num [1:8821] 2 13 38 22 1 22 13 38 81 1 ...
    ##  $ Área de Avaliação               : chr [1:8821] "DIREITO" "CIÊNCIAS ECONÔMICAS" "SERVIÇO SOCIAL" "CIÊNCIAS CONTÁBEIS" ...
    ##  $ Código da IES                   : num [1:8821] 1 1 1 1 1 1 2 2 2 2 ...
    ##  $ Nome da IES                     : chr [1:8821] "UNIVERSIDADE FEDERAL DE MATO GROSSO" "UNIVERSIDADE FEDERAL DE MATO GROSSO" "UNIVERSIDADE FEDERAL DE MATO GROSSO" "UNIVERSIDADE FEDERAL DE MATO GROSSO" ...
    ##  $ Sigla da IES                    : chr [1:8821] "UFMT" "UFMT" "UFMT" "UFMT" ...
    ##  $ Organização Acadêmica           : chr [1:8821] "Universidade" "Universidade" "Universidade" "Universidade" ...
    ##  $ Categoria Administrativa        : chr [1:8821] "Pessoa Jurídica de Direito Público - Federal" "Pessoa Jurídica de Direito Público - Federal" "Pessoa Jurídica de Direito Público - Federal" "Pessoa Jurídica de Direito Público - Federal" ...
    ##  $ Código do Curso                 : num [1:8821] 1 2 7 8 13 21 122 126 128 145 ...
    ##  $ Modalidade de Ensino            : chr [1:8821] "Educação Presencial" "Educação Presencial" "Educação Presencial" "Educação Presencial" ...
    ##  $ Código do Município             : num [1:8821] 5103403 5103403 5103403 5103403 5103403 ...
    ##  $ Município do Curso              : chr [1:8821] "CUIABA" "CUIABA" "CUIABA" "CUIABA" ...
    ##  $ Sigla da UF                     : chr [1:8821] "MT" "MT" "MT" "MT" ...
    ##  $ Nº de Concluintes Inscritos     : num [1:8821] 82 29 32 75 122 54 113 91 158 274 ...
    ##  $ Nº  de Concluintes Participantes: num [1:8821] 72 23 22 66 101 49 92 81 134 189 ...
    ##  $ Nota Bruta - FG                 : num [1:8821] 68.4 57.6 48.8 54.4 53.4 ...
    ##  $ Nota Padronizada - FG           : num [1:8821] 4.73 3.2 3.27 4.36 3.81 ...
    ##  $ Nota Bruta - CE                 : num [1:8821] 50.3 31 54.8 41.9 44.9 ...
    ##  $ Nota Padronizada - CE           : num [1:8821] 4.02 1.84 3.46 3.25 3.64 ...
    ##  $ Conceito Enade (Contínuo)       : num [1:8821] 4.2 2.18 3.41 3.53 3.68 ...
    ##  $ Conceito Enade (Faixa)          : num [1:8821] 5 3 4 4 4 3 5 5 4 5 ...
    ##  $ Observação                      : chr [1:8821] NA NA NA NA ...

### Descrição da base de dados

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

Além disso, a presente base de dados fornece informações que abarcam a
área de avaliação, o nome da Instituição de Ensino Superior (IES), o
município do curso, a organização acadêmica, o Conceito Enade Faixa,
dentre outras importantes dimensões e métricas para a conformação do
panorama de qualidade do Ensino Superior no Brasil.

### Análise Exploratória

A segunda pergunta analisada questiona acerca de como se dá a
distribuição do Conceito Enade (Faixa) para os cursos avaliados da
Universidade Federal de Minas Gerais (UFMG). O gráfico obtido a partir
da manipulação dos dados encontra-se a seguir:

![Figura 2: Conceito Enade UFMG](/cloud/project/distribuicao_ufmg.jpg)
Figura 2: Conceito Enade UFMG

A base de dados apresenta o Conceito Enade (Faixa) para doze diferentes
áreas de avaliação: Administração (Campus Belo Horizonte),
Administração (Campus Montes Claros), Administração Pública, Ciências
Contábeis, Ciências Econômicas, Comunicação Social – Jornalismo,
Comunicação Social – Publicidade e Propaganda, Design, Direito,
Psicologia, Relações Internacionais e Turismo. Destes, 8 cursos (66,67%)
obtiveram nota máxima (5) no conceito Enade, enquanto os outros 4 cursos
(33,33%) obtiveram nota 4. Dessa forma, observa-se que a UFMG alcançou
notas altas na avaliação realizada.

### Considerações finais

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

### Referências

Brasil. Ministério da Educação - Instituto Nacional de Estudos e
Pesquisas Educacionais Anísio Teixeira (INEP). **Exame Nacional de
Desempenho dos Estudantes (Enade)**. Disponível em:
<http://portal.inep.gov.br/enade>. Acesso em: 18 jul. 2020.
