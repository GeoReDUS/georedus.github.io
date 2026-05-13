# Pessoas indígenas

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \
**Bases de dados:** [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip), [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Pessoas indígenas: Cor ou raça é indígena (principal)](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01321}}{\mathrm{V0001}}$ |
| **[Mulheres indígenas: Sexo feminino, Cor ou raça é indígena](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01331}}{\mathrm{V0001}}$ |
| **[Homens indígenas: Sexo masculino, Cor ou raça é indígena](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01326}}{\mathrm{V0001}}$ |

### 📊 Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V0001` | Total de pessoas | [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip) |
| `V01321` | Cor ou raça é indígena | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01326` | Sexo masculino, Cor ou raça é indígena | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01331` | Sexo feminino, Cor ou raça é  indígena | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |

---

## Detalhamento das variáveis

### 📊 Pessoas indígenas (principal)

**ID da variável:** `cn22_pop01_res_cor_ind_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01321}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas residentes da cor ou raça indígena em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Campo Grande (MS), no setor censitário 500270405000015, 88% das pessoas residentes são da cor ou raça indígena em 2022.


### 📊 Mulheres indígenas

**ID da variável:** `cn22_pop01_res_corsex_ind_f_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01331}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino da cor ou raça indígena em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Belo Horizonte (MG), no setor censitário 310620060680088, 6% das pessoas residentes são do sexo feminino e da cor ou raça indígena em 2022.


### 📊 Homens indígenas

**ID da variável:** `cn22_pop01_res_corsex_ind_m_2`\
**Script de processamento:** [cn22_pop01.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop01.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01326}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino da cor ou raça indígena em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Porto Alegre (RS), no setor censitário 431490205002966, 63% das pessoas residentes são pessoas do sexo masculino e da cor ou raça indígena em 2022.


---

## Detalhamento metodológico

As variáveis relativas foram obtidas pela divisão de cada indicador pela população total do setor censitário (V0001), denominada neste trabalho `cn22_pop01_res_tot_0`, resultando em medidas proporcionais ao total populacional do setor.

O Censo 2022 do IBGE divulga os resultados a partir de grupos de variáveis, os quais geram arquivos, como “Alfabetização”, “Demografia”, “Parentesco”, entre outros.

Algumas dessas variáveis apresentam a mesma descrição em mais de um arquivo. Por exemplo, a variável “V0001”, do Arquivo “Básico” representa o “Total de pessoas”, e a variável “V01006”, do Arquivo “Demografia”, representa a “Quantidade de moradores”. Portanto, ambas representam a população total do setor censitário.

Entretanto, para diferentes arquivos, podem ocorrer diferentes tratamentos de dados quanto ao Sigilo e Confidencialidade, os registros identificados pelo IBGE como “dado numérico omitido” (Categoria “X”).

Em relação ao Arquivo “Básico”, que apresenta informações fundamentais para o cálculo populacional do país, o IBGE opta por divulgar o número real de pessoas do setor censitário, mesmo que este tenha menos de 5 domicílios ocupados. Já para os demais arquivos, o sigilo é aplicado nessas situações. Dessa maneira, o Arquivo “Básico” não sofre omissão de dados por sigilo enquanto o Arquivo “Demografia” sofre.

Para a maioria dos casos, ao se comparar os valores da variável “V01006” com os valores de “V0001”, a diferença não existe. Porém, nos poucos casos em que o tratamento de sigilo causou divergências nessa comparação, há setores com diferenças bastantes significativos, como o setor censitário 530010805400050, que apresenta “V0001” = 10163 moradores, enquanto o “V01006” = “X”.

Diante disso, neste script, optou-se pela variável “V0001”, por se demonstrar mais consistente, como denominador dos indicadores gerados, em detrimento da variável “V01006”. Essa escolha visa eliminar os “dados numéricos omitidos” (Categoria “X”), que a partir da metodologia adotada, são convertidos em “NA”.

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

**Download de dados do IBGE**

- [Agregados_por_setores_cor_ou_raca_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip)
- [Agregados_por_setores_basico_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

