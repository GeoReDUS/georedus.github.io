# Indicadores — Tempos de Viagem


## Descrição do indicador

Tempo de viagem porta a porta, em transporte público e a pé, do hexágono clicado até cada hexágono alcançável em até 120 minutos.

| Indicador | Cálculo | Como ler |
|-----------|-----------|-----------|
| **[Tempos de Viagem](https://gilandrade.github.io/process_gtfs/#tempo-de-viagem)** | $t_{o,d} = \operatorname{mediana}_{\tau} \, T(o, d, \tau)$, com $\tau$ entre 07:00 e 08:00 | Um hexágono na faixa de 30–60 min é alcançado em 30 a 60 minutos (mediana), saindo do hexágono clicado entre 7h e 8h. |


## Visão geral

As camadas de mobilidade da [GeoReDUS](https://www.redus.org.br/georedus) descrevem a rede de transporte público (ônibus, BRT, VLT, metrô, trem e balsa) de cidades brasileiras a partir de arquivos [GTFS](https://gtfs.org/pt/), o formato aberto em que operadores e órgãos gestores publicam linhas, paradas e horários.

São quatro grupos de camadas:

-   **Estações**: cada parada com serviço, dimensionada pelas partidas por hora ou pelo número de linhas que a atendem.
-   **Linhas**: o traçado de cada linha, com espessura proporcional à frequência, com filtros por modo de transporte.
-   **Oferta acessível por hexágono**: quantas partidas por hora estão ao alcance de 10 minutos a pé de cada hexágono.
-   **Tempo de viagem**: o tempo de viagem porta a porta, em transporte público e a pé, a partir do hexágono clicado.

Os indicadores por área usam a grade hexagonal [H3](https://h3geo.org/) na resolução 9 (hexágonos de cerca de 0,1 km², com uns 200 m de lado), sobre uma área de estudo formada pela união de faixas de 3 km em torno das paradas de cada feed.


## Detalhamento metodológico

Matriz de tempo de viagem porta a porta entre todos os pares de hexágonos da área de estudo, calculada com o [R5](https://github.com/conveyal/r5) (via [r5py](https://r5py.readthedocs.io/)) a partir do GTFS e da rede viária do OpenStreetMap. Ao clicar em um hexágono, o mapa colore os demais pelo tempo até eles, em faixas de 0–15, 15–30, 30–60, 60–90 e 90–120 minutos. A camada aparece a partir do zoom 9.

-   **Trajeto**: do centro do hexágono de origem ao centro do de destino, combinando caminhada e transporte público. O tempo inclui caminhada, espera, tempo a bordo e transferências.
-   **Horário de partida**: janela de 60 minutos a partir das 07:00 do dia de referência, percorrida minuto a minuto. O valor publicado é a **mediana** dos tempos ao longo da janela, o que amortece a sorte de chegar ao ponto logo antes ou logo depois de um veículo.
-   **Caminhada**: a 4,8 km/h, com no máximo 15 minutos por trecho de acesso ou de chegada ao transporte público. O limite vale também para uma viagem feita inteiramente a pé, então destinos próximos que exigiriam mais de 15 minutos de caminhada só aparecem se houver transporte público que os alcance.
-   **Corte**: só aparecem os destinos alcançáveis em até 120 minutos.
-   **Assimetria**: o tempo de A até B pode diferir do de B até A, por causa de horários e sentidos das linhas.

**Redes metropolitanas.** Onde linhas de cidades vizinhas se cruzam, as cidades são roteadas em uma rede única, com o GTFS de todas: São Paulo, Franco da Rocha e Jundiaí; Rio de Janeiro e Niterói; São José dos Campos e Jacareí. As redes de São Paulo e do Vale do Paraíba incluem também o GTFS da ARTESP e ampliam a grade com hexágonos em torno das paradas das linhas intermunicipais da região. Como os feeds não têm um dia em comum, cada rede usa a data de referência da sua cidade principal (São Paulo, Rio de Janeiro e São José dos Campos), e o serviço do dia de referência de cada feed é aplicado a essa data.

### Definições gerais

**Dia útil de referência.** Todas as camadas descrevem um único dia de serviço, e não a média do período de validade do feed. Em cada cidade, escolhe-se a terça, quarta ou quinta-feira com mais viagens ativas em toda a validade do feed; segunda e sexta ficam de fora por concentrarem serviço atípico. Somar todos os padrões de serviço do feed contaria dia útil, sábado e domingo como se fossem o mesmo dia e inflaria a oferta. A data usada em cada cidade está em [Cidades e datas de referência](https://gilandrade.github.io/process_gtfs/#cidades).

**Faixas horárias.** Os perfis por hora cobrem as 24 horas do dia, em faixas fechadas à esquerda: a faixa 07–08 conta o que parte entre 07:00 e 07:59. Horários a partir de 24:00, que no GTFS designam a madrugada do mesmo dia de serviço, são dobrados: 25:30 conta na faixa 01–02. Por isso, as faixas da madrugada reúnem o serviço do início do dia e o fim da operação noturna.

**Feeds por frequência.** Em São Paulo e no Rio de Janeiro, o GTFS descreve a oferta por intervalos: uma viagem-modelo e o intervalo entre partidas em cada período. Essas janelas são expandidas em uma corrida por partida antes de qualquer contagem. Chama-se **corrida** cada realização de uma viagem do GTFS no dia de referência.

**Horários interpolados.** O GTFS permite omitir o horário nas paradas intermediárias de uma viagem. Nesses casos, o horário é interpolado linearmente ao longo da sequência de paradas, entre as paradas com horário. Isso pesa em Porto Alegre, cujo feed só traz horário na primeira e na última parada de cada viagem.

**Município.** Paradas e trechos de linha recebem o código IBGE do setor censitário do Censo 2022 que os contém. Cada hexágono recebe o município que concentra a maior parte da sua população.

**Cobertura.** Cada feed descreve apenas o serviço de quem o publica. A grade e as linhas de uma cidade avançam sobre municípios vizinhos, mas ali mostram só o serviço desse feed: o transporte local do vizinho não está incluído. Pelo mesmo motivo, um município pode exibir linhas e paradas de mais de um feed: em Franco da Rocha e Jundiaí, por exemplo, os trens da CPTM vêm do feed de São Paulo. Da mesma forma, a ausência de um modo costuma ser do feed, e não da cidade. O metrô e os trens do Rio de Janeiro, o metrô de Belo Horizonte e o Trensurb (Porto Alegre) não constam dos feeds usados.


## Cidades e datas de referência

| Cidade | Fonte do GTFS | Dia útil de referência | Tempo de viagem | Rede de roteamento |
|-----------|-----------|-----------|-----------|-----------|
| Belo Horizonte (MG) | SUMOB (PBH) | 02/01/2024 (terça) | 02/01/2024 (terça) | Própria |
| Campinas (SP) | Cittamobi | 21/07/2026 (terça) | 21/07/2026 (terça) | Própria |
| Curitiba (PR) | Cittamobi | 02/01/2024 (terça) | 02/01/2024 (terça) | Própria |
| Fortaleza (CE) | Cittamobi | 01/01/2026 (quinta) | 01/01/2026 (quinta) | Própria |
| Franco da Rocha (SP) | Cittamobi | 29/10/2026 (quinta) | 04/11/2026 (quarta) | São Paulo (RM) |
| Jacareí (SP) | Cittamobi | 03/11/2026 (terça) | 03/11/2026 (terça) | Vale do Paraíba (RM) |
| Juazeiro (BA) | Cittamobi | 07/09/2026 (segunda) | 07/09/2026 (segunda) | Própria |
| Juiz de Fora (MG) | Cittamobi | 04/08/2026 (terça) | 04/08/2026 (terça) | Própria |
| Jundiaí (SP) | Cittamobi | 14/10/2026 (quarta) | 04/11/2026 (quarta) | São Paulo (RM) |
| Maceió (AL) | Cittamobi | 23/07/2026 (quinta) | 23/07/2026 (quinta) | Própria |
| Pelotas (RS) | Cittamobi | 20/08/2026 (quinta) | 20/08/2026 (quinta) | Própria |
| Porto Alegre (RS) | EPTC | 16/09/2025 (terça) | 16/09/2025 (terça) | Própria |
| Rio de Janeiro (RJ) | SMTR (Prefeitura do Rio) | 04/11/2026 (quarta) | 04/11/2026 (quarta) | Rio de Janeiro (RM) |
| Salvador (BA) | Cittamobi | 20/08/2026 (quinta) | 20/08/2026 (quinta) | Própria |
| São Luís (MA) | Cittamobi | 20/05/2025 (terça) | 20/05/2025 (terça) | Própria |
| São Paulo (SP) | SPTrans e ARTESP | 04/11/2026 (quarta) | 04/11/2026 (quarta) | São Paulo (RM) |
| Sorocaba (SP) | Cittamobi | 21/07/2026 (terça) | 21/07/2026 (terça) | Própria |
| Uberlândia (MG) | Cittamobi | 19/08/2026 (quarta) | 19/08/2026 (quarta) | Própria |

Datas conforme o processamento de 11/11/2026.


## Fonte dos dados

-   **GTFS.** Na maior parte das cidades, os feeds vêm da API da [Cittamobi](https://www.cittamobi.com.br/). São Paulo (SPTrans), Rio de Janeiro (Secretaria Municipal de Transportes), Belo Horizonte (Superintendência de Mobilidade, SUMOB) e Porto Alegre (EPTC) usam os feeds publicados pelos órgãos gestores, obtidos no catálogo [Mobility Database](https://mobilitydatabase.org/). Em São Paulo, entra também o GTFS da [ARTESP](https://www.artesp.sp.gov.br/), com as linhas de ônibus intermunicipais; ele integra ainda a rede metropolitana do Vale do Paraíba usada no tempo de viagem.
-   **Rede de caminhada e viária.** [OpenStreetMap](https://www.openstreetmap.org/): grafo de caminhada obtido com OSMnx para as distâncias a pé das estações e dos hexágonos; extratos da [Geofabrik](https://download.geofabrik.de/south-america/brazil.html) para o roteamento do tempo de viagem.
-   **Municípios.** Malha de setores censitários do [Censo Demográfico 2022 (IBGE)](https://www.ibge.gov.br/geociencias/organizacao-do-territorio/malhas-territoriais/26565-malhas-de-setores-censitarios-divisoes-intramunicipais.html), usada para atribuir o código do município a paradas, trechos de linha e hexágonos.


**Metodologia completa:** https://gilandrade.github.io/process_gtfs/