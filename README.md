# Imersao-dados-python-alura
Projeto de exploração, limpeza e visualização interativa de dados salariais da área de dados com Python, Pandas, Seaborn e Plotly.

📊 Exploração, Limpeza e Visualização de Dados com Python
🧠 Objetivo do Projeto

Este projeto tem como finalidade demonstrar o processo completo de análise de dados utilizando Python, desde a exploração inicial do dataset até a criação de visualizações interativas e dashboards analíticos sobre salários na área de dados.

O projeto utiliza um dataset público contendo informações sobre cargos, senioridade, localização e remuneração de profissionais de tecnologia e ciência de dados.

🧰 Bibliotecas Utilizadas
📌 Pandas

Principal biblioteca para manipulação e análise de dados estruturados.

Utilizações:

Leitura de arquivos CSV

Tratamento e limpeza de dados

Transformações e agrupamentos

Análise estatística

Manipulação de colunas

📌 NumPy

Biblioteca utilizada para cálculos numéricos e manipulação de valores nulos.

Utilizações:

Criação de DataFrames fictícios

Tratamento de valores ausentes (NaN)

Cálculos estatísticos

📌 Matplotlib

Biblioteca base para criação de gráficos estáticos.

Utilizações:

Configuração de figuras

Personalização de títulos, rótulos e tamanho dos gráficos

📌 Seaborn

Biblioteca para visualização estatística com gráficos mais elaborados e intuitivos.

Utilizações:

Gráficos de barras

Histogramas

Boxplots

Análise de distribuição salarial

📌 Plotly

Biblioteca para criação de gráficos interativos e dashboards.

Utilizações:

Gráficos de barras interativos

Gráficos de pizza e donut

Mapas coropléticos (mapa mundial com salários médios)

Visualização dinâmica de dados

📌 PyCountry

Biblioteca utilizada para conversão de códigos de países.

Utilizações:

Conversão do padrão ISO2 para ISO3

Preparação de dados para mapas interativos

📂 Etapas do Projeto
🔎 1. Exploração Inicial dos Dados
Ações realizadas:

Importação do dataset via URL

Visualização das primeiras linhas

Análise estrutural do DataFrame

Identificação de tipos de dados

Estatísticas descritivas

Verificação de dimensão do dataset

Principais métodos utilizados:
.head()
.info()
.describe()
.shape
.columns

🔄 2. Padronização e Tradução dos Dados

Os dados originais possuíam abreviações e nomes em inglês.

Foi realizada a tradução e padronização das variáveis:

Exemplos:

Senioridade

Tipo de contrato

Modalidade de trabalho

Tamanho da empresa

Utilizando dicionários de substituição:

.replace()
.rename()

🧹 3. Limpeza e Tratamento de Dados
Tratamento de valores ausentes:

Substituição pela média

Substituição pela mediana

Preenchimento progressivo (ffill)

Preenchimento regressivo (bfill)

Remoção de registros incompletos

Métodos utilizados:
.isnull()
.fillna()
.dropna()
.assign()
.astype()

📊 4. Análise Exploratória

Foram realizadas análises para identificar padrões e distribuição salarial considerando:

Senioridade

Tipo de trabalho

Distribuição de salários

Técnicas utilizadas:

Contagem de frequência

Agrupamento por categorias

Cálculo de médias salariais

.value_counts()
.groupby()
.mean()
.sort_values()

📈 5. Visualização de Dados
Gráficos Criados
📊 Gráfico de Barras

Distribuição salarial por nível de senioridade.

📉 Histograma

Distribuição geral dos salários.

📦 Boxplot

Identificação de dispersão salarial e outliers.

🌎 6. Dashboard Interativo e Análise Geográfica

Foi desenvolvido um mapa interativo mostrando o salário médio de Cientistas de Dados por país.

Etapas:

Conversão dos países para padrão ISO-3

Filtragem por cargo

Agrupamento por localização

Criação de mapa coroplético

Tecnologias:
plotly.express.choropleth()

📌 Principais Conceitos Aplicados

✔ ETL (Extract, Transform, Load)
✔ Data Cleaning
✔ Data Wrangling
✔ Estatística Descritiva
✔ Data Visualization
✔ Dashboards Interativos
✔ Agrupamentos e Transformações
✔ Manipulação de valores nulos
✔ Conversão e padronização de dados

📁 Exportação do Dataset Final

Após o tratamento e enriquecimento dos dados, foi gerado um novo arquivo:

df_limpo.to_csv('dados-imersao-final.csv', index=False)

🚀 Possíveis Evoluções do Projeto

Construção de dashboard com Streamlit

Criação de filtros dinâmicos

Deploy em ambiente web

Integração com APIs

Automação de atualização dos dados

💡 Aprendizados Obtidos

Este projeto permitiu consolidar conhecimentos em:

Python para análise de dados

Manipulação avançada com Pandas

Visualização estatística

Construção de dashboards interativos

Tratamento e preparação de dados reais
