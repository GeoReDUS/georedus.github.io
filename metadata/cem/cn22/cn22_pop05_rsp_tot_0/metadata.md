# Renda das pessoas responsáveis

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Renda das pessoas responsáveis: Valor do rendimento nominal médio mensal das pessoas responsáveis com rendimentos por domicílios particulares permanentes ocupados (principal)](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop05.qmd#L140)** | Renda média mensal das pessoas responsáveis | $\mathrm{V06004}$ |

---

## Detalhamento das variáveis

### 📊 Renda das pessoas responsáveis (principal)

**ID da variável:** `cn22_pop05_rsp_tot_0`\
**Script de processamento:** [cn22_pop05.qmd#L140](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop05.qmd#L140)\
**Unidade de medida:** Renda média mensal das pessoas responsáveis

**Cálculo:** $\mathrm{V06004}$

O indicador mostra o valor do rendimento nominal médio mensal das pessoas responsáveis com rendimentos por Domicílios Particulares Permanentes Ocupados em cada setor censitário, a partir dos dados do Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Pindamonhangaba (SP), no setor censitário 353800605000365, a renda média mensal das pessoas responsáveis com rendimento é de R$ 4394.96 em 2022.


---

## Detalhamento metodológico

Atualmente, o conjunto de indicadores relativos ao grupo pop05 (Rendimento) é composto por um único indicador, correspondente à própria variável pop05. Esse indicador deriva diretamente da variável V06004 do Censo 2022, que representa o valor do rendimento nominal médio mensal das pessoas responsáveis com rendimentos por domicílios particulares permanentes ocupados. Dessa forma, não há necessidade de construção adicional de métricas relativas.

---

## Referências

### 🗺️ Base Cartográfica

**Nome:** [Setor Censitário (Censo Demográfico) – 2022](https://metadadosgeo.ibge.gov.br/geonetwork_ibge/srv/por/catalog.search#/metadata/da590223-27dc-4254-8cf4-5d67f55bc64d)\
**Responsável:** [Instituto Brasileiro de Geografia e Estatística (IBGE)](https://www.ibge.gov.br/)

#### Características Técnicas

| Atributo               | Valor                   |
| ---------------------- | ----------------------- |
| Representação espacial | Vetor                   |
| Escala                 | 1:250.000               |
| Sistema de referência  | SIRGAS 2000 (EPSG:4674) |
| Codificação            | UTF-8                   |

A escala de referência de 1:250.000 reflete a escala de trabalho adotada para a malha nacional. Na prática, a dimensão dos setores censitários varia conforme a situação territorial: em áreas urbanas, os setores tendem a apresentar menor extensão e maior densidade demográfica; em áreas rurais, maior extensão e população esparsa (IBGE, [Quadro Geográfico de Referência, 2022](https://www.ibge.gov.br/apps/quadrogeografico/pdf/qg_2022_600_setcensitario.pdf)). Essa variação implica que a precisão geoespacial efetiva é consideravelmente maior nas áreas urbanas do que a escala nominal sugere.

#### Extensão Geográfica

Todo o território brasileiro

| Limite | Valor      |
| ------ | ---------- |
| Oeste  | -73,99044° |
| Leste  | -28,84763° |
| Sul    | -33,75117° |
| Norte  | 5,271841°  |

---

### 📚 Referências Bibliográficas

INSTITUTO BRASILEIRO DE GEOGRAFIA E ESTATÍSTICA (IBGE). _Censo Demográfico 2022 - Malha de setores censitários_. Rio de Janeiro: IBGE, 2024. Disponível em: <https://biblioteca.ibge.gov.br/index.php/biblioteca-catalogo?view=detalhes&id=2102138>. Acesso em: 20 out. 2025.

**\_\_**. _Censo Demográfico 2022 - Dicionário de dados da Malha de Setores Censitários – Agregados por Setores Censitários_. Rio de Janeiro: IBGE, 2024. Disponível em: <https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/malha_com_atributos/Dicionario_de_dados_malha_agregados.xlsx>. Acesso em: 20 out. 2025.

**\_\_**. _Quadro geográfico de referência para produção, análise e disseminação de estatísticas_. 2. ed. Rio de Janeiro: IBGE, 2022. Disponível em: <https://biblioteca.ibge.gov.br/index.php/biblioteca-catalogo?view=detalhes&id=2101962>. Acesso em: 20 out. 2025.

**\_\_**. _Unidades de coleta e divulgação de pesquisa: Setor Censitário_. Rio de Janeiro: IBGE, 2022. Disponível em: <https://www.ibge.gov.br/apps/quadrogeografico/pdf/qg_2022_600_setcensitario.pdf>. Acesso em: 01 abr. 2026.


### 🔗 Links
**Scripts GeoReDUS**

- [cn22_pop05.qmd#L140](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop05.qmd#L140)

