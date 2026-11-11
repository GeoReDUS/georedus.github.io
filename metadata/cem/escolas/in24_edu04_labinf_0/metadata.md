# Microdados do Censo Escolar: Infraestrutura (edu04)

**ID da variável:** `in24_edu04_labinf_0`\
**Ano:** 2024\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/inep-micro-censo-esc/

## Descrição

O indicador (binário) aponta se a escola possui laboratório de informática.

**Definição**: Local com computadores para uso dos alunos destinado, prioritariamente, ao desenvolvimento de atividades escolares, contribuindo para democratização e universalização do acesso às tecnologias de informação e comunicação (TIC). Os equipamentos também são utilizados como mediação para diversas disciplinas.

**Cálculo ou variável de origem:** `in_laboratorio_informatica`

**Como ler:**
> *A escola possui laboratório de informática (valor 1).*

---

## Visão geral

O presente documento apresenta uma proposta para a obtenção, o tratamento e a disponibilização dos microdados do [**Censo da Educação Básica do Brasil (Censo Escolar)**](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/taxas-de-rendimento-escolar).

Criado pelo [Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (Inep)](https://www.gov.br/inep/pt-br), o [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar) é o principal instrumento de coleta de informações da educação básica e a mais importante pesquisa estatística educacional brasileira. Por meio de seus microdados, ele permite compreender a situação educacional do país, para além de funcionar como a fonte original de diversos indicadores produzidos pelo INEP (Ideb, TDI, TRTA, etc.).

Os dados podem ser obtidos por escolas, municípios, estados, regiões e federação. Sublinhe-se, ainda, que o levantamento é realizado **anualmente** e é **obrigatório para todas as escolas** do país (públicas e privadas).

Para mais detalhes, acesse a página do [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar)

---

## Fonte dos dados

Os dados utilizados no presente documento são provenientes do:

-   [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar): realizado anualmente, o censo é o principal instrumento de coleta de informações sobre todas as etapas e modalidades da educação básica e profissional; abarca todas as escolas públicas e privadas do país e é coordenado pelo Inep e realizado em regime de colaboração entre as secretarias estaduais e municipais de educação.

---

## Definições metodológicas

A seguir, cada um dos indicadores é apresentado em maior detalhe. Expõe-se a descrição de seu cálculo com o nome das variáveis em formato padronizado (por meio do [janitor::clean\_names()](https://sfirke.github.io/janitor/articles/janitor.html)), sua descrição e como se espera que ele seja interpretado. Para facilitar a leitura, eles estão organizados por blocos temáticos, a saber: **Dimensão da Escola (edu02)**, **Serviços Públicos (edu03)**, **Infraestrutura (edu04)** e **Profissionais (edu05)**.

Note, ainda, que as definições fornecidas para os itens foram extraídas do [**Caderno de Conceitos e Orientações do Censo Escolar 2025: 1ª Etapa da Coleta**](https://www.gov.br/inep/pt-br/centrais-de-conteudo/acervo-linha-editorial/publicacoes-institucionais/estatisticas-e-indicadores-educacionais/caderno-de-conceitos-e-orientacoes-do-censo-escolar-2025-1a-etapa-da-coleta). Esse material é disponibilizado pelo [Inep](https://www.gov.br/inep/pt-br) e tem como objetivo orientar os responsáveis pela declaração e pelo acompanhamento da coleta do Censo Escolar.

---

### 🔗 Links

- Documentação completa do processamento: [Microdados do Censo Escolar](https://georedus.github.io/inep-micro-censo-esc/)
- Dicionário de indicadores (`edu04_labinf_0`): [Microdados do Censo Escolar](https://georedus.github.io/inep-micro-censo-esc/#dicionário-de-indicadores-que-serão-produzidos)
