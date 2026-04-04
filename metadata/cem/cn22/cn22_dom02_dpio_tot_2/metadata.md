# Domicílios improvisados

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-dom \
**Bases de dados:** [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de domicílios: Domicílios Particulares Improvisados Ocupados (principal)](#cn22_dom02_dpio_tot_2)**<br/> | Porcentagem em relação ao total de domicílios | $\dfrac{\mathrm{V00002}}{\mathrm{V00001} + \mathrm{V00002} + \mathrm{V00003}}$ |

### Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V00001` | Domicílios Particulares Permanentes Ocupados | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00002` | Domicílios Particulares Improvisados Ocupados | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00003` | Unidades de Habitação em Domicílios Coletivos Com Morador | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |

---

## Detalhamento das variáveis

### Total de domicílios (principal) {#cn22_dom02_dpio_tot_2}

**ID da variável:** `cn22_dom02_dpio_tot_2`\
**Unidade de medida:** Porcentagem em relação ao total de domicílios

**Cálculo:** $\dfrac{\mathrm{V00002}}{\mathrm{V00001} + \mathrm{V00002} + \mathrm{V00003}}$

O indicador mostra a porcentagem de domicílios particulares improvisados ocupados em relação ao total de domicílios ocupados em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de João Pessoa (PB), no setor censitário 250750705000140, 15% dos domicílios ocupados são particulares improvisados.

**Script de processamento:** [cn22_dom.qmd#L213](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L213)

---

## Detalhamento metodológico

-   **Unidade territorial:** os indicadores são calculados na escala do setor censitário, identificado pelo código oficial `cd_setor`.
    
-   **Tratamento da categoria “X”:** registros identificados pelo IBGE como “dado numérico omitido” são convertidos para `NA` antes do processamento. [`Documento acessível aqui`](https://biblioteca.ibge.gov.br/index.php/biblioteca-catalogo?view=detalhes&id=2102138)
    
-   **Indicadores absolutos:** a soma de variáveis utiliza a função interna `safe_row_sum()`, com as seguintes regras:
    
    -   valor numérico + `NA` → retorna o valor numérico;
    -   todos os valores `NA` → retorna `NA`.
-   **Indicadores relativos:** as proporções são calculadas com a função interna `safe_divide()`, que:
    
    -   retorna `NA` quando o denominador é `0` ou `NA`;
    -   evita a geração de valores `NaN` ou `Inf`.

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

- [cn22_dom.qmd#L213](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L213)

**Download de dados do IBGE**

- [Agregados_por_setores_caracteristicas_domicilio1_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip)

