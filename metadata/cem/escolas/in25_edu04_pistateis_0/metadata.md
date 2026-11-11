# Microdados do Censo Escolar: Infraestrutura (edu04)

**ID da variável:** `in25_edu04_pistateis_0`\
**Ano:** 2025\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/inep-micro-censo-esc/

## Descrição

O indicador (binário) aponta se a escola possui pisos táteis.

**Definição**: Piso caracterizado por textura e cor contrastantes em relação ao piso adjacente, destinado a constituir alerta ou linha-guia, servindo de orientação, principalmente, às pessoas cegas ou com baixa visão. Existem dois tipos de piso tátil: o piso tátil de alerta e o piso tátil direcional. O piso tátil de alerta é conhecido como “piso de bolinha” e sua função é alertar. Esse tipo de piso é instalado em início e término de escadas e rampas, em frente à porta de elevadores, em rampas de acesso às calçadas ou mesmo para alertar quanto a um obstáculo que o deficiente visual não consiga rastrear com a bengala. O outro tipo de piso é o direcional, e sua função é justamente direcionar e orientar sobre o trajeto. Em locais onde não há ponto de referência que possa ser detectado com o uso da bengala, o piso tátil direcional serve como guia.

**Cálculo ou variável de origem:** `in_acessibilidade_pisos_tateis`

**Como ler:**
> *A escola possui pisos táteis (valor 1).*

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
- Dicionário de indicadores (`edu04_pistateis_0`): [Microdados do Censo Escolar](https://georedus.github.io/inep-micro-censo-esc/#dicionário-de-indicadores-que-serão-produzidos)
