# Pessoas residentes

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \
**Bases de dados:** [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de residentes: Quantidade de moradores (principal)](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop04.qmd)** | Pessoas residentes por km² | $\dfrac{\mathrm{V0001}}{\mathrm{area\_km2}}$ |

### 📊 Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V0001` | Total de pessoas | [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip) |

---

## Detalhamento das variáveis

### 📊 Total de residentes (principal)

**ID da variável:** `cn22_pop04_res_tot_kmtot_2`\
**Script de processamento:** [cn22_pop04.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop04.qmd)\
**Unidade de medida:** Pessoas residentes por km²

**Cálculo:** $\dfrac{\mathrm{V0001}}{\mathrm{area\_km2}}$

O indicador mostra a densidade demográfica de pessoas residentes por área total do setor censitário, a partir dos dados do Censo Demográfico de 2022 do IBGE. Diferentemente do cn22_pop04_res_tot_kmdom_2, que usa apenas a área domiciliada, este indicador utiliza a área total do setor censitário (incluindo áreas não domiciliadas, como praças, ruas e áreas verdes) como denominador. O valor é obtido pela razão entre o total de pessoas residentes e a área total em km² do setor censitário.

**Exemplo**:
> No município de Teresina (PI), no setor censitário 221100105000010, foram registrados 542 moradores residentes e a área total do setor é de 0,49778 quilometros quadrados. Ao relacionar o total de moradores à área total do setor, obtém-se aproximadamente 1088,83 moradores por quilometro quadrado.


---

## Detalhamento metodológico

Atualmente, o grupo pop04 (Densidade) possui dois indicadores. Um deles deriva diretamente da variável V0005 do Censo 2022, que representa o número médio de moradores residentes por domicílio.

Porém, os demais não derivam diretamente de variáveis construídas pelo IBGE. Por isso, há necessidade de construção adicional de métricas relativas, as quais foram obtidas pela divisão do indicador absoluto por duas medidas de área do setor censitário: a área domiciliada (area\_domiciliada\_km2), denominada neste trabalho `cn22_ter01_area_dom_0`, e a área total do setor (area\_km2), denominada `cn22_ter02_area_setor_0`, resultando em medidas proporcionais por km² de área domiciliada e por km² de área total do setor, respectivamente.

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

- [cn22_pop04.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop04.qmd)

**Download de dados do IBGE**

- [Agregados_por_setores_basico_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

