# Inse


## Descrição do indicador

O indicador mostra a média contínua do Indicador de Nível Socioeconômico (Inse) da escola.

| Indicador | Cálculo | Como ler |
|-----------|-----------|-----------|
| **[Inse](https://georedus.github.io/inep-inse/)** | `media_inse` | No município de Recife (PE), a escola de código 26000123 apresenta um Inse médio de 5,12. |


## Visão Geral

Criado pelo [Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (Inep)](https://www.gov.br/inep/pt-br), o [Inse](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/nivel-socioeconomico) é uma medida sintética construída a partir dos questionários do **Saeb** e tem como objetivo “traçar um panorama da realidade social de escolas e redes de ensino a partir do perfil dos alunos, além de produzir evidências para auxiliar na implementação, no monitoramento e na avaliação de políticas públicas voltadas à educação” ([INEP](https://www.gov.br/inep/pt-br/centrais-de-conteudo/noticias/saeb/indicador-de-nivel-socioeconomico-do-saeb-disponivel))

Para o seu cômputo, o índice considera **a escolaridade dos responsáveis**, bem como **a posse de bens** e **o acesso a serviços no domicílio dos estudantes**. A partir desses fatores, as estimativas do Inse são produzidas por meio de modelagem estatística baseada na Teoria de Resposta ao Item (TRI).

O resultado obtido é uma medida contínua, posteriormente classificada em oito níveis (I a VIII). Ressalte-se, também, que os dados podem ser obtidos por escolas, municípios, estados e federação. Por fim, merece ser mencionado que o [Inse](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/nivel-socioeconomico), assim como o Ideb, é produzido **bienalmente**, acompanhando o ciclo de aplicação do Saeb.

Para mais detalhes, acesse as [Notas Técnicas do Inse](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/nivel-socioeconomico).

Observação:

De acordo com a nota técnica do índice produzida em 2023 pelo INEP, é importante destacar que, a rigor, o [Inse](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/nivel-socioeconomico)

_“… não é um índice de desigualdade, pois seu produto primário são os escores dos estudantes agrupados em determinados níveis de análise, e não uma distância entre pontuações de extremos (ou seja, uma medida de variabilidade ou dispersão) representada em um valor. Estudos nessa direção, no entanto, podem ser planejados e desenvolvidos, já que o delineamento metodológico do Inse do Saeb permite a comparação de resultados entre anos”._


## Detalhamento metodológico

Deve-se salientar, desde já, que o procedimento proposto gerará dados apenas para as _escolas consideradas ativas_, que são as assim identificadas na base disponibilizada pelo [INEP](https://www.gov.br/inep/pt-br) e que possuem ao menos uma matrícula ativa. As escolas que não apresentaram um código único de identificação também não comporão os resultados finais aqui gerados.

## Fonte dos dados

-   [Sistema de Avaliação da Educação Básica (Saeb)](https://www.gov.br/inep/pt-br/areas-de-atuacao/avaliacao-e-exames-educacionais/saeb): realizado a cada dois anos na rede pública e em uma amostra da rede privada, o SAEB é um conjunto de avaliações externas que busca captar os níveis de aprendizagem dos estudantes avaliados. Dessa forma, ele oferece um indicativo da qualidade do ensino brasileiro, gerando subsídios para a elaboração, o monitoramento e o aprimoramento de políticas educacionais com base em evidências.


**Ano:** 2022

**Repositório de tratamento e processamento de dados:** https://georedus.github.io/inep-inse/