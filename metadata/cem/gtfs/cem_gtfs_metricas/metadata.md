# Indicadores — Partidas por hora


## Descrição do indicador

Oferta de transporte público alcançável em até 10 minutos a pé (800 m pela rede de caminhada) do centro de cada hexágono, em partidas por hora entre 06:00 e 09:00.

| Indicador | Cálculo | Como ler |
|-----------|-----------|-----------|
| **[Partidas por hora](https://gilandrade.github.io/process_gtfs/#oferta-hexagono)** | $M2_h = \sum_{(r,d) \in R_h} \max_{s \in S_h} f_{s,r,d}$ | Um hexágono com valor 40 tem ao alcance de uma caminhada de 10 minutos o equivalente a 40 partidas por hora, contando cada linha e sentido uma única vez. |


## Visão geral

As camadas de mobilidade da [GeoReDUS](https://www.redus.org.br/georedus) descrevem a rede de transporte público (ônibus, BRT, VLT, metrô, trem e balsa) de cidades brasileiras a partir de arquivos [GTFS](https://gtfs.org/pt/), o formato aberto em que operadores e órgãos gestores publicam linhas, paradas e horários.

São quatro grupos de camadas:

-   **Estações**: cada parada com serviço, dimensionada pelas partidas por hora ou pelo número de linhas que a atendem.
-   **Linhas**: o traçado de cada linha, com espessura proporcional à frequência, com filtros por modo de transporte.
-   **Oferta acessível por hexágono**: quantas partidas por hora estão ao alcance de 10 minutos a pé de cada hexágono.
-   **Tempo de viagem**: o tempo de viagem porta a porta, em transporte público e a pé, a partir do hexágono clicado.

Os indicadores por área usam a grade hexagonal [H3](https://h3geo.org/) na resolução 9 (hexágonos de cerca de 0,1 km², com uns 200 m de lado), sobre uma área de estudo formada pela união de faixas de 3 km em torno das paradas de cada feed.


## Detalhamento metodológico

Mede quanta oferta de transporte público está ao alcance de uma caminhada de 10 minutos, a 4,8 km/h (800 m), a partir do centro de cada hexágono:

$$M2_h = \sum_{(r,d) \in R_h} \max_{s \in S_h} f_{s,r,d}$$

-   $S_h$ é o conjunto das paradas a até 800 m do centro do hexágono, medidos pela rede de caminhada do OpenStreetMap, e não em linha reta.
-   $R_h$ é o conjunto dos pares (linha, sentido) que atendem alguma parada de $S_h$.
-   $f_{s,r,d}$ é o número de partidas por hora do par na parada, em média entre 06:00 e 09:00 do dia útil de referência.

Cada par (linha, sentido) entra uma única vez, pela sua melhor parada acessível. Somar por parada contaria a mesma corrida uma vez por ponto da linha dentro do raio, o que tornaria o indicador dependente do espaçamento entre pontos e impediria a comparação entre cidades. Linhas paralelas somam integralmente, sem desconto de redundância. Um hexágono sem parada a até 800 m tem valor 0. O valor não muda com o controle de horário, porque o indicador usa sempre a janela de 06:00 a 09:00.

Ao passar o cursor, aparece também a **distância à parada mais próxima**: a distância pela rede de caminhada, do centro do hexágono à parada com serviço mais próxima, sem limite de distância.

### Definições gerais

**Dia útil de referência.** Todas as camadas descrevem um único dia de serviço, e não a média do período de validade do feed. Em cada cidade, escolhe-se a terça, quarta ou quinta-feira com mais viagens ativas em toda a validade do feed; segunda e sexta ficam de fora por concentrarem serviço atípico. Somar todos os padrões de serviço do feed contaria dia útil, sábado e domingo como se fossem o mesmo dia e inflaria a oferta. A data usada em cada cidade está em [Cidades e datas de referência](https://gilandrade.github.io/process_gtfs/#cidades).

**Faixas horárias.** Os perfis por hora cobrem as 24 horas do dia, em faixas fechadas à esquerda: a faixa 07–08 conta o que parte entre 07:00 e 07:59. Horários a partir de 24:00, que no GTFS designam a madrugada do mesmo dia de serviço, são dobrados: 25:30 conta na faixa 01–02. Por isso, as faixas da madrugada reúnem o serviço do início do dia e o fim da operação noturna.

**Feeds por frequência.** Em São Paulo e no Rio de Janeiro, o GTFS descreve a oferta por intervalos: uma viagem-modelo e o intervalo entre partidas em cada período. Essas janelas são expandidas em uma corrida por partida antes de qualquer contagem. Chama-se **corrida** cada realização de uma viagem do GTFS no dia de referência.

**Horários interpolados.** O GTFS permite omitir o horário nas paradas intermediárias de uma viagem. Nesses casos, o horário é interpolado linearmente ao longo da sequência de paradas, entre as paradas com horário. Isso pesa em Porto Alegre, cujo feed só traz horário na primeira e na última parada de cada viagem.

**Município.** Paradas e trechos de linha recebem o código IBGE do setor censitário do Censo 2022 que os contém. Cada hexágono recebe o município que concentra a maior parte da sua população.

**Cobertura.** Cada feed descreve apenas o serviço de quem o publica. A grade e as linhas de uma cidade avançam sobre municípios vizinhos, mas ali mostram só o serviço desse feed: o transporte local do vizinho não está incluído. Pelo mesmo motivo, um município pode exibir linhas e paradas de mais de um feed: em Franco da Rocha e Jundiaí, por exemplo, os trens da CPTM vêm do feed de São Paulo. Da mesma forma, a ausência de um modo costuma ser do feed, e não da cidade. O metrô e os trens do Rio de Janeiro, o metrô de Belo Horizonte e o Trensurb (Porto Alegre) não constam dos feeds usados.


## Cidades e datas de referência

| Cidade | Fonte do GTFS | Dia útil de referência |
|-----------|-----------|-----------|
| Belo Horizonte (MG) | SUMOB (PBH) | 02/01/2024 (terça) |
| Campinas (SP) | Cittamobi | 21/07/2026 (terça) |
| Curitiba (PR) | Cittamobi | 02/01/2024 (terça) |
| Fortaleza (CE) | Cittamobi | 01/01/2026 (quinta) |
| Franco da Rocha (SP) | Cittamobi | 29/10/2026 (quinta) |
| Jacareí (SP) | Cittamobi | 03/11/2026 (terça) |
| Juazeiro (BA) | Cittamobi | 07/09/2026 (segunda) |
| Juiz de Fora (MG) | Cittamobi | 04/08/2026 (terça) |
| Jundiaí (SP) | Cittamobi | 14/10/2026 (quarta) |
| Maceió (AL) | Cittamobi | 23/07/2026 (quinta) |
| Pelotas (RS) | Cittamobi | 20/08/2026 (quinta) |
| Porto Alegre (RS) | EPTC | 16/09/2025 (terça) |
| Rio de Janeiro (RJ) | SMTR (Prefeitura do Rio) | 04/11/2026 (quarta) |
| Salvador (BA) | Cittamobi | 20/08/2026 (quinta) |
| São Luís (MA) | Cittamobi | 20/05/2025 (terça) |
| São Paulo (SP) | SPTrans e ARTESP | 04/11/2026 (quarta) |
| Sorocaba (SP) | Cittamobi | 21/07/2026 (terça) |
| Uberlândia (MG) | Cittamobi | 19/08/2026 (quarta) |

Datas conforme o processamento de 11/11/2026.


## Fonte dos dados

-   **GTFS.** Na maior parte das cidades, os feeds vêm da API da [Cittamobi](https://www.cittamobi.com.br/). São Paulo (SPTrans), Rio de Janeiro (Secretaria Municipal de Transportes), Belo Horizonte (Superintendência de Mobilidade, SUMOB) e Porto Alegre (EPTC) usam os feeds publicados pelos órgãos gestores, obtidos no catálogo [Mobility Database](https://mobilitydatabase.org/). Em São Paulo, entra também o GTFS da [ARTESP](https://www.artesp.sp.gov.br/), com as linhas de ônibus intermunicipais; ele integra ainda a rede metropolitana do Vale do Paraíba usada no tempo de viagem.
-   **Rede de caminhada e viária.** [OpenStreetMap](https://www.openstreetmap.org/): grafo de caminhada obtido com OSMnx para as distâncias a pé das estações e dos hexágonos; extratos da [Geofabrik](https://download.geofabrik.de/south-america/brazil.html) para o roteamento do tempo de viagem.
-   **Municípios.** Malha de setores censitários do [Censo Demográfico 2022 (IBGE)](https://www.ibge.gov.br/geociencias/organizacao-do-territorio/malhas-territoriais/26565-malhas-de-setores-censitarios-divisoes-intramunicipais.html), usada para atribuir o código do município a paradas, trechos de linha e hexágonos.


**Metodologia completa:** https://gilandrade.github.io/process_gtfs/