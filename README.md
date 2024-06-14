# Projeto ETL Zebrinha

## Descrição
O projeto ETL Zebrinha foi desenvolvido com o objetivo de criar um pipeline ETL (Extract, Transform, Load) para coletar, transformar e visualizar dados meteorológicos e de trânsito da cidade de São Paulo. Utilizando APIs públicas, o projeto extrai dados, realiza transformações necessárias para limpeza e padronização, armazena em um banco de dados SQLite e apresenta as informações em um dashboard interativo desenvolvido com Dash e Plotly.

## Propósito
O propósito do projeto é fornecer uma ferramenta que permita a visualização clara e interativa dos dados de clima e trânsito, ajudando a identificar padrões, tendências e fornecer insights úteis para tomadas de decisão.

## Fluxo Esperado

1. **Extração de Dados:**
    - **API de Clima:** Utiliza a API do OpenWeatherMap (https://openweathermap.org/api) para coletar dados climáticos.
    - **API de Trânsito:** Utiliza a API do Google Maps Directions (https://developers.google.com/maps/documentation/directions/overview) para coletar dados de trânsito.

2. **Limpeza e Transformação:**
    - Remoção de duplicatas e registros inválidos.
    - Padronização de formatos (datas, números, etc.).
    - Tratamento de valores nulos ou ausentes.
    - Identificação de tendências ou padrões nos dados.

3. **Modelagem de Dados:**
    - Definição do esquema de banco de dados, incluindo tabelas, relacionamentos, índices e chaves primárias/estrangeiras.

4. **Integração com o Banco de Dados:**
    - Conexão e carregamento dos dados transformados no banco de dados SQLite.

5. **Visualização de Dados:**
    - Criação de um dashboard interativo utilizando Dash e Plotly para visualizar dados de clima e trânsito.

## Tecnologias Utilizadas
- **Python**: Linguagem de programação principal utilizada no desenvolvimento do projeto.
- **SQLite**: Banco de dados utilizado para armazenar os dados.
- **Pandas**: Biblioteca Python utilizada para manipulação e análise de dados.
- **Plotly**: Biblioteca Python utilizada para criação de gráficos interativos.
- **Dash**: Framework utilizado para criar aplicações web interativas.
- **APIs**: OpenWeatherMap e Google Maps Directions para extração de dados.
- **GitHub**: Plataforma utilizada para versionamento de código e colaboração.

### Proposta do Dashboard
A proposta do dashboard é oferecer uma visualização clara e interativa dos dados meteorológicos de São Paulo. Ele permite aos usuários:
- Visualizar a variação de temperatura ao longo do tempo.
- Obter informações sobre a média e o desvio padrão da temperatura.
- Verificar os horários de nascer e pôr do sol.

### Gráfico de Temperatura
O gráfico de temperatura exibe a variação da temperatura ao longo do tempo, preenchendo a área entre as linhas para uma melhor visualização. O gráfico é interativo e foi criado utilizando a biblioteca Plotly.

![image](https://github.com/PATRICIAJUNQUEIRA/Zebrinha_ETL/assets/96187596/90460970-dd58-4430-9983-48ce38df6244)
![image](https://github.com/PATRICIAJUNQUEIRA/Zebrinha_ETL/assets/96187596/df70f853-2af3-4e33-87e0-329e665a8c23)


### Informações Adicionais
Além do gráfico, o dashboard exibe uma caixa de texto com informações adicionais:
- Média da Temperatura
- Desvio Padrão da Temperatura
- Horários de Nascer e Pôr do Sol
