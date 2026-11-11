# Índice de Infraestrutura: Iceb (edu06)

**ID da variável:** `in23_edu06_iceb_classif_num`\
**Ano:** 2023\
**Repositório de tratamento e processamento de dados:** https://georedus.github.io/inep-micro-censo-esc/r/iceb.html

## Descrição

O indicador (numérico) aponta a classificação da escola, em termos numéricos, segundo sua adequação ao atendimento da infraestrutura mínima exigida por lei.

**Cálculo:**

$$
\begin{cases} 1, & \text{se } 0 \leq \mathrm{edu06\_iceb} \leq 6 \\ 2, & \text{se } 7 \leq \mathrm{edu06\_iceb} \leq 8 \\ 3, & \text{se } 9 \leq \mathrm{edu06\_iceb} \leq 10 \\ 4, & \text{se } 11 \leq \mathrm{edu06\_iceb} \leq 13 \end{cases}
$$

**Como ler:**
> *A escola possui nível 3 de adequação (média-alta) em termos de conformidade com a lei 15.360/2026 (valor 3).*

---

## Visão geral

O presente documento apresenta a proposta de um **índice sintético para avaliar as condições mínimas de infraestrutura das escolas públicas brasileiras**. Baseado na [Lei Nº 15.360](https://www2.camara.leg.br/legin/fed/lei/2026/lei-15360-25-marco-2026-798852-publicacaooriginal-178602-pl.html), de 25 março 2026 - que define e inclui as condições mínimas que as escolas públicas brasileiras devem garantir na [Lei de Diretrizes e Bases da Educação](https://www.planalto.gov.br/ccivil_03/leis/l9394.htm) (art. 25-A) -, propomos um índice das condições mínimas de infraestrutura das escolas da Educação Básica brasileira, que busca fornecer subsídios para a caracterização e o monitoramento das escolas, sobretudo públicas, de forma rápida e intuitiva.

Ao promover maior transparência sobre as condições das escolas e permitir a identificação de áreas que necessitam de melhorias, acredita-se que o índice pode atuar como uma importante ferramenta para gestores, educadores e a sociedade em geral, visando garantir um padrão adequado de qualidade.

Registre-se, ainda, que dada a frequência dos dados originais que serão utilizados - microdados do [**Censo da Educação Básica do Brasil (Censo Escolar)**](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/taxas-de-rendimento-escolar) -, o cômputo do índice pode ser realizado _anualmente_.

---

## Fonte dos dados

Os dados utilizados no presente documento são provenientes do:

-   [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar): realizado anualmente, o censo é o principal instrumento de coleta de informações sobre todas as etapas e modalidades da educação básica e profissional; abarca todas as escolas públicas e privadas do país e é coordenado pelo [Inep](https://www.gov.br/inep/pt-br) e realizado em regime de colaboração entre as secretarias estaduais e municipais de educação.

---

## Definições metodológicas

NoteNota

A construção dos indicadores utilizados na GeoReDUS é resultado de um processo contínuo de diálogo com pesquisadores especialistas e com a comunidade de usuários. Sugestões, comentários e críticas são sempre bem-vindos. Convidamos você a registrar suas contribuições [neste formulário](https://www.redus.org.br/georedus-rede-de-dados-urbanos/formularios/cbf766bb-9a74-4bc5-897a-70b9151afbdb), que serão analisadas e consideradas nas próximas revisões dos indicadores.

De acordo com o determinado pelo Art. No. 25-A da [LDB](https://www.planalto.gov.br/ccivil_03/leis/l9394.htm), as condições mínimas que as escolas devem atender, a partir de 2026, são:

1.  Existência de biblioteca; IN\_BIBLIOTECA
2.  Existência de laboratório de ciências; IN\_LABORATORIO\_CIENCIAS
3.  Existência de laboratório de informática; IN\_LABORATORIO\_INFORMATICA
4.  Acesso à internet; IN\_INTERNET
5.  Existência de quadra poliesportiva coberta; IN\_QUADRA\_ESPORTES\_COBERTA
6.  Existência de cozinha; IN\_COZINHA
7.  Existência de refeitório; IN\_REFEITORIO
8.  Existência de banheiro; IN\_BANHEIRO
9.  Existência de instalações com acessibilidade;
10.  Número adequado de estudantes por turma;
11.  Acesso à energia elétrica; IN\_ENERGIA\_INEXISTENTE (usa-se o oposto)
12.  Abastecimento de água tratada; IN\_AGUA\_POTAVEL
13.  Acesso a esgotamento sanitário; IN\_ESGOTO\_INEXISTENTE (usa-se o oposto)
14.  Manejo de resíduos sólidos; IN\_LIXO\_SERVICO\_COLETA

Considerando-se o conjunto dos itens, de modo geral é possível encontrar uma variável do [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar) que corresponde de forma direta e objetiva ao previsto na legislação. Dois itens, porém, apresentam maior complexidade, pois carecem de definições mais assertivas: i) _instalações com acessibilidade_ e ii) _número adequado de estudantes por turma_.

No caso das _instalações com acessibilidade_, o artigo 24 do Decreto nº 5.296/2004 estabelece que todos os espaços das escolas brasileiras devem estar preparados para atender pessoas com deficiência ou mobilidade reduzida. Nesse sentido, o índice considera válidas para esse critério as escolas que dispõem de acessibilidade em todas as suas salas em uso e contam com todos os recursos avaliados pelo Censo Escolar, à exceção do elevador.

Já no caso do _número adequado de estudantes por turma_, ainda que a inclusão dessa questão na norma seja um importante reconhecimento, a ausência de um critério objetivo para concretizá-la (número máximo de estudantes, por exemplo) impede o seu acompanhamento. Como decorrência, neste momento esse será o único item que _não comporá o índice_.

Saliente-se, para terminar as considerações sobre as variáveis utilizadas, que os itens relacionados à _água_, aos _resíduos sólidos_ e ao _esgotamento sanitário_ podem ser mensurados por meio de outras variáveis disponibilizadas pelo [Censo Escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar). A questão, neste caso, reside no grau de restritividade que se adota ao capturar cada um desses itens.

Passando ao desenho do índice, destaque-se que todas as variáveis terão o mesmo peso. Tal escolha baseia-se:

-   No reconhecimento de que a própria **normativa não estabelece** ou sinaliza a necessidade de se adotar alguma **diferenciação** entre os itens previstos, e,
    
-   No entendimento de que, por tratar das **condições mínimas** para o funcionamento adequado das escolas, **todas as variáveis são igualmente importantes**.
    

Com relação à comunicação do índice, para apresentar os resultados de forma mais intuitiva e menos complexa, serão criadas quatro classes de adequação. Inicialmente será computado o número de itens presentes em cada uma das escolas. Realizada a soma e obtidos os valores específicos para cada caso, passar-se-á, então, à etapa de classificação, realizada com base em análises da distribuição dos indicadores entre as escolas, tal qual proposto a seguir:

Grau de adequação

Soma de itens

Adequação baixa (1)

0 a 6

Adequação média-baixa (2)

7 a 8

Adequação média-alta (3)

9 a 10

Adequação alta (4)

11 a 13

Expostos os comentários sobre a composição do índice, é importante salientar que, de todo o universo das escolas, serão avaliadas apenas as **escolas ativas**. Ou seja, aquelas que são assim discriminadas pelo [censo escolar](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-escolar) (variável “tp\_situacao\_funcionamento”) e que possuem ao menos uma matrícula.

Por fim, a seguir apresenta-se a lógica da nomenclatura do índice. Apenas para fins ilustrativos, adotou-se o ano de 2025 como referência (mais atual no momento de geração do código).

A seguir, os itens que compõem o índice, bem como as variáveis selecionadas para computá-los são apresentados em maior detalhe. Expõe-se a descrição de seu cálculo, o que ele representa e como se espera que ele seja interpretado.

Note, ainda, que as definições fornecidas para os itens foram extraídas do [**Caderno de Conceitos e Orientações do Censo Escolar 2025: 1ª Etapa da Coleta**](https://www.gov.br/inep/pt-br/centrais-de-conteudo/acervo-linha-editorial/publicacoes-institucionais/estatisticas-e-indicadores-educacionais/caderno-de-conceitos-e-orientacoes-do-censo-escolar-2025-1a-etapa-da-coleta). Esse material é disponibilizado pelo [Inep](https://www.gov.br/inep/pt-br) e tem como objetivo orientar os responsáveis pela declaração e pelo acompanhamento da coleta do Censo Escolar.

---

### 🔗 Links

- Documentação completa do processamento: [Índice de Infraestrutura](https://georedus.github.io/inep-micro-censo-esc/r/iceb.html)
- Dicionário de indicadores (`edu06_iceb_classif_num`): [Índice de Infraestrutura](https://georedus.github.io/inep-micro-censo-esc/r/iceb.html#dicionário-de-indicadores-que-serão-produzidos)
