# TRTA: Taxas de Rendimento Escolar (Reprovação e Abandono)

**ID da variável:** `in24_edu01_txaba_fn1_0`\
**Ano:** 2024\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/inep-trta/

## Descrição

O indicador mostra a **Taxa de Abandono** para os **anos iniciais** do ensino fundamental da escola, refletindo o percentual de evasão intra-anual.

**Cálculo ou variável de origem:** `x3_cat_fun_ai`

**Como ler:**
> *No município de Manaus (AM), a escola de código 13000123 apresenta uma taxa de abandono de 1,2% nos anos iniciais.*

---

## Visão geral

O presente documento apresenta uma proposta para a obtenção, o tratamento e a disponibilização dos dados das [**Taxas de Rendimento Escolar (Reprovação e Abandono) - TRTA**](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/taxas-de-rendimento-escolar).

Criadas pelo [Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (Inep)](https://www.gov.br/inep/pt-br), as TRTA são construídas a partir dos dados do [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar) e permitem o monitoramento dos dados escolares. Elas também são utilizadas como insumo para a geração do [**Índice de Desenvolvimento da Educação Básica (Ideb)**](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/ideb), um dos mais importantes indicadores educacionais brasileiros.

Em seu cômputo, as [**TRTA**](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/taxas-de-rendimento-escolar) utilizam “… as informações de rendimento e movimento dos alunos coletadas na segunda etapa do Censo Escolar, denominada Situação do Aluno. Nessa etapa, os respondentes preenchem as informações de rendimento (“aprovado” ou “reprovado”), movimento (“falecido”, “deixou de frequentar” ou “transferido”), curso em andamento e sem movimentação dos alunos que foram declarados na Matrícula Inicial do Censo Escolar (primeira etapa)” (INEP, 2021).

Os dados podem ser obtidos por escolas, municípios, estados, regiões e federação. Sublinhe-se, ainda, que por ser gerada a partir do censo escolar, a TRTA apresenta frequência **anual**, disponibilizando, neste momento, dados para o período de 2007 a 2025.

Para mais detalhes, acesse o documento sobre as [TRTA](https://www.gov.br/inep/pt-br/centrais-de-conteudo/acervo-linha-editorial/publicacoes-institucionais/estatisticas-e-indicadores-educacionais/taxas-de-rendimento-escolar).

---

## Fonte dos dados

Os dados utilizados são provenientes do:

-   [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar): realizado anualmente, o censo é o principal instrumento de coleta de informações sobre todas as etapas e modalidades da educação básica e profissional; abarca todas as escolas públicas e privadas do país e é coordenado pelo Inep e realizado em regime de colaboração entre as secretarias estaduais e municipais de educação.

---

## Definições metodológicas

Deve-se salientar, desde já, que o procedimento proposto gerará dados apenas para as _escolas consideradas ativas_, que são as assim identificadas na base disponibilizada pelo [INEP](https://www.gov.br/inep/pt-br) e que possuem ao menos uma matrícula ativa. As escolas que não apresentaram um código único de identificação também não comporão os resultados finais aqui gerados. Por fim, a seguir apresenta-se o dicionário dos indicadores que serão produzidos. Apenas para fins ilustrativos, adotou-se o ano de 2025 como referência (mais atual no momento de geração do código).

---

### 🔗 Links

- Documentação completa do processamento: [TRTA](https://georedus.github.io/inep-trta/)
- Dicionário de indicadores (`edu01_txaba_fn1_0`): [TRTA](https://georedus.github.io/inep-trta/#dicionário-de-indicadores-que-serão-produzidos-trta---taxas-de-rendimento)
