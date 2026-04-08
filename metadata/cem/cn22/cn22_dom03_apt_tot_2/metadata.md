# Domicílios tipo apartamento

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-dom \
**Bases de dados:** [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip), [Domicílios 3](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de domicílios: Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento (principal)](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L222)** | Porcentagem em relação ao total de domicílios | $\dfrac{\mathrm{V00049}}{\mathrm{V00001}}$ |
| **[Mulheres: Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento, Pessoas de sexo feminino no domicílio](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L225)** | Porcentagem em relação ao total de mulheres residentes | $\dfrac{\mathrm{V00507}}{\mathrm{V00014}}$ |
| **[Homens: Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento, Pessoas de sexo masculino no domicílio](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L224)** | Porcentagem em relação ao total de homens residentes | $\dfrac{\mathrm{V00504}}{\mathrm{V00011}}$ |
| **[Total de moradores: Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento, Quantidade de moradores](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L223)** | Porcentagem em relação ao total de moradores | $\dfrac{\mathrm{V00086}}{\mathrm{V00005}}$ |

### 📊 Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V00001` | Domicílios Particulares Permanentes Ocupados | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00005` | Domicílios Particulares Permanentes Ocupados, Quantidade de moradores | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00011` | Domicílios Particulares Permanentes Ocupados, Pessoas de sexo masculino no domicílio | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00014` | Domicílios Particulares Permanentes Ocupados, Pessoas de sexo feminino no domicílio | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00049` | Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00086` | Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento, Quantidade de moradores | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00504` | Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento, Pessoas de sexo masculino no domicílio | [Domicílios 3](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip) |
| `V00507` | Domicílios Particulares Permanentes Ocupados, Tipo de espécie é apartamento, Pessoas de sexo feminino no domicílio | [Domicílios 3](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip) |

---

## Detalhamento das variáveis

### 📊 Total de domicílios (principal)

**ID da variável:** `cn22_dom03_apt_tot_2`\
**Script de processamento:** [cn22_dom.qmd#L222](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L222)\
**Unidade de medida:** Porcentagem em relação ao total de domicílios

**Cálculo:** $\dfrac{\mathrm{V00049}}{\mathrm{V00001}}$

O indicador mostra a porcentagem de domicílios tipo apartamento em relação ao total de domicílios particulares permanentes ocupados, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Natal (RN), no setor censitário 240810205080070, 87% dos domicílios particulares permanentes ocupados são do tipo apartamento.


### 📊 Mulheres

**ID da variável:** `cn22_dom03_apt_sex_f_2`\
**Script de processamento:** [cn22_dom.qmd#L225](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L225)\
**Unidade de medida:** Porcentagem em relação ao total de mulheres residentes

**Cálculo:** $\dfrac{\mathrm{V00507}}{\mathrm{V00014}}$

O indicador mostra a porcentagem de moradores do sexo feminino residentes em domicílios tipo apartamento em relação ao total de moradores do sexo feminino residentes em domicílios particulares permanentes ocupados, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Pelotas (RS), no setor censitário 431440705130103, 78% dos moradores do sexo feminino residentes em domicílios particulares permanentes ocupados residem em apartamentos.


### 📊 Homens

**ID da variável:** `cn22_dom03_apt_sex_m_2`\
**Script de processamento:** [cn22_dom.qmd#L224](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L224)\
**Unidade de medida:** Porcentagem em relação ao total de homens residentes

**Cálculo:** $\dfrac{\mathrm{V00504}}{\mathrm{V00011}}$

O indicador mostra a porcentagem de moradores do sexo masculino residentes em domicílios tipo apartamento em relação ao total de moradores do sexo masculino residentes em domicílios particulares permanentes ocupados, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Osasco (SP), no setor censitário 353440105001159, 88% dos moradores do sexo masculino residentes em domicílios particulares permanentes ocupados residem em apartamentos.


### 📊 Total de moradores

**ID da variável:** `cn22_dom03_apt_tot_mor_2`\
**Script de processamento:** [cn22_dom.qmd#L223](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L223)\
**Unidade de medida:** Porcentagem em relação ao total de moradores

**Cálculo:** $\dfrac{\mathrm{V00086}}{\mathrm{V00005}}$

O indicador mostra a porcentagem de moradores residentes em domicílios tipo apartamento em relação ao total de moradores residentes em domicílios particulares permanentes ocupados, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Santarém (PA), no setor censitário 150680705000651, 24% dos moradores residentes em domicílios particulares permanentes ocupados residem em apartamentos.


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

- [cn22_dom.qmd#L222](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L222)
- [cn22_dom.qmd#L225](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L225)
- [cn22_dom.qmd#L224](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L224)
- [cn22_dom.qmd#L223](https://github.com/GeoReDUS/cn22-dom/blob/main/r/cn22_dom.qmd#L223)

**Download de dados do IBGE**

- [Agregados_por_setores_caracteristicas_domicilio1_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip)
- [Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip)

