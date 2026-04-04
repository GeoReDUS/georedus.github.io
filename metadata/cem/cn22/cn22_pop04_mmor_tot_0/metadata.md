# Moradores por domicílio

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \
**Bases de dados:** [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de moradores: Média de moradores em domicílios particulares permanentes ocupados (principal)](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop04.qmd#L140)** | Média de moradores por domicílio | $\mathrm{V0005}$ |

### Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V0005` | Média de moradores em Domicílios Particulares Ocupados (Total pessoas em Domicílios Particulares Ocupados / DPPO + DPIO) | [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip) |

---

## Detalhamento das variáveis

### Total de moradores (principal)

**ID da variável:** `cn22_pop04_mmor_tot_0`\
**Script de processamento:** [cn22_pop04.qmd#L140](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop04.qmd#L140)\
**Unidade de medida:** Média de moradores por domicílio

**Cálculo:** $\mathrm{V0005}$

O indicador mostra a média de moradores residentes em Domicílios Particulares Ocupados (DPO) em cada setor censitário, a partir dos dados do Censo Demográfico de 2022 do IBGE. O valor é obtido pela razão entre o total de pessoas residentes em DPO e o número total de DPO no setor censitário.

**Exemplo**:
> No município de Gravataí (RS), no setor censitário 430920905000244, foram registrados 785 moradores residindo em domicílios particulares e 292 domicílios particulares ocupados. Ao relacionar o total de moradores ao número de domicílios particulares ocupados, obtém-se uma média de 2,7 moradores por domicílio.


---

## Detalhamento metodológico

Atualmente, o conjunto de indicadores relativos ao grupo pop04 (Moradores por domicílio) é composto por um único indicador, correspondente à própria variável pop04. Esse indicador deriva diretamente da variável V0005 do Censo 2022, que representa o número médio de moradores residentes por domicílio. Dessa forma, não há necessidade de construção adicional de métricas relativas, uma vez que a variável já expressa, em sua forma original, a relação entre população residente e domicílios.

---

## Referências

### Base Cartográfica

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

### Referências Bibliográficas

INSTITUTO BRASILEIRO DE GEOGRAFIA E ESTATÍSTICA (IBGE). _Censo Demográfico 2022 - Malha de setores censitários_. Rio de Janeiro: IBGE, 2024. Disponível em: <https://biblioteca.ibge.gov.br/index.php/biblioteca-catalogo?view=detalhes&id=2102138>. Acesso em: 20 out. 2025.

**\_\_**. _Censo Demográfico 2022 - Dicionário de dados da Malha de Setores Censitários – Agregados por Setores Censitários_. Rio de Janeiro: IBGE, 2024. Disponível em: <https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/malha_com_atributos/Dicionario_de_dados_malha_agregados.xlsx>. Acesso em: 20 out. 2025.

**\_\_**. _Quadro geográfico de referência para produção, análise e disseminação de estatísticas_. 2. ed. Rio de Janeiro: IBGE, 2022. Disponível em: <https://biblioteca.ibge.gov.br/index.php/biblioteca-catalogo?view=detalhes&id=2101962>. Acesso em: 20 out. 2025.

**\_\_**. _Unidades de coleta e divulgação de pesquisa: Setor Censitário_. Rio de Janeiro: IBGE, 2022. Disponível em: <https://www.ibge.gov.br/apps/quadrogeografico/pdf/qg_2022_600_setcensitario.pdf>. Acesso em: 01 abr. 2026.


### Links
**Scripts GeoReDUS**

- [cn22_pop04.qmd#L140](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop04.qmd#L140)

**Download de dados do IBGE**

- [Agregados_por_setores_basico_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

