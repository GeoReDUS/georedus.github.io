# Pessoas residentes

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Bases de dados:** [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip), [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip), [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **Total de residentes: Quantidade de moradores (principal)** | Pessoas residentes por km² | — |
| **[Pessoas amarelas: Cor ou raça é amarela](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01319}}{\mathrm{V0001}}$ |
| **[Pessoas brancas: Cor ou raça é branca](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01317}}{\mathrm{V0001}}$ |
| **[Pessoas indígenas: Cor ou raça é indígena](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01321}}{\mathrm{V0001}}$ |
| **[Pessoas negras: Cor ou raça é preta ou parda](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01318}+\mathrm{V01320}}{\mathrm{V0001}}$ |
| **[Mulheres: Sexo feminino](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01008}}{\mathrm{V0001}}$ |
| **[Mulheres amarelas: Sexo feminino, Cor ou raça é amarela](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01329}}{\mathrm{V0001}}$ |
| **[Mulheres brancas: Sexo feminino, Cor ou raça é branca](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01327}}{\mathrm{V0001}}$ |
| **[Mulheres indígenas: Sexo feminino, Cor ou raça é indígena](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01331}}{\mathrm{V0001}}$ |
| **[Mulheres negras: Sexo feminino, Cor ou raça é preta ou parda](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01328}+\mathrm{V01330}}{\mathrm{V0001}}$ |
| **[Homens: Sexo masculino](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01007}}{\mathrm{V0001}}$ |
| **[Homens amarelos: Sexo masculino, Cor ou raça é amarela](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01324}}{\mathrm{V0001}}$ |
| **[Homens brancos: Sexo masculino, Cor ou raça é branca](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01322}}{\mathrm{V0001}}$ |
| **[Homens indígenas: Sexo masculino, Cor ou raça é indígena](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01326}}{\mathrm{V0001}}$ |
| **[Homens negros: Sexo masculino, Cor ou raça é preta ou parda](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01323}+\mathrm{V01325}}{\mathrm{V0001}}$ |

### 📊 Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V0001` | Total de pessoas | [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip) |
| `V01007` | Sexo masculino | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01008` | Sexo feminino | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01317` | Cor ou raça é branca | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01318` | Cor ou raça é preta | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01319` | Cor ou raça é amarela | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01320` | Cor ou raça é parda | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01321` | Cor ou raça é indígena | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01322` | Sexo masculino, Cor ou raça é branca | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01323` | Sexo masculino, Cor ou raça é preta | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01324` | Sexo masculino, Cor ou raça é amarela | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01325` | Sexo masculino, Cor ou raça é parda | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01326` | Sexo masculino, Cor ou raça é indígena | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01327` | Sexo feminino, Cor ou raça é branca | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01328` | Sexo feminino, Cor ou raça é preta | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01329` | Sexo feminino, Cor ou raça é amarela | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01330` | Sexo feminino, Cor ou raça é parda | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01331` | Sexo feminino, Cor ou raça é  indígena | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |

---

## Detalhamento das variáveis

### 📊 Pessoas amarelas

**ID da variável:** `cn22_pop01_res_cor_ama_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01319}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas residentes da cor ou raça amarela em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Curitiba (PR), no setor censitário 410690205040407, 07% das pessoas residentes são da cor ou raça amarela em 2022.


### 📊 Pessoas brancas

**ID da variável:** `cn22_pop01_res_cor_bra_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01317}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas residentes da cor ou raça branca em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Manaus (AM), no setor censitário 130260305110231, 35% das pessoas residentes são da cor ou raça branca em 2022.


### 📊 Pessoas indígenas

**ID da variável:** `cn22_pop01_res_cor_ind_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01321}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas residentes da cor ou raça indígena em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Campo Grande (MS), no setor censitário 500270405000015, 88% das pessoas residentes são da cor ou raça indígena em 2022.


### 📊 Pessoas negras

**ID da variável:** `cn22_pop01_res_cor_neg_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01318}+\mathrm{V01320}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas residentes da cor ou raça negra (preta e parda) em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de São Paulo (SP), no setor censitário 355030878000036, 44% das pessoas residentes são da cor ou raça negra em 2022.


### 📊 Mulheres

**ID da variável:** `cn22_pop01_res_sex_f_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01008}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Fortaleza (CE), no setor censitário 230440005170242, 56% das pessoas residentes são do sexo feminino em 2022.


### 📊 Mulheres amarelas

**ID da variável:** `cn22_pop01_res_corsex_ama_f_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01329}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino da cor ou raça amarela em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Porto Velho (RO), no setor censitário 110020505060023, 5% das pessoas residentes são do sexo feminino e da cor ou raça amarela em 2022.


### 📊 Mulheres brancas

**ID da variável:** `cn22_pop01_res_corsex_bra_f_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01327}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino da cor ou raça branca em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Cuiabá (MT), no setor censitário 510340310420036, 31% das pessoas residentes são do sexo feminino e da cor ou raça branca em 2022.


### 📊 Mulheres indígenas

**ID da variável:** `cn22_pop01_res_corsex_ind_f_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01331}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino da cor ou raça indígena em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Belo Horizonte (MG), no setor censitário 310620060680088, 6% das pessoas residentes são do sexo feminino e da cor ou raça indígena em 2022.


### 📊 Mulheres negras

**ID da variável:** `cn22_pop01_res_corsex_neg_f_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01328}+\mathrm{V01330}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino da cor ou raça negra (preta e parda) em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Recife (PE), no setor censitário 261160605230483, 39% das pessoas residentes são do sexo feminino e da cor ou raça negra em 2022.


### 📊 Homens

**ID da variável:** `cn22_pop01_res_sex_m_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01007}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Goiânia (GO), no setor censitário 520870705220007, 46% das pessoas residentes são do sexo masculino em 2022.


### 📊 Homens amarelos

**ID da variável:** `cn22_pop01_res_corsex_ama_m_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01324}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino da cor ou raça amarela em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município do Rio de Janeiro (RJ), no setor censitário 330455705240784, 03% das pessoas residentes são pessoas do sexo masculino e da cor ou raça amarela em 2022.


### 📊 Homens brancos

**ID da variável:** `cn22_pop01_res_corsex_bra_m_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01322}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino da cor ou raça branca em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Salvador (BA), no setor censitário 292740805060420, 31% das pessoas residentes são do sexo masculino e da cor ou raça branca em 2022.


### 📊 Homens indígenas

**ID da variável:** `cn22_pop01_res_corsex_ind_m_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01326}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino da cor ou raça indígena em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Porto Alegre (RS), no setor censitário 431490205002966, 63% das pessoas residentes são pessoas do sexo masculino e da cor ou raça indígena em 2022.


### 📊 Homens negros

**ID da variável:** `cn22_pop01_res_corsex_neg_m_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01323}+\mathrm{V01325}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino da cor ou raça negra (preta e parda) em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Belém (PA), no setor censitário 150140205000009, 25% das pessoas residentes são do sexo masculino e da cor ou raça negra em 2022.


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

- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)
- [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)

**Download de dados do IBGE**

- [Agregados_por_setores_cor_ou_raca_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip)
- [Agregados_por_setores_basico_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)
- [Agregados_por_setores_demografia_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip)

