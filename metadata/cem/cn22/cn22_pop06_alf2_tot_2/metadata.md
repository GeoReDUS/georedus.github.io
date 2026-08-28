# Pessoas alfabetizadas de 15 a 19 anos de idade

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \
**Bases de dados:** [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip), [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de pessoas alfabetizadas: 15 a 19 anos (principal)](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L258)** | Porcentagem em relação ao total de pessoas residentes com idade de 15 a 19 anos | $\dfrac{\scriptstyle \mathrm{V00748}}{\scriptstyle \mathrm{V01034}}$ |
| **[Pessoas amarelas: 15 a 19 anos, Cor ou raça é amarela](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L274)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça amarela com idade de 15 a 19 anos | $\dfrac{\scriptstyle \mathrm{V00763}}{\scriptstyle \mathrm{V00659}}$ |
| **[Pessoas brancas: 15 a 19 anos, Cor ou raça é branca](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L272)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça branca com idade de 15 a 19 anos | $\dfrac{\scriptstyle \mathrm{V00761}}{\scriptstyle \mathrm{V00657}}$ |
| **[Pessoas indígenas: 15 a 19 anos, Cor ou raça é indígena](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L275)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça indígena com idade de 15 a 19 anos | $\dfrac{\scriptstyle \mathrm{V00765}}{\scriptstyle \mathrm{V00661}}$ |
| **[Pessoas negras: 15 a 19 anos, Cor ou raça é preta ou parda](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L273)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça negra com idade de 15 a 19 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00762}+\mathrm{V00764}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V00658}+\mathrm{V00660}\end{matrix}}$ |
| **[Mulheres: Sexo feminino, 15 a 19 anos](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L267)** | Porcentagem em relação ao total de pessoas residentes do sexo feminino com idade de 15 a 19 anos | $\dfrac{\scriptstyle \mathrm{V00839}}{\scriptstyle \mathrm{V01023}}$ |
| **[Homens: Sexo masculino, 15 a 19 anos](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L263)** | Porcentagem em relação ao total de pessoas residentes do sexo masculino com idade de 15 a 19 anos | $\dfrac{\scriptstyle \mathrm{V00826}}{\scriptstyle \mathrm{V01012}}$ |

### 📊 Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V00657` | 15 a 19 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00658` | 15 a 19 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00659` | 15 a 19 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00660` | 15 a 19 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00661` | 15 a 19 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00748` | Pessoas alfabetizadas, 15 a 19 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00761` | Pessoas alfabetizadas, 15 a 19 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00762` | Pessoas alfabetizadas, 15 a 19 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00763` | Pessoas alfabetizadas, 15 a 19 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00764` | Pessoas alfabetizadas, 15 a 19 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00765` | Pessoas alfabetizadas, 15 a 19 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00826` | Pessoas alfabetizadas, Sexo masculino, 15 a 19 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00839` | Pessoas alfabetizadas, Sexo feminino, 15 a 19 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V01012` | Sexo masculino, 15 a 19 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01023` | Sexo feminino, 15 a 19 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01034` | 15 a 19 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |

---

## Detalhamento das variáveis

### 📊 Total de pessoas alfabetizadas (principal)

