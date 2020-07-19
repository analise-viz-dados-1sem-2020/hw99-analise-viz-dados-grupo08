Trabalho Final
================
Gabriela Silva, Guilherme Amalisis, Melissa Dias e Mylena Dias
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
    (concluintes participantes/concluintes inscritos) e o conceito Enade
    faixa?

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
    ##  $ Conceito Enade (Faixa)          : chr [1:8821] "5" "3" "4" "4" ...
    ##  $ Observação                      : logi [1:8821] NA NA NA NA NA NA ...

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

### Considerações finais

### Referências

Brasil. Ministério da Educação - Instituto Nacional de Estudos e
Pesquisas Educacionais Anísio Teixeira (INEP). **Exame Nacional de
Desempenho dos Estudantes (Enade)**. Disponível em:
<http://portal.inep.gov.br/enade>. Acesso em: 18 jul. 2020.
