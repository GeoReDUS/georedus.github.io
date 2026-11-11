# Linhas — BRT


## Descrição do indicador

Linhas de BRT, com espessura proporcional à frequência média (partidas por hora) no período selecionado.

| Indicador | Cálculo | Como ler |
|-----------|-----------|-----------|
| **[BRT](https://gilandrade.github.io/process_gtfs/#linhas)** | $f_r = \frac{1}{n_H} \sum_{h \in H} \max_d n_{r,d,h}$, só linhas com `route_type` 702 | Uma linha de BRT com frequência 12 parte, em média, a cada 5 minutos no seu sentido mais frequente durante o período selecionado. |


## Visão geral

As camadas de mobilidade da [GeoReDUS](https://www.redus.org.br/georedus) descrevem a rede de transporte público (ônibus, BRT, VLT, metrô, trem e balsa) de cidades brasileiras a partir de arquivos [GTFS](https://gtfs.org/pt/), o formato aberto em que operadores e órgãos gestores publicam linhas, paradas e horários.

São quatro grupos de camadas:

-   **Estações**: cada parada com serviço, dimensionada pelas partidas por hora ou pelo número de linhas que a atendem.
-   **Linhas**: o traçado de cada linha, com espessura proporcional à frequência, com filtros por modo de transporte.
-   **Oferta acessível por hexágono**: quantas partidas por hora estão ao alcance de 10 minutos a pé de cada hexágono.
-   **Tempo de viagem**: o tempo de viagem porta a porta, em transporte público e a pé, a partir do hexágono clicado.

Os indicadores por área usam a grade hexagonal [H3](https://h3geo.org/) na resolução 9 (hexágonos de cerca de 0,1 km², com uns 200 m de lado), sobre uma área de estudo formada pela união de faixas de 3 km em torno das paradas de cada feed.


## Detalhamento metodológico

Cada feição é o traçado de uma linha (rota do GTFS) dentro de um município. Linhas intermunicipais são recortadas em um trecho por município, para que o trecho comum não seja desenhado duas vezes quando vários municípios estão visíveis. O traçado é o da primeira viagem da linha no feed, então uma rota de ida e volta aparece com o traçado de um só sentido.

**Frequência.** Para a linha $r$ e a faixa horária $h$, conta-se o número de corridas $n_{r,d,h}$ que **iniciam** na faixa em cada sentido $d$. Uma corrida que apenas atravessa a faixa não representa nova oportunidade de embarque. Toma-se o sentido mais frequente: somar ida e volta faria o intervalo parecer metade do que o passageiro de fato espera em um ponto. O headway da faixa é $60 / \max_d n_{r,d,h}$ minutos, e feeds sem indicação de sentido tratam a linha como de sentido único. O cálculo supõe corridas regulares dentro da hora.

No mapa, a espessura da linha é a frequência média, em partidas por hora, nas faixas do período selecionado ($H$, com $n_H$ faixas). Faixas em que nenhuma corrida da linha se inicia contam como zero. A escala de espessuras é fixa, calculada sobre o dia inteiro de todas as linhas do município: mover o controle de horário muda a espessura de cada linha, mas não a legenda.

As informações exibidas ao passar o cursor são:

-   **Tipo da linha**: o código `route_type` do GTFS (0 bonde/VLT, 1 metrô, 2 trem, 3 ônibus, 4 balsa, 702 BRT; 200 e 700 são tipos estendidos de ônibus usados no Rio de Janeiro).
-   **Paradas**: paradas distintas que a linha atende no feed, sem recorte de dia ou de horário.
-   **Headway mínimo**: o menor headway da linha entre as 24 faixas do dia.

As camadas por modo filtram as linhas pelo `route_type` declarado no feed. A classificação segue o que o feed declara: um sistema de BRT cadastrado como ônibus comum aparece na camada Ônibus. Cada camada por modo só fica disponível nos municípios em que o feed traz aquele modo.

### Definições gerais

**Dia útil de referência.** Todas as camadas descrevem um único dia de serviço, e não a média do período de validade do feed. Em cada cidade, escolhe-se a terça, quarta ou quinta-feira com mais viagens ativas em toda a validade do feed; segunda e sexta ficam de fora por concentrarem serviço atípico. Somar todos os padrões de serviço do feed contaria dia útil, sábado e domingo como se fossem o mesmo dia e inflaria a oferta. A data usada em cada cidade está em [Cidades e datas de referência](https://gilandrade.github.io/process_gtfs/#cidades).

**Faixas horárias.** Os perfis por hora cobrem as 24 horas do dia, em faixas fechadas à esquerda: a faixa 07–08 conta o que parte entre 07:00 e 07:59. Horários a partir de 24:00, que no GTFS designam a madrugada do mesmo dia de serviço, são dobrados: 25:30 conta na faixa 01–02. Por isso, as faixas da madrugada reúnem o serviço do início do dia e o fim da operação noturna.

**Feeds por frequência.** Em São Paulo e no Rio de Janeiro, o GTFS descreve a oferta por intervalos: uma viagem-modelo e o intervalo entre partidas em cada período. Essas janelas são expandidas em uma corrida por partida antes de qualquer contagem. Chama-se **corrida** cada realização de uma viagem do GTFS no dia de referência.

**Horários interpolados.** O GTFS permite omitir o horário nas paradas intermediárias de uma viagem. Nesses casos, o horário é interpolado linearmente ao longo da sequência de paradas, entre as paradas com horário. Isso pesa em Porto Alegre, cujo feed só traz horário na primeira e na última parada de cada viagem.

**Município.** Paradas e trechos de linha recebem o código IBGE do setor censitário do Censo 2022 que os contém. Cada hexágono recebe o município que concentra a maior parte da sua população.

**Cobertura.** Cada feed descreve apenas o serviço de quem o publica. A grade e as linhas de uma cidade avançam sobre municípios vizinhos, mas ali mostram só o serviço desse feed: o transporte local do vizinho não está incluído. Pelo mesmo motivo, um município pode exibir linhas e paradas de mais de um feed: em Franco da Rocha e Jundiaí, por exemplo, os trens da CPTM vêm do feed de São Paulo. Da mesma forma, a ausência de um modo costuma ser do feed, e não da cidade. O metrô e os trens do Rio de Janeiro, o metrô de Belo Horizonte e o Trensurb (Porto Alegre) não constam dos feeds usados.


## Cidades e datas de referência

| Cidade | Fonte do GTFS | Modos no feed | Dia útil de referência |
|-----------|-----------|-----------|-----------|
| Rio de Janeiro (RJ) | SMTR (Prefeitura do Rio) | ônibus, BRT | 04/11/2026 (quarta) |

Datas conforme o processamento de 11/11/2026.


## Fonte dos dados

-   **GTFS.** Na maior parte das cidades, os feeds vêm da API da [Cittamobi](https://www.cittamobi.com.br/). São Paulo (SPTrans), Rio de Janeiro (Secretaria Municipal de Transportes), Belo Horizonte (Superintendência de Mobilidade, SUMOB) e Porto Alegre (EPTC) usam os feeds publicados pelos órgãos gestores, obtidos no catálogo [Mobility Database](https://mobilitydatabase.org/). Em São Paulo, entra também o GTFS da [ARTESP](https://www.artesp.sp.gov.br/), com as linhas de ônibus intermunicipais; ele integra ainda a rede metropolitana do Vale do Paraíba usada no tempo de viagem.
-   **Rede de caminhada e viária.** [OpenStreetMap](https://www.openstreetmap.org/): grafo de caminhada obtido com OSMnx para as distâncias a pé das estações e dos hexágonos; extratos da [Geofabrik](https://download.geofabrik.de/south-america/brazil.html) para o roteamento do tempo de viagem.
-   **Municípios.** Malha de setores censitários do [Censo Demográfico 2022 (IBGE)](https://www.ibge.gov.br/geociencias/organizacao-do-territorio/malhas-territoriais/26565-malhas-de-setores-censitarios-divisoes-intramunicipais.html), usada para atribuir o código do município a paradas, trechos de linha e hexágonos.


**Metodologia completa:** https://gilandrade.github.io/process_gtfs/