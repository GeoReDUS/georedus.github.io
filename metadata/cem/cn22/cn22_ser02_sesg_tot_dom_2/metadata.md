# Domicílios sem destinação do esgoto por rede geral ou pluvial

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-ser \
**Bases de dados:** [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip), [Domicílios 2](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio2_BR_20250417.zip), [Domicílios 3](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de domicílios: Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial (principal)](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L256)** | Porcentagem em relação ao total de domicílios | $\dfrac{\mathrm{V00001} - \mathrm{V00309}}{\mathrm{V00001}}$ |
| **[Mulheres: Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial, Pessoas de sexo feminino no domicílio](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L266)** | Porcentagem em relação ao total de mulheres nos domicílios | $\dfrac{\mathrm{V00014} - \mathrm{V00604}}{\mathrm{V00014}}$ |
| **[Total de moradores: Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial, Quantidade de moradores](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L259)** | Porcentagem em relação ao total de moradores | $\dfrac{\mathrm{V00005} - \mathrm{V00580}}{\mathrm{V00005}}$ |
| **[Homens: Domicílios Particulares Permanentes Ocupados, Destinação do esgoto inexistente, pois não tinham banheiro nem sanitário, Pessoas de sexo masculino no domicílio OU Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial, Pessoas de sexo masculino no domicílio](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L263)** | Porcentagem em relação ao total de homens nos domicílios | $\dfrac{\mathrm{V00011} - \mathrm{V00596}}{\mathrm{V00011}}$ |

### Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V00001` | Domicílios Particulares Permanentes Ocupados | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00005` | Domicílios Particulares Permanentes Ocupados, Quantidade de moradores | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00011` | Domicílios Particulares Permanentes Ocupados, Pessoas de sexo masculino no domicílio | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00014` | Domicílios Particulares Permanentes Ocupados, Pessoas de sexo feminino no domicílio | [Domicílios 1](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip) |
| `V00309` | Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial | [Domicílios 2](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio2_BR_20250417.zip) |
| `V00580` | Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial, Quantidade de moradores | [Domicílios 3](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip) |
| `V00596` | Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial, Pessoas de sexo masculino no domicílio | [Domicílios 3](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip) |
| `V00604` | Domicílios Particulares Permanentes Ocupados, Destinação do esgoto do banheiro ou sanitário ou buraco para dejeções é rede geral ou pluvial, Pessoas de sexo feminino no domicílio | [Domicílios 3](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip) |

---

## Detalhamento das variáveis

### Total de domicílios (principal)

