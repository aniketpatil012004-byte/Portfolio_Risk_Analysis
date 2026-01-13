# Portfolio Risk Analysis: Monte Carlo Simulation (VaR)

## 📌 Project Overview
This project performs a **Value at Risk (VaR)** analysis on a diversified portfolio of Indian stocks using **Monte Carlo Simulations**. By analyzing 15 years of historical data, the model estimates the potential loss of a portfolio over a specific time horizon (e.g., 5 days) with varying confidence levels (95% and 99%).

The goal is to quantify financial risk and understand the probability of extreme market movements affecting a hypothetical portfolio worth ₹10,000,000 (1 Crore).

## 📊 Stock Portfolio
The analysis is based on a weighted portfolio consisting of the following major NSE companies:
* **NTPC** (Energy)
* **TCS** (IT Services)
* **ITC** (FMCG)
* **CIPLA** (Pharmaceuticals)
* **RELIANCE** (Energy/Conglomerate)

## 🛠️ Technologies Used
* **Python:** Core programming language.
* **YFinance:** To download historical stock market data.
* **Pandas & NumPy:** For data manipulation, logarithmic return calculations, and covariance matrix generation.
* **SciPy:** For statistical functions (norm/Z-score).
* **Matplotlib:** For visualizing the distribution of simulated returns.

## ⚙️ Methodology
1.  **Data Extraction:** Fetched adjusted closing prices for the last 15 years.
2.  **Statistical Analysis:** Calculated daily Log Returns, Mean Returns, and the Covariance Matrix.
3.  **Monte Carlo Simulation:** * Simulated **10,000** potential future market scenarios based on historical volatility (Standard Deviation) and correlations.
    * Used random Z-scores to project portfolio gain/loss.
4.  **VaR Calculation:** Determined the maximum expected loss at **95%** and **99%** confidence intervals.

## 📈 Results
The simulation outputs a distribution of potential profits and losses. The **Value at Risk (VaR)** is marked to show the "danger zone" (the worst-case scenarios).

*(You can upload a screenshot of your histogram here later!)*

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  Install required libraries:
    ```bash
    pip install numpy pandas yfinance matplotlib scipy
    ```
3.  Run the notebook `Portfolio_VaR_Analysis.ipynb`.

## ⚠️ Disclaimer
This project is for educational purposes only. It is not financial advice. The simulations are based on historical assumptions which may not predict future market performance.
