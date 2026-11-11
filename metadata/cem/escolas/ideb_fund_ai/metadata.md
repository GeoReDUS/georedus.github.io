# Ideb - Fundamental I


## Descrição do indicador

O indicador mostra a nota do Índice de Desenvolvimento da Educação Básica (IDEB) observada no ano de 2022 para os anos iniciais do ensino fundamental de cada escola.

| Indicador | Cálculo | Como ler |
|-----------|-----------|-----------|
| **[Ideb - Fundamental I](https://georedus.github.io/inep-ideb/)** | `vl_observado_ANO` | No município de São Paulo (SP), a escola de código 35000123 obteve a nota 6,5 no IDEB para os anos iniciais do ensino fundamental. |


## Visão Geral

Criado pelo [Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira, o INEP](https://www.gov.br/inep/pt-br), o [Ideb](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/ideb) é um indicador sintético, formulado em 2007, para avaliar diferentes etapas da educação básica (ensinos fundamental e médio). Graças a ele, é possível _monitorar a qualidade do aprendizado nacional e estabelecer metas de melhoria do ensino no Brasil_.

Para isso, conforme exposto na [proposta metodológica](https://download.inep.gov.br/ideb/nota_informativa_ideb_2023.pdf) disponibilizada pelo INEP, o [Ideb](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/ideb) trabalha com duas dimensões essenciais da qualidade educacional: **aprendizagem** e **progressão escolar**. Mais especificamente, as medidas utilizadas, por dimensão, são:

1.  **Fluxo escolar**, dado pela taxa de aprovação obtida a partir do [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar);
2.  **Desempenho acadêmico**, definido a partir das médias de proficiência dos estudantes em língua portuguesa e matemática no [Saeb](https://www.gov.br/inep/pt-br/areas-de-atuacao/avaliacao-e-exames-educacionais/saeb).

Ao integrar esses dois componentes/dimensões, o índice busca reduzir distorções que poderiam surgir caso se considerasse, isoladamente, apenas os resultados de fluxo ou de desempenho.

Note-se, ainda, que: i) o índice adota uma escala de **0 a 10**, com 0 representando o pior cenário e 10 o melhor, ii) os dados podem ser obtidos por escolas, municípios, estados e federação. Por fim, merece ser destacado que o [Ideb](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/ideb) é produzido **bienalmente**, acompanhando o ciclo de aplicação do Saeb.

Nota sobre o Ideb 2021

-   Para uma avaliação temporal/histórica, é importante destacar que:
    
    _“… a interpretação do Ideb, em especial, a oscilação nos valores das suas componentes, precisa ser realizada com cautela. A mudança brusca observada nas taxas de aprovação faz com que a interpretação do Ideb 2021 esteja dissociada da série histórica do rendimento e seja entendida sob a ótica das mudanças sociais, psicológicas e econômicas derivadas da **pandemia de Covid-19**. Ao mesmo tempo, a situação adversa ocasionada pela pandemia de Covid-19 importou em impacto significativo para a aderência à trajetória de metas, estabelecida há 14 anos, em um cenário ausente de fatores exógenos”\* (p. 04)._
    

Para mais detalhes, acesse: [Nota Informativa do Ideb 2021](https://download.inep.gov.br/educacao_basica/portal_ideb/planilhas_para_download/2021/nota_informativa_ideb_2021.pdf).


## Detalhamento metodológico

Deve-se salientar, desde já, que o procedimento proposto gerará dados apenas para as _escolas consideradas ativas_, que são as assim identificadas na base disponibilizada pelo [INEP](https://www.gov.br/inep/pt-br) e que possuem ao menos uma matrícula ativa. As escolas que não apresentaram um código único de identificação também não comporão os resultados finais aqui gerados. Por fim, a seguir apresenta-se o dicionário dos indicadores que serão produzidos. Apenas para fins ilustrativos, adotou-se o ano de 2025 como referência (mais atual no momento de geração do código).

## Fonte dos dados

-   [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar): realizado anualmente, o censo é o principal instrumento de coleta de informações sobre todas as etapas e modalidades da educação básica e profissional; abarca todas as escolas públicas e privadas do país, e, é coordenado pelo Inep e realizado em regime de colaboração entre as secretarias estaduais e municipais de educação.
-   [Sistema de Avaliação da Educação Básica (Saeb)](https://www.gov.br/inep/pt-br/areas-de-atuacao/avaliacao-e-exames-educacionais/saeb): realizado a cada dois anos na rede pública e em uma amostra da rede privada, o SAEB é um conjunto de avaliações externas que busca captar os níveis de aprendizagem dos estudantes avaliados. Dessa forma, ele oferece um indicativo da qualidade do ensino brasileiro, gerando subsídios para a elaboração, o monitoramento e o aprimoramento de políticas educacionais com base em evidências.


**Ano:** 2022

**Repositório de tratamento e processamento de dados:** https://georedus.github.io/inep-ideb/