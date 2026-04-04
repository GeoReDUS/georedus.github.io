# Pessoas de 60 ou mais anos de idade

**Fonte:** [CENSO Demográfico 2022 - IBGE](https://censo2022.ibge.gov.br/panorama/)\
**Ano:** 2022\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/cn22-pop/ \
**Bases de dados:** [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip), [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip), [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip)

| Variável | Unidade de medida | Cálculo |
|----------|-------------------|---------|
| **[Total de pessoas alfabetizadas: 60 anos ou mais (principal)](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L260)** | Porcentagem em relação ao total de pessoas residentes com idade superior a 60 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00757}+\mathrm{V00758}+\mathrm{V00759}+\\ \mathrm{V00760}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01040}+\mathrm{V01041}\end{matrix}}$ |
| **[Pessoas amarelas: 60 anos ou mais, Cor ou raça é amarela](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L284)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça amarela com idade superior a 60 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00808}+\mathrm{V00813}+\mathrm{V00818}+\\ \mathrm{V00823}\end{matrix}}{\scriptstyle \mathrm{V01389}}$ |
| **[Pessoas brancas: 60 anos ou mais, Cor ou raça é branca](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L282)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça branca com idade superior a 60 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00806}+\mathrm{V00811}+\mathrm{V00816}+\\ \mathrm{V00821}\end{matrix}}{\scriptstyle \mathrm{V01387}}$ |
| **[Pessoas indígenas: 60 anos ou mais, Cor ou raça é indígena](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L285)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça indígena com idade superior a 60 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00810}+\mathrm{V00815}+\mathrm{V00820}+\\ \mathrm{V00825}\end{matrix}}{\scriptstyle \mathrm{V01391}}$ |
| **[Pessoas negras: 60 anos ou mais, Cor ou raça é preta ou parda](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L283)** | Porcentagem em relação ao total de pessoas residentes de cor ou raça negra com idade superior a 60 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00807}+\mathrm{V00809}+\mathrm{V00812}+\\ \mathrm{V00814}+\mathrm{V00817}+\mathrm{V00819}+\\ \mathrm{V00822}+\mathrm{V00824}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01388}+\mathrm{V01390}\end{matrix}}$ |
| **[Mulheres: Sexo feminino, 60 ou mais anos](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L269)** | Porcentagem em relação ao total de pessoas residentes do sexo feminino com idade superior a 60 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00848}+\mathrm{V00849}+\mathrm{V00850}+\\ \mathrm{V00851}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01029}+\mathrm{V01030}\end{matrix}}$ |
| **[Homens: Sexo masculino, 60 ou mais anos](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L265)** | Porcentagem em relação ao total de pessoas residentes do sexo masculino com idade superior a 60 anos | $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00835}+\mathrm{V00836}+\mathrm{V00837}+\\ \mathrm{V00838}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01018}+\mathrm{V01019}\end{matrix}}$ |

### Variáveis originais do CENSO 2022 - IBGE

