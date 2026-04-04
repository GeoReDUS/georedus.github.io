# Domicílios sem iluminação pública

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-inf \

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de domicílios: Teste (principal)](#cn22_inf01_silu_tot_dom_2)**<br/> | Porcentagem em relação ao total de domicílios | $\dfrac{\mathrm{V05013}}{\mathrm{V05000}}$ |
| **[Total de moradores: Teste](#cn22_inf01_silu_tot_mor_2)**<br/> | Porcentagem em relação ao total de moradores | $\dfrac{\mathrm{V05213}}{\mathrm{V05200}}$ |

---

## Detalhamento das variáveis

### Total de domicílios (principal) {#cn22_inf01_silu_tot_dom_2}

**ID da variável:** `cn22_inf01_silu_tot_dom_2`\
**Unidade de medida:** Porcentagem em relação ao total de domicílios

**Cálculo:** $\dfrac{\mathrm{V05013}}{\mathrm{V05000}}$

O indicador mostra a porcentagem de domicílios particulares permanentes ocupados (DPPO) sem iluminação pública no entorno em relação ao total de DPPO, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Coari (AM), no setor censitário 130120905000103, 11% dos domicílios particulares permanentes ocupados não possuem iluminação pública no entorno.

**Script de processamento:** [cn22_inf.qmd#L209](https://github.com/GeoReDUS/cn22-inf/blob/main/r/cn22_inf.qmd#L209)

### Total de moradores {#cn22_inf01_silu_tot_mor_2}

**ID da variável:** `cn22_inf01_silu_tot_mor_2`\
**Unidade de medida:** Porcentagem em relação ao total de moradores

**Cálculo:** $\dfrac{\mathrm{V05213}}{\mathrm{V05200}}$

O indicador mostra a porcentagem de moradores residentes em domicílios particulares permanentes ocupados (DPPO) sem iluminação pública no entorno em relação ao total de moradores residentes em DPPO, para cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Belford Roxo (RJ), no setor censitário 330045605030196, 90% dos moradores residentes em domicílios particulares permanentes ocupados residem em domicílios que não possuem iluminação pública no entorno.

**Script de processamento:** [cn22_inf.qmd#L212](https://github.com/GeoReDUS/cn22-inf/blob/main/r/cn22_inf.qmd#L212)

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
-   **Geração de indicativos:** as variáveis relativas foram obtidas pela divisão dos indicadores por um dos seguintes:
    
    -   total de domicílios particulares permanentes ocupados \[Domicílios em Setor Escolhido para Aplicação do Entorno\] (V05000), denominada neste trabalho `cn_22_dom06_ent_tot_0`, resultando em medidas proporcionais ao total de domicílios particulares permanentes ocupados do setor;
    -   quantidade total de moradores em domicílios particulares permanentes ocupados \[Domicílios em Setor Escolhido para Aplicação do Entorno\] (V05200), denominada neste trabalho `cn_22_dom06_ent_tot_mor_0`, resultando em medidas proporcionais ao total de moradores em domicílios particulares permanentes ocupados do setor;

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

- [cn22_inf.qmd#L209](https://github.com/GeoReDUS/cn22-inf/blob/main/r/cn22_inf.qmd#L209)
- [cn22_inf.qmd#L212](https://github.com/GeoReDUS/cn22-inf/blob/main/r/cn22_inf.qmd#L212)

