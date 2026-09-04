# 📈 Extracting and Visualizing Stock Data

## Technologies

- Python
- Jupyter Notebook
- Pandas
- yfinance
- Requests
- BeautifulSoup
- Matplotlib

## Project structure

```text
stock-data-visualization/
│
├── Extracting_and_Visualizing_Stock_Data.ipynb
├── requirements.txt
├── README.md
├── SOURCES.txt
├── .gitignore
└── output/
    ├── tesla_revenue.csv
    └── gme_revenue.csv
```

The `output/` directory is generated when the notebook is run.

## Run locally in VS Code

### 1. Clone or download

Open this repository in VS Code.

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Windows:

```powershell
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Open the notebook

Open:

```text
Extracting_and_Visualizing_Stock_Data.ipynb
```

Install/select the VS Code **Jupyter** kernel and choose the `.venv` environment.

### 5. Run

Run all cells from top to bottom.

Internet access is required because stock data and the revenue HTML pages are retrieved online.

## Web scraping approach

The project intentionally demonstrates both:

```text
requests
   ↓
HTML response
   ↓
BeautifulSoup
   ↓
HTML tables
   ↓
pandas.read_html()
   ↓
DataFrame
   ↓
Data cleaning
```

The revenue pages are IBM Skills Network-hosted HTML snapshots used by the original lab. This avoids depending on direct automated access to Macrotrends' current website while still demonstrating genuine web scraping.

## GitHub

Recommended repository name:

```text
stock-data-visualization
```

Do not commit:

```text
.venv/
__pycache__/
.ipynb_checkpoints/
```

These are already included in `.gitignore`.

## Portfolio description

> A Python data-analysis project that extracts Tesla and GameStop historical stock prices using yfinance, scrapes quarterly revenue tables from HTML using Requests and BeautifulSoup, cleans the financial data with Pandas, and visualizes stock price and revenue using Matplotlib.

## Disclaimer

This project is educational and is not financial advice.