| Variável | Descrição | Conjunto de dados |
|----------|-----------|-------------------|
| `V00757` | Pessoas alfabetizadas, 60 a 64 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00758` | Pessoas alfabetizadas, 65 a 69 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00759` | Pessoas alfabetizadas, 70 a 79 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00760` | Pessoas alfabetizadas, 80 anos ou mais | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00806` | Pessoas alfabetizadas, 60 a 64 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00807` | Pessoas alfabetizadas, 60 a 64 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00808` | Pessoas alfabetizadas, 60 a 64 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00809` | Pessoas alfabetizadas, 60 a 64 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00810` | Pessoas alfabetizadas, 60 a 64 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00811` | Pessoas alfabetizadas, 65 a 69 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00812` | Pessoas alfabetizadas, 65 a 69 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00813` | Pessoas alfabetizadas, 65 a 69 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00814` | Pessoas alfabetizadas, 65 a 69 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00815` | Pessoas alfabetizadas, 65 a 69 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00816` | Pessoas alfabetizadas, 70 a 79 anos, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00817` | Pessoas alfabetizadas, 70 a 79 anos, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00818` | Pessoas alfabetizadas, 70 a 79 anos, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00819` | Pessoas alfabetizadas, 70 a 79 anos, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00820` | Pessoas alfabetizadas, 70 a 79 anos, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00821` | Pessoas alfabetizadas, 80 anos ou mais, Cor ou raça é branca | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00822` | Pessoas alfabetizadas, 80 anos ou mais, Cor ou raça é preta | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00823` | Pessoas alfabetizadas, 80 anos ou mais, Cor ou raça é amarela | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00824` | Pessoas alfabetizadas, 80 anos ou mais, Cor ou raça é parda | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00825` | Pessoas alfabetizadas, 80 anos ou mais, Cor ou raça é indígena | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00835` | Pessoas alfabetizadas, Sexo masculino, 60 a 64 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00836` | Pessoas alfabetizadas, Sexo masculino, 65 a 69 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00837` | Pessoas alfabetizadas, Sexo masculino, 70 a 79 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00838` | Pessoas alfabetizadas, Sexo masculino, 80 anos ou mais | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00848` | Pessoas alfabetizadas, Sexo feminino, 60 a 64 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00849` | Pessoas alfabetizadas, Sexo feminino, 65 a 69 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00850` | Pessoas alfabetizadas, Sexo feminino, 70 a 79 anos | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V00851` | Pessoas alfabetizadas, Sexo feminino, 80 anos ou mais | [Alfabetização](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip) |
| `V01018` | Sexo masculino, 60 a 69 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01019` | Sexo masculino, 70 anos ou mais | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01029` | Sexo feminino, 60 a 69 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01030` | Sexo feminino, 70 anos ou mais | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01040` | 60 a 69 anos | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01041` | 70 anos ou mais | [Demografia](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip) |
| `V01387` | 60 anos ou mais, Cor ou raça é branca | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01388` | 60 anos ou mais, Cor ou raça é preta | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01389` | 60 anos ou mais, Cor ou raça é amarela | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01390` | 60 anos ou mais, Cor ou raça é parda | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |
| `V01391` | 60 anos ou mais, Cor ou raça é indígena | [Cor/Raça](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip) |

---

## Detalhamento das variáveis

### Total de pessoas alfabetizadas (principal)

**ID da variável:** `cn22_pop06_alf4_tot_2`\
**Script de processamento:** [cn22_pop06.qmd#L260](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L260)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes com idade superior a 60 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00757}+\mathrm{V00758}+\mathrm{V00759}+\\ \mathrm{V00760}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01040}+\mathrm{V01041}\end{matrix}}$

O indicador mostra a porcentagem de pessoas alfabetizadas, com mais de 60 anos, em relação ao número total de pessoas com idade superior a 60 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Brasília (DF), no setor censitário 530010805440143, 69% das pessoas com idade superior a 60 anos são alfabetizadas em 2022.


### Pessoas amarelas

**ID da variável:** `cn22_pop06_alf4_cor_ama_2`\
**Script de processamento:** [cn22_pop06.qmd#L284](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L284)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça amarela com idade superior a 60 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00808}+\mathrm{V00813}+\mathrm{V00818}+\\ \mathrm{V00823}\end{matrix}}{\scriptstyle \mathrm{V01389}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça amarela, com idade superior a 60 anos, em relação ao número total de pessoas de cor ou raça amarela com idade superior a 60 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Sertaneja (PR), no setor censitário 412641000000000, 69% das pessoas com idade superior a 60 anos e de cor ou raça amarela são alfabetizadas em 2022.


### Pessoas brancas

**ID da variável:** `cn22_pop06_alf4_cor_bra_2`\
**Script de processamento:** [cn22_pop06.qmd#L282](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L282)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça branca com idade superior a 60 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00806}+\mathrm{V00811}+\mathrm{V00816}+\\ \mathrm{V00821}\end{matrix}}{\scriptstyle \mathrm{V01387}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça branca, com idade superior a 60 anos, em relação ao número total de pessoas de cor ou raça branca com idade superior a 60 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Novo Cruzeiro (MG), no setor censitário 314531000000000, 62% das pessoas com idade superior a 60 anos e de cor ou raça branca são alfabetizadas em 2022.


### Pessoas indígenas

**ID da variável:** `cn22_pop06_alf4_cor_ind_2`\
**Script de processamento:** [cn22_pop06.qmd#L285](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L285)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça indígena com idade superior a 60 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00810}+\mathrm{V00815}+\mathrm{V00820}+\\ \mathrm{V00825}\end{matrix}}{\scriptstyle \mathrm{V01391}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça indígena, com idade superior a 60 anos, em relação ao número total de pessoas de cor ou raça indígena com idade superior a 60 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Itarema (CE), no setor censitário 230655000000000, 23% das pessoas com idade superior a 60 anos e de cor ou raça indígena são alfabetizadas em 2022.


### Pessoas negras

**ID da variável:** `cn22_pop06_alf4_cor_neg_2`\
**Script de processamento:** [cn22_pop06.qmd#L283](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L283)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes de cor ou raça negra com idade superior a 60 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00807}+\mathrm{V00809}+\mathrm{V00812}+\\ \mathrm{V00814}+\mathrm{V00817}+\mathrm{V00819}+\\ \mathrm{V00822}+\mathrm{V00824}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01388}+\mathrm{V01390}\end{matrix}}$

O indicador mostra a porcentagem de pessoas alfabetizadas de cor ou raça negra (preta e parda), com idade superior a 60 anos, em relação ao número total de pessoas de cor ou raça negra com idade superior a 60 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Iconha (ES), no setor censitário 320260000000000, 50% das pessoas com idade superior a 60 anos e de cor ou raça negra são alfabetizadas em 2022.


### Mulheres

**ID da variável:** `cn22_pop06_alf4_sex_f_2`\
**Script de processamento:** [cn22_pop06.qmd#L269](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L269)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes do sexo feminino com idade superior a 60 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00848}+\mathrm{V00849}+\mathrm{V00850}+\\ \mathrm{V00851}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01029}+\mathrm{V01030}\end{matrix}}$

O indicador mostra a porcentagem de pessoas do sexo feminino alfabetizadas, com idade superior a 60 anos, em relação ao número total de pessoas do sexo feminino com idade superior a 60 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Riachão do Jacuípe (BA), no setor censitário 292630105000006, 38% das pessoas do sexo feminino com idade superior a 60 anos são alfabetizadas em 2022.


### Homens

**ID da variável:** `cn22_pop06_alf4_sex_m_2`\
**Script de processamento:** [cn22_pop06.qmd#L265](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L265)\
**Unidade de medida:** Porcentagem em relação ao total de pessoas residentes do sexo masculino com idade superior a 60 anos

**Cálculo:** $\dfrac{\scriptstyle \begin{matrix}\mathrm{V00835}+\mathrm{V00836}+\mathrm{V00837}+\\ \mathrm{V00838}\end{matrix}}{\scriptstyle \begin{matrix}\mathrm{V01018}+\mathrm{V01019}\end{matrix}}$

O indicador mostra a porcentagem de pessoas do sexo masculino alfabetizadas, com idade superior a 60 anos, em relação ao número total de pessoas do sexo masculino com idade superior a 60 anos em cada setor censitário, segundo o Censo Demográfico de 2022 do IBGE.

**Exemplo**:
> No município de Blumenau (SC), no setor censitário 420240405000629, 57% das pessoas do sexo masculino com idade superior a 60 anos são alfabetizadas em 2022.


---

## Detalhamento metodológico

As variáveis relativas foram obtidas pela razão entre cada indicador e o total de pessoas da mesma faixa etária no setor censitário. Desse modo, os resultados expressam medidas proporcionais internas a cada grupo etário - por exemplo, o número de pessoas alfabetizadas de 15 a 19 anos em relação ao total de pessoas de 15 a 19 anos no setor. Quando houver recorte de cor ou raça, a abordagem é semelhante, sendo expressas medidas proporcionais internas ao grupo etário e de cor ou raça - por exemplo, o número de pessoas alfabetizadas de 15 a 19 anos e de cor ou raça negra em relação ao total de pessoas de 15 a 19 anos e de cor ou raça negra no setor.

O Censo 2022 do IBGE divulga os resultados a partir de grupos de variáveis, os quais geram arquivos, como “Alfabetização”, “Demografia”, “Parentesco”, entre outros.

Algumas dessas variáveis apresentam a mesma descrição em mais de um arquivo. Por exemplo, a variável “V00645”, do Arquivo “Alfabetização”, e a variável “V01035”, do Arquivo “Demografia”, representam o número de moradores com idade de 20 a 24 anos. Entretanto, para diferentes arquivos, podem ocorrer diferentes agregações de grupos etários - por exemplo, no arquivo “Alfabetização”, a variável “V00647” representa o número de moradores com idade de 30 a 34 anos, porém no arquivo “Demografia”, a variável “V01037” representa o número de moradores com idade de 30 a 39 anos.

Diante disso, neste script, quando houve possibilidade de escolha entre distintas variáveis para obter denominadores de indicadores relativos, optou-se por variáveis com dados de grupos etários mais agregados, portanto, mais abrangentes. Essa escolha visa reduzir os registros identificados pelo IBGE como “dado numérico omitido” (Categoria “X”), que a partir da metodologia adotada, são convertidos em “NA”.

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

- [cn22_pop06.qmd#L260](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L260)
- [cn22_pop06.qmd#L284](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L284)
- [cn22_pop06.qmd#L282](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L282)
- [cn22_pop06.qmd#L285](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L285)
- [cn22_pop06.qmd#L283](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L283)
- [cn22_pop06.qmd#L269](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L269)
- [cn22_pop06.qmd#L265](https://github.com/GeoReDUS/cn22-pop/blob/main/r/cn22_pop06.qmd#L265)

**Download de dados do IBGE**

- [Agregados_por_setores_alfabetizacao_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_alfabetizacao_BR.zip)
- [Agregados_por_setores_demografia_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_demografia_BR.zip)
- [Agregados_por_setores_cor_ou_raca_BR.zip](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Setor_csv/Agregados_por_setores_cor_ou_raca_BR.zip)

