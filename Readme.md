Here is the **README.md content only** in clean copy-paste format.

---

# PrimeTradeAI – Sentiment Driven Trader Performance Analysis

## Project Overview

This project analyzes how market sentiment regimes impact trader performance and behavior.

Sentiment Regimes:

* Extreme Fear
* Fear
* Neutral
* Greed
* Extreme Greed

The objective is to evaluate profitability, risk characteristics, and behavioral shifts across regimes and derive actionable trading insights.

---

## Methodology

### Part A – Data Preparation

* Loaded trade-level and sentiment datasets
* Checked for missing values and duplicates
* Converted timestamps to daily format
* Merged datasets at daily level
* Engineered key metrics:

  * Daily PnL per account
  * Win day indicator
  * Average trade size
  * Number of trades per day
  * Long/short ratio
  * Volatility (standard deviation of daily PnL)
  * Risk-adjusted return (mean / volatility)
  * Payoff ratio (average win / average loss)

---

### Part B – Regime Analysis

Performance was evaluated across sentiment regimes using:

* Mean PnL
* Win rate
* Volatility
* Risk-adjusted return
* Payoff ratio

Behavioral analysis included:

* Trade frequency variation
* Position sizing changes
* Long/short bias shifts

Interactive visualizations were created using Plotly.

---

## Key Insights

1. Neutral regime delivers the highest risk-adjusted return due to significantly lower volatility.
2. Extreme Greed provides the strongest combination of win probability and payoff quality.
3. Fear regime generates the highest raw returns but exhibits elevated dispersion risk.
4. Standard Greed underperforms across most performance metrics.
5. Traders increase position sizing most aggressively during Fear conditions, amplifying volatility.

---

## Strategy Implications

* Allocate core capital during Neutral regimes due to superior capital efficiency.
* Increase tactical exposure during Extreme Greed environments.
* Apply risk control during Fear due to volatility expansion.
* Reduce exposure during Standard Greed regimes.

---

## Tools Used

* Python
* Pandas
* NumPy
* Plotly

---

## Installation

Install required packages:

```
pip install pandas numpy plotly kaleido
```

---

## How to Run

```
jupyter notebook
```

Open the notebook and run all cells.

---

## Saving Figures

Save as PNG:

```
fig.write_image("figure_name.png", scale=2)
```

Save as interactive HTML:

```
fig.write_html("figure_name.html")
```

---

That’s it. Copy. Paste. Commit. Submit.
