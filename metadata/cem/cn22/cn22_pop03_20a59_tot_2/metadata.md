# Pessoas de 20 a 59 anos de idade

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \
**Bases de dados:** [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip), [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip), [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de residentes: 20 a 59 anos (principal)](#cn22_pop03_20a59_tot_2)**<br/> | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\begin{aligned}\mathrm{V01035} + \mathrm{V01036} + \mathrm{V01037} \\ + \mathrm{V01038} + \mathrm{V01039}\end{aligned}}{\mathrm{V0001}}$ |
| **[Pessoas amarelas: 60 anos ou mais, Cor ou raça é amarela](#cn22_pop03_20a59_cor_ama_2)**<br/> | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\begin{aligned}\mathrm{V00664} + \mathrm{V00669} + \mathrm{V00674} \\ + \mathrm{V00679} + \mathrm{V00684} + \mathrm{V00689} \\ + \mathrm{V00694} + \mathrm{V00699}\end{aligned}}{\mathrm{V0001}}$ |
| **[Pessoas brancas: 60 anos ou mais, Cor ou raça é branca](#cn22_pop03_20a59_cor_bra_2)**<br/> | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\begin{aligned}\mathrm{V00662} + \mathrm{V00667} + \mathrm{V00672} \\ + \mathrm{V00677} + \mathrm{V00682} + \mathrm{V00687} \\ + \mathrm{V00692} + \mathrm{V00697}\end{aligned}}{\mathrm{V0001}}$ |
| **[Pessoas indígenas: 60 anos ou mais, Cor ou raça é indígena](#cn22_pop03_20a59_cor_ind_2)**<br/> | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\begin{aligned}\mathrm{V00666} + \mathrm{V00671} + \mathrm{V00676} \\ + \mathrm{V00681} + \mathrm{V00686} + \mathrm{V00691} \\ + \mathrm{V00696} + \mathrm{V00701}\end{aligned}}{\mathrm{V0001}}$ |
| **[Pessoas negras: 60 anos ou mais, Cor ou raça é preta ou parda](#cn22_pop03_20a59_cor_neg_2)**<br/> | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\begin{aligned}\mathrm{V00663} + \mathrm{V00665} + \mathrm{V00668} \\ + \mathrm{V00670} + \mathrm{V00673} + \mathrm{V00675} \\ + \mathrm{V00678} + \mathrm{V00680} + \mathrm{V00683} \\ + \mathrm{V00685} + \mathrm{V00688} + \mathrm{V00690} \\ + \mathrm{V00693} + \mathrm{V00695} + \mathrm{V00698} \\ + \mathrm{V00700}\end{aligned}}{\mathrm{V0001}}$ |
| **[Mulheres: Sexo feminino, 20 a 59 anos](#cn22_pop03_20a59_sex_f_2)**<br/> | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\begin{aligned}\mathrm{V01024} + \mathrm{V01025} + \mathrm{V01026} \\ + \mathrm{V01027} + \mathrm{V01028}\end{aligned}}{\mathrm{V0001}}$ |
| **[Homens: Sexo masculino, 20 a 59 anos](#cn22_pop03_20a59_sex_m_2)**<br/> | Porcentagem em relação ao total de pessoas residentes | $\dfrac{\begin{aligned}\mathrm{V01013} + \mathrm{V01014} + \mathrm{V01015} \\ + \mathrm{V01016} + \mathrm{V01017}\end{aligned}}{\mathrm{V0001}}$ |

### Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V0001` | Total de pessoas | [Básico](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip) |
| `V00662` | 20 a 24 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00663` | 20 a 24 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00664` | 20 a 24 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00665` | 20 a 24 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00666` | 20 a 24 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00667` | 25 a 29 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00668` | 25 a 29 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00669` | 25 a 29 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00670` | 25 a 29 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00671` | 25 a 29 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00672` | 30 a 34 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00673` | 30 a 34 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00674` | 30 a 34 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00675` | 30 a 34 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00676` | 30 a 34 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00677` | 35 a 39 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00678` | 35 a 39 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00679` | 35 a 39 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00680` | 35 a 39 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00681` | 35 a 39 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00682` | 40 a 44 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00683` | 40 a 44 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00684` | 40 a 44 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00685` | 40 a 44 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00686` | 40 a 44 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00687` | 45 a 49 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00688` | 45 a 49 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00689` | 45 a 49 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00690` | 45 a 49 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00691` | 45 a 49 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00692` | 50 a 54 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00693` | 50 a 54 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00694` | 50 a 54 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00695` | 50 a 54 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00696` | 50 a 54 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00697` | 55 a 59 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00698` | 55 a 59 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00699` | 55 a 59 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00700` | 55 a 59 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00701` | 55 a 59 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V01013` | Sexo masculino, 20 a 24 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01014` | Sexo masculino, 25 a 29 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01015` | Sexo masculino, 30 a 39 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01016` | Sexo masculino, 40 a 49 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01017` | Sexo masculino, 50 a 59 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01024` | Sexo feminino, 20 a 24 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01025` | Sexo feminino, 25 a 29 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01026` | Sexo feminino, 30 a 39 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01027` | Sexo feminino, 40 a 49 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01028` | Sexo feminino, 50 a 59 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01035` | 20 a 24 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01036` | 25 a 29 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01037` | 30 a 39 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01038` | 40 a 49 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01039` | 50 a 59 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |

---

## Detalhamento das variáveis

### Total de residentes (principal) {#cn22_pop03_20a59_tot_2}

**ID da variável:** `cn22_pop03_20a59_tot_2`\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\begin{aligned}\mathrm{V01035} + \mathrm{V01036} + \mathrm{V01037} \\ + \mathrm{V01038} + \mathrm{V01039}\end{aligned}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas residentes com idade de 20 a 59 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Três Lagoas (MS), no setor censitário 500830505000235, 63% das pessoas residentes tem idade de 20 a 59 anos em 2022.

**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

### Pessoas amarelas {#cn22_pop03_20a59_cor_ama_2}

**ID da variável:** `cn22_pop03_20a59_cor_ama_2`\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\begin{aligned}\mathrm{V00664} + \mathrm{V00669} + \mathrm{V00674} \\ + \mathrm{V00679} + \mathrm{V00684} + \mathrm{V00689} \\ + \mathrm{V00694} + \mathrm{V00699}\end{aligned}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas de cor ou raça amarela com idade de 20 a 59 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Aracaju (SE), no setor censitário 280030805000002, 16% das pessoas residentes são de cor ou raça amarela com idade de 20 a 59 anos em 2022.

**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

### Pessoas brancas {#cn22_pop03_20a59_cor_bra_2}

**ID da variável:** `cn22_pop03_20a59_cor_bra_2`\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\begin{aligned}\mathrm{V00662} + \mathrm{V00667} + \mathrm{V00672} \\ + \mathrm{V00677} + \mathrm{V00682} + \mathrm{V00687} \\ + \mathrm{V00692} + \mathrm{V00697}\end{aligned}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas de cor ou raça branca com idade de 20 a 59 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Rio de Janeiro (RJ), no setor censitário 330455705110151, 32% das pessoas residentes são de cor ou raça branca com idade de 20 a 59 anos em 2022.

**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

### Pessoas indígenas {#cn22_pop03_20a59_cor_ind_2}

**ID da variável:** `cn22_pop03_20a59_cor_ind_2`\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\begin{aligned}\mathrm{V00666} + \mathrm{V00671} + \mathrm{V00676} \\ + \mathrm{V00681} + \mathrm{V00686} + \mathrm{V00691} \\ + \mathrm{V00696} + \mathrm{V00701}\end{aligned}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas de cor ou raça indígena com idade de 20 a 59 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Caucaia (CE), no setor censitário 230370905000485, 64% das pessoas residentes são de cor ou raça indígena com idade de 20 a 59 anos em 2022.

**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

### Pessoas negras {#cn22_pop03_20a59_cor_neg_2}

**ID da variável:** `cn22_pop03_20a59_cor_neg_2`\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\begin{aligned}\mathrm{V00663} + \mathrm{V00665} + \mathrm{V00668} \\ + \mathrm{V00670} + \mathrm{V00673} + \mathrm{V00675} \\ + \mathrm{V00678} + \mathrm{V00680} + \mathrm{V00683} \\ + \mathrm{V00685} + \mathrm{V00688} + \mathrm{V00690} \\ + \mathrm{V00693} + \mathrm{V00695} + \mathrm{V00698} \\ + \mathrm{V00700}\end{aligned}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas de cor ou raça negra (preta e parda) com idade de 20 a 59 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Feira de Santana (BA), no setor censitário 291080005060185, 56% das pessoas residentes são de cor ou raça negra com idade de 20 a 59 anos em 2022.

**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

### Mulheres {#cn22_pop03_20a59_sex_f_2}

**ID da variável:** `cn22_pop03_20a59_sex_f_2`\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\begin{aligned}\mathrm{V01024} + \mathrm{V01025} + \mathrm{V01026} \\ + \mathrm{V01027} + \mathrm{V01028}\end{aligned}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo feminino com idade de 20 a 59 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Itaituba (PA), no setor censitário 150360605000247, 31% das pessoas residentes são do sexo feminino com idade de 20 a 59 anos em 2022.

**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

### Homens {#cn22_pop03_20a59_sex_m_2}

**ID da variável:** `cn22_pop03_20a59_sex_m_2`\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes

**Cálculo:** $\dfrac{\begin{aligned}\mathrm{V01013} + \mathrm{V01014} + \mathrm{V01015} \\ + \mathrm{V01016} + \mathrm{V01017}\end{aligned}}{\mathrm{V0001}}$

O indicador mostra a porcentagem de pessoas do sexo masculino com idade de 20 a 59 anos em relação ao número total de pessoas residentes em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Olinda (PE), no setor censitário 260960005000723, 36% das pessoas residentes são do sexo masculino com idade de 20 a 59 anos em 2022.

**Script de processamento:** [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

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

- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)
- [cn22_pop03.qmd](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop03.qmd)

**Download de dados do IBGE**

- [Agregados_por_setores_demografia_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip)
- [Agregados_por_setores_basico_BR_20250417.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_basico_BR_20250417.zip)
- [Agregados_por_setores_alfabetizacao_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip)