**ID da variável:** `cn22_pop06_alf2_tot_2`\
**Script de processamento:** [cn22_pop06.qmd#L258](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L258)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes com idade de 15 a 19 anos

**Cálculo:** $\dfrac{\scriptstyle \mathrm{V00748}}{\scriptstyle \mathrm{V01034}}$

O indicador mostra a porcentagem de pessoas alfabetizadas, com idade de 15 a 19 anos, em relação ao número total de pessoas com idade de 15 a 19 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Monte das Gameleiras (RN), no setor censitário 240790605000002, 94% das pessoas com idade de 15 a 19 anos são alfabetizadas em 2022.


### 📊 Pessoas amarelas

**ID da variável:** `cn22_pop06_alf2_cor_ama_2`\
**Script de processamento:** [cn22_pop06.qmd#L274](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L274)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça amarela com idade de 15 a 19 anos

**Cálculo:** $\dfrac{\scriptstyle \mathrm{V00763}}{\scriptstyle \mathrm{V00659}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça amarela, com idade de 15 a 19 anos, em relação ao número total de pessoas de cor ou raça amarela com idade de 15 a 19 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de São Paulo (SP), no setor censitário 355031000000000, 75% das pessoas com idade de 15 a 19 anos e de cor ou raça amarela são alfabetizadas em 2022.


### 📊 Pessoas brancas

**ID da variável:** `cn22_pop06_alf2_cor_bra_2`\
**Script de processamento:** [cn22_pop06.qmd#L272](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L272)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça branca com idade de 15 a 19 anos

**Cálculo:** $\dfrac{\scriptstyle \mathrm{V00761}}{\scriptstyle \mathrm{V00657}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça branca, com idade de 15 a 19 anos, em relação ao número total de pessoas de cor ou raça branca com idade de 15 a 19 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Foz do Iguaçu (PR), no setor censitário 410830405000421, 93% das pessoas com idade de 15 a 19 anos e de cor ou raça branca são alfabetizadas em 2022.


### 📊 Pessoas indígenas

**ID da variável:** `cn22_pop06_alf2_cor_ind_2`\
**Script de processamento:** [cn22_pop06.qmd#L275](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L275)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça indígena com idade de 15 a 19 anos

**Cálculo:** $\dfrac{\scriptstyle \mathrm{V00765}}{\scriptstyle \mathrm{V00661}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça indígena, com idade de 15 a 19 anos, em relação ao número total de pessoas de cor ou raça indígena com idade de 15 a 19 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de São Gabriel da Cachoeira (AM), no setor censitário 130381000000000, 36% das pessoas com idade de 15 a 19 anos e de cor ou raça indígena são alfabetizadas em 2022.


### 📊 Pessoas negras

**ID da variável:** `cn22_pop06_alf2_cor_neg_2`\
**Script de processamento:** [cn22_pop06.qmd#L273](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L273)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça negra com idade de 15 a 19 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00762}+\mathrm{V00764}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V00658}+\mathrm{V00660}\end{matrix}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça negra (preta e parda), com idade de 15 a 19 anos, em relação ao número total de pessoas de cor ou raça negra com idade de 15 a 19 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Mogi das Cruzes (SP), no setor censitário 353061000000000, 89% das pessoas com idade de 15 a 19 anos e de cor ou raça negra são alfabetizadas em 2022.


### 📊 Mulheres

**ID da variável:** `cn22_pop06_alf2_sex_f_2`\
**Script de processamento:** [cn22_pop06.qmd#L267](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L267)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes do sexo feminino com idade de 15 a 19 anos

**Cálculo:** $\dfrac{\scriptstyle \mathrm{V00839}}{\scriptstyle \mathrm{V01023}}$

O indicador mostra a porcentagem de pessoas do sexo feminino alfabetizadas, com idade de 15 a 19 anos, em relação ao número total de pessoas do sexo feminino com idade de 15 a 19 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Piracicaba (SP), no setor censitário 353870905000490, 86% das pessoas do sexo feminino com idade de 15 a 19 anos são alfabetizadas em 2022.


### 📊 Homens

**ID da variável:** `cn22_pop06_alf2_sex_m_2`\
**Script de processamento:** [cn22_pop06.qmd#L263](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L263)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes do sexo masculino com idade de 15 a 19 anos

**Cálculo:** $\dfrac{\scriptstyle \mathrm{V00826}}{\scriptstyle \mathrm{V01012}}$

O indicador mostra a porcentagem de pessoas do sexo masculino alfabetizadas, com idade de 15 a 19 anos, em relação ao número total de pessoas do sexo masculino com idade de 15 a 19 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Alta Floresta D’Oeste (RO), no setor censitário 110001525000003, 86% das pessoas do sexo masculino com idade de 15 a 19 anos são alfabetizadas em 2022.


---

## Detalhamento metodológico

As variáveis relativas foram obtidas pela razão entre cada indicador e o total de pessoas da mesma faixa etária no setor censitário. Desse modo, os resultados expressam medidas proporcionais internas a cada grupo etário - por exemplo, o número de pessoas alfabetizadas de 15 a 19 anos em relação ao total de pessoas de 15 a 19 anos no setor. Quando houver recorte de cor ou raça, a abordagem é semelhante, sendo expressas medidas proporcionais internas ao grupo etário e de cor ou raça - por exemplo, o número de pessoas alfabetizadas de 15 a 19 anos e de cor ou raça negra em relação ao total de pessoas de 15 a 19 anos e de cor ou raça negra no setor.

O Censo 2022 do IBGE divulga os resultados a partir de grupos de variáveis, os quais geram arquivos, como “Alfabetização”, “Demografia”, “Parentesco”, entre outros.

Algumas dessas variáveis apresentam a mesma descrição em mais de um arquivo. Por exemplo, a variável “V00645”, do Arquivo “Alfabetização”, e a variável “V01035”, do Arquivo “Demografia”, representam o número de moradores com idade de 20 a 24 anos. Entretanto, para diferentes arquivos, podem ocorrer diferentes agregações de grupos etários - por exemplo, no arquivo “Alfabetização”, a variável “V00647” representa o número de moradores com idade de 30 a 34 anos, porém no arquivo “Demografia”, a variável “V01037” representa o número de moradores com idade de 30 a 39 anos.

Diante disso, neste script, quando houve possibilidade de escolha entre distintas variáveis para obter denominadores de indicadores relativos, optou-se por variáveis com dados de grupos etários mais agregados, portanto, mais abrangentes. Essa escolha visa reduzir os registros identificados pelo IBGE como “dado numérico omitido” (Categoria “X”), que a partir da metodologia adotada, são convertidos em “NA”.

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

- [cn22_pop06.qmd#L258](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L258)
- [cn22_pop06.qmd#L274](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L274)
- [cn22_pop06.qmd#L272](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L272)
- [cn22_pop06.qmd#L275](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L275)
- [cn22_pop06.qmd#L273](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L273)
- [cn22_pop06.qmd#L267](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L267)
- [cn22_pop06.qmd#L263](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L263)

**Download de dados do IBGE**

- [Agregados_por_setores_alfabetizacao_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip)
- [Agregados_por_setores_demografia_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip)

