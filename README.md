# Data Exploration and Visualization Tool

This project is a Python-based tool for loading, analyzing, and visualizing datasets from CSV files. It supports exploratory data analysis (EDA), including statistical summaries and graphical visualizations. The code can load datasets from URLs, including Google Drive links, and generate insights using libraries like `pandas`, `matplotlib`, and `seaborn`.

## Main Features

### 1. Load Data:
- **Function:** `carregar_dados(url, tipo_arquivo='CSV')`
- **Description:** Loads data from a CSV file using a URL. If the URL is from Google Drive, it extracts the file ID and downloads the data. The function reads the data and returns a pandas DataFrame.
  
### 2. Exploratory Data Analysis (EDA):
- **Function:** `analise_exploratoria(df)`
- **Description:** Displays the first few rows, general information, and descriptive statistics of the DataFrame. It also generates graphical visualizations, including histograms, line charts, scatter plots, boxplots, and a correlation matrix.

### 3. Visualizations:
- **Function:** `plot_histograma(df)`
  - Plots a histogram for a randomly selected numeric column.
  
- **Function:** `plot_grafico_de_linha(df)`
  - Plots a line chart for two randomly selected numeric columns.

- **Function:** `plot_grafico_de_dispersao(df)`
  - Plots a scatter plot between two randomly selected numeric columns.

- **Function:** `plot_boxplot(df)`
  - Plots a boxplot for all numeric columns.

- **Function:** `identificacao_correlacoes(df)`
  - Generates a correlation matrix between numeric columns in the DataFrame.

### 4. Expert Analysis:
- **Function:** `analise_especialista()`
  - Adds an expert analysis or insights based on the data explored.

### 5. Main Execution:
- **Function:** `main(urls)`
  - Processes a list of URLs, loads and analyzes the data for each URL, and performs exploratory and expert analysis.

## Requirements

- `pandas`
- `matplotlib`
- `seaborn`
- `requests`

Install the required Python libraries by running:

```bash
pip install pandas matplotlib seaborn requests
