# :earth_americas: GDP dashboard template

A simple Streamlit app showing the GDP of different countries in the world.

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://gdp-dashboard-template.streamlit.app/)

📊 Dashboard Interativo de PIB Mundial (GDP)
Este projeto é uma ferramenta de Visualização de Dados interativa construída com Python e Streamlit. O sistema processa dados macroeconómicos complexos do Banco Mundial para fornecer uma visão clara e comparativa das tendências do PIB global entre 1960 e 2022.

🚀 Funcionalidades
Filtragem Dinâmica: O utilizador pode definir o intervalo de anos e selecionar países específicos para comparação em tempo real.

Análise de Séries Temporais: Gráfico de linhas responsivo que demonstra a evolução económica ao longo das décadas.

Métricas de Desempenho: Cálculo automático do crescimento do PIB (Delta) entre os anos selecionados.

Pipeline de Dados Otimizado: Implementação de caching (@st.cache_data) para processar ficheiros CSV de forma eficiente, evitando operações de I/O redundantes.

🛠️ Stack Tecnológica
Linguagem: Python 3.14

Manipulação de Dados: Pandas (Operações de Melt e Pivot)

Frontend/UI: Streamlit

Infraestrutura: Docker & .devcontainer (configurado para um workflow nativo em WSL2/Linux)

🏗️ Arquitetura e Clean Code
Seguindo os princípios de Clean Architecture, o projeto está organizado em:

Camada de Dados: Ingestão de CSV bruto e armazenamento estruturado no diretório /data.

Camada de Lógica: Tratamento de dados (Data Wrangling) com Pandas para transformar o formato "wide" do Banco Mundial em séries temporais estruturadas.

Camada de Apresentação: Interface interativa com gestão de estado reativa.

### How to run it on your own machine

1. Install the requirements

   ```
   $ pip install -r requirements.txt
   ```

2. Run the app

   ```
   $ streamlit run streamlit_app.py

   ```
git clone https://github.com/OlgarioDev/gdp-dashboard.git
cd gdp-dashboard

📄 Licença
Este projeto está licenciado sob a Apache License 2.0 - consulta o ficheiro LICENSE para mais detalhes.
