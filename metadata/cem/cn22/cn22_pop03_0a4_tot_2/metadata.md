# Pessoas de 0 a 4 anos de idade

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \
**Bases de dados:** [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip), [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de residentes: 0 a 4 anos (principal)](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01031}}{\mathrm{V0001}}$ |
| **[Mulheres: Sexo feminino, 0 a 4 anos](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01020}}{\mathrm{V0001}}$ |
| **[Homens: Sexo masculino, 0 a 4 anos](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)** | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\mathrm{V01009}}{\mathrm{V0001}}$ |

### 📊 Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V0001` | Total de pessoas | [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip) |
| `V01009` | Sexo masculino, 0 a 4 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01020` | Sexo feminino, 0 a 4 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01031` | 0 a 4 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |

---

## Detalhamento das variáveis

### 📊 Total de residentes (principal)

**ID da variável:** `cn22_pop03_0a4_tot_2`\
**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01031}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas residentes com idade de 0 a 4 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Caucaia (CE), no setor censitário 230370905000530, 09% das pessoas residentes tem idade de 0 a 4 anos, em 2022.


### 📊 Mulheres

**ID da variável:** `cn22_pop03_0a4_sex_f_2`\
**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01020}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino com idade de 0 a 4 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Juiz de Fora (MG), no setor censitário 313670205090068, 02% das pessoas residentes são do sexo feminino com idade de 0 a 4 anos em 2022.


### 📊 Homens

**ID da variável:** `cn22_pop03_0a4_sex_m_2`\
**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\mathrm{V01009}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino com idade de 0 a 4 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Barcarena (PA), no setor censitário 150130310000116, 06% das pessoas residentes são do sexo masculino com idade de 0 a 4 anos.


---

## Detalhamento metodológico

Os indicadores relativos do **pop03** foram obtidos pela razão entre cada variável de faixa etária e o total de pessoas residentes no setor censitário, correspondente ao indicador **cn22\_pop01\_res\_tot\_0** e à variável **V0001** do IBGE. Assim, os resultados expressam medidas proporcionais em relação ao total da população residente em cada setor.

O Censo 2022 do IBGE divulga os resultados a partir de grupos de variáveis, os quais geram arquivos, como “Alfabetização”, “Demografia”, “Parentesco”, entre outros.

Algumas dessas variáveis apresentam a mesma descrição em mais de um arquivo. Por exemplo, a variável “V0001”, do Arquivo “Básico” representa o “Total de pessoas”, e a variável “V01006”, do Arquivo “Demografia”, representa a “Quantidade de moradores”. Portanto, ambas representam a população total do setor censitário.

Entretanto, para diferentes arquivos, podem ocorrer diferentes tratamentos de dados quanto ao Sigilo e Confidencialidade, os registros identificados pelo IBGE como “dado numérico omitido” (Categoria “X”).

Em relação ao Arquivo “Básico”, que apresenta informações fundamentais para o cálculo populacional do país, o IBGE opta por divulgar o número real de pessoas do setor censitário, mesmo que este tenha menos de 5 domicílios ocupados. Já para os demais arquivos, o sigilo é aplicado nessas situações. Dessa maneira, o Arquivo “Básico” não sofre omissão de dados por sigilo enquanto o Arquivo “Demografia” sofre.

Para a maioria dos casos, ao se comparar os valores da variável “V01006” com os valores de “V0001”, a diferença não existe. Porém, nos poucos casos em que o tratamento de sigilo causou divergências nessa comparação, há setores com diferenças bastantes significativos, como o setor censitário 530010805400050, que apresenta “V0001” = 10163 moradores, enquanto o “V01006” = “X”.

Diante disso, neste script, optou-se pela variável “V0001”, por se demonstrar mais consistente, como denominador dos indicadores gerados, em detrimento da variável “V01006”. Essa escolha visa eliminar os “dados numéricos omitidos” (Categoria “X”), que a partir da metodologia adotada, são convertidos em “NA”.

Por fim, destaca-se que os indicadores com recorte de cor/raça são disponibilizados apenas a partir da faixa etária de 15 anos. Isso se deve ao fato de que os dados do Censo Demográfico 2022 não divulgam variáveis que articulem simultaneamente faixas etárias desagregadas - como aquelas adotadas na plataforma (0 a 4, 5 a 9 e 10 a 14 anos) - com o recorte de cor/raça. Dessa forma, a construção dessas métricas inicia-se na faixa de 15 a 19 anos, primeiro grupo etário em que essa combinação de variáveis está disponível.

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

- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

**Download de dados do IBGE**

- [Agregados_por_setores_demografia_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip)
- [Agregados_por_setores_basico_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)

