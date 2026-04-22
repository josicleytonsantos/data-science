# 📊 B3 Stock Analysis: PETR4 vs ITUB4

This project performs an exploratory data analysis (EDA) of two major Brazilian stocks:

* **PETR4** – Petrobras
* **ITUB4** – Itaú Unibanco

The analysis focuses on price behavior, daily variation, and volatility using Python.

---

## 🚀 Objectives

* Analyze historical stock prices
* Compare performance between assets
* Study daily price variations
* Visualize volatility through distributions

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – data manipulation
* **NumPy** – numerical operations
* **Matplotlib** – data visualization
* **yFinance** – data collection

---

## 📥 Data Source

Stock data is obtained using the `yfinance` library, which retrieves historical market data from Yahoo Finance.

```python
import yfinance as yf

df = yf.download(['PETR4.SA', 'ITUB4.SA'],
                 start='2025-10-01',
                 end='2026-04-01')
```

---

## 📊 Project Structure

```
├── notebook.ipynb        # Main analysis notebook
├── stock_analysis.png    # Generated plot
├── stock_analysis.pdf    # Exported figure
├── stock_analysis.svg    # Vector version
└── README.md             # Project documentation
```

---

## 📈 Visualizations

The project includes:

### 🔹 Line Chart

* Displays stock price evolution over time
* Allows direct comparison between PETR4 and ITUB4

### 🔹 Histograms

* Show distribution of daily price changes
* Highlight average variation using a reference line

---

## 📉 Key Analyses

### ✔️ Price Evolution

Tracks how each stock behaves over time.

### ✔️ Daily Variation

Uses `.diff()` to analyze day-to-day price changes.

### ✔️ Volatility Insight

* Wider distributions → higher volatility
* Narrow distributions → more stability

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/b3-stock-analysis.git
```

2. Install dependencies:

```bash
pip install pandas numpy matplotlib yfinance
```

3. Run the notebook:

```bash
jupyter notebook
```

---

## 📌 Example Output

The generated visualization includes:

* Combined line chart
* Histograms for both stocks
* Mean variation indicators

---

## 📚 Future Improvements

* Add moving averages (MA20, MA50)
* Compute daily returns (`pct_change`)
* Correlation analysis
* Interactive dashboards (Plotly)

---

## 👨‍💻 Author

Josicleyton Santos  
Production Engineer & M.Sc. in Computer Science  
Focus: Data Science, Optimization, and Computational Intelligence

---

## 📄 License

This project is for educational purposes.