**ID da variável:** `cn22_ser02_sesg_tot_dom_2`\
**Script de processamento:** [cn22_ser.qmd#L256](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L256)\
**Unidade de medida:** Porcentagem em relação ao total de domicílios

**Cálculo:** $\dfrac{\mathrm{V00001} - \mathrm{V00309}}{\mathrm{V00001}}$

O indicador mostra a porcentagem de domicílios particulares permanentes ocupados (DPPO) sem destinação de esgoto por rede geral ou pluvial em relação ao total de DPPO, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Sorocaba (SP), no setor censitário 355220505000722, 29% dos domicílios particulares permanentes ocupados não possuem destinação de esgoto por rede geral ou pluvial.


### Mulheres

**ID da variável:** `cn22_ser02_sesg_sex_f_2`\
**Script de processamento:** [cn22_ser.qmd#L266](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L266)\
**Unidade de medida:** Porcentagem em relação ao total de mulheres nos domicílios

**Cálculo:** $\dfrac{\mathrm{V00014} - \mathrm{V00604}}{\mathrm{V00014}}$

O indicador mostra a porcentagem de moradores do sexo feminino residentes em domicílios particulares permanentes ocupados (DPPO) sem destinação de esgoto por rede geral ou pluvial em relação ao total de moradores do sexo feminino residentes em DPPO, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Ilhéus (BA), no setor censitário 291360605000272, 42% dos moradores do sexo feminino residentes em domicílios particulares permanentes ocupados residem em domicílios que não possuem destinação de esgoto por rede geral ou pluvial.


### Total de moradores

**ID da variável:** `cn22_ser02_sesg_tot_mor_2`\
**Script de processamento:** [cn22_ser.qmd#L259](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L259)\
**Unidade de medida:** Porcentagem em relação ao total de moradores

**Cálculo:** $\dfrac{\mathrm{V00005} - \mathrm{V00580}}{\mathrm{V00005}}$

O indicador mostra a porcentagem de moradores residentes em domicílios particulares permanentes ocupados (DPPO) sem destinação de esgoto por rede geral ou pluvial em relação ao total de moradores residentes em DPPO, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Santa Cruz do Sul (RS), no setor censitário 431680805000155, 74% dos moradores residentes em domicílios particulares permanentes ocupados residem em domicílios que não possuem destinação de esgoto por rede geral ou pluvial.


### Homens

**ID da variável:** `cn22_ser02_sesg_sex_m_2`\
**Script de processamento:** [cn22_ser.qmd#L263](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L263)\
**Unidade de medida:** Porcentagem em relação ao total de homens nos domicílios

**Cálculo:** $\dfrac{\mathrm{V00011} - \mathrm{V00596}}{\mathrm{V00011}}$

O indicador mostra a porcentagem de moradores do sexo masculino residentes em domicílios particulares permanentes ocupados (DPPO) sem destinação de esgoto por rede geral ou pluvial em relação ao total de moradores do sexo masculino residentes em DPPO, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Tangará da Serra (MT), no setor censitário 510795805000010, 24% dos moradores do sexo masculino residentes em domicílios particulares permanentes ocupados residem em domicílios que não possuem destinação de esgoto por rede geral ou pluvial.


---

## Detalhamento metodológico

-   **Unidade territorial:** os indicadores são calculados na escala do setor censitário, identificado pelo código oficial `cd_setor`.
    
-   **Tratamento da categoria “X”:** registros identificados pelo IBGE como “dado numérico omitido” são convertidos para `NA` antes do processamento, passando a obedecer às regras de agregação acima. [Documento acessível aqui](https://biblioteca.ibge.gov.br/index.php/biblioteca-catalogo?view=detalhes&id=2102138)
    
-   **Indicadores absolutos:** a soma de variáveis utiliza a função interna `safe_row_sum()`, com as seguintes regras:
    
    -   valor numérico + `NA` → retorna o valor numérico;
    -   todos os valores `NA` → retorna `NA`.
-   **Indicadores relativos:** as proporções são calculadas com a função interna `safe_divide()`, que:
    
    -   retorna `NA` quando o denominador é `0` ou `NA`;
    -   evita a geração de valores `NaN` ou `Inf`.
-   **Geração de indicadores:** as variáveis relativas foram obtidas pela divisão dos indicadores por um dos seguintes:
    
    -   total de domicílios particulares permanentes ocupados (V00001), denominada neste trabalho `cn_22_dom02_dppo_tot_0`, resultando em medidas proporcionais ao total de domicílios particulares permanentes ocupados do setor;
    -   quantidade total de moradores em domicílios particulares permanentes ocupados (V00005), denominada neste trabalho `cn_22_dom02_dppo_tot_mor_0`, resultando em medidas proporcionais ao total de moradores em domicílios particulares permanentes ocupados do setor;
    -   quantidade total de moradores do sexo masculino em domicílios particulares permanentes ocupados (V00011), denominada neste trabalho `cn_22_dom02_dppo_sex_m_0`, resultando em medidas proporcionais ao total de moradores do sexo masculino em domicílios particulares permanentes ocupados do setor;
    -   quantidade total de moradores do sexo feminino em domicílios particulares permanentes ocupados (V00014), denominada neste trabalho `cn_22_dom02_dppo_sex_f_0`, resultando em medidas proporcionais ao total de moradores do sexo feminino em domicílios particulares permanentes ocupados do setor.

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

- [cn22_ser.qmd#L256](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L256)
- [cn22_ser.qmd#L266](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L266)
- [cn22_ser.qmd#L259](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L259)
- [cn22_ser.qmd#L263](https://github.com/GeoReDUS/cn22-ser/blob/main/r/cn22_ser.qmd#L263)

**Download de dados do IBGE**

- [Agregados_por_setores_caracteristicas_domicilio1_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio1_BR.zip)
- [Agregados_por_setores_caracteristicas_domicilio2_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio2_BR_20250417.zip)
- [Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_caracteristicas_domicilio3_BR_20250417.zip)

