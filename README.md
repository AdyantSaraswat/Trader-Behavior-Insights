# Trader-Behavior-Insights
# 📊 Market Sentiment vs Trader Behavior Analysis

This project explores how **trader performance (profitability, risk, and trade volume)** aligns or diverges from **overall Bitcoin market sentiment (Fear vs Greed)**.
The objective is to uncover patterns and insights that can help design **smarter, sentiment-aware trading strategies**.

---

## 🧠 Project Overview

We combine two datasets:

1. **Bitcoin Market Sentiment Dataset**

   * Columns: `timestamp`, `value`, `classification`, `date`
   * Represents daily market emotions ranging from *Extreme Fear* to *Extreme Greed*.

2. **Hyperliquid Trader Data**

   * Columns: `account`, `execution price`, `size`, `side`, `closedPnL`, `leverage`, etc.
   * Includes trader activity, profit/loss, and leverage data.

The analysis investigates whether trading behavior and profitability change under different market sentiment phases.

---

## 🗂️ Repository Structure

```
ds_spidy/
├── notebook_1.ipynb        # Main Colab notebook (EDA + Analysis)
├── notebook_2.ipynb        # (Optional) Secondary notebook
├── csv_files/              # Raw and processed datasets
│   ├── sentiment_data.csv
│   ├── trade_history.csv
│   └── processed_trades.csv
├── outputs/                # Generated visualizations
│   ├── profit_loss_dist.png
│   ├── trade_size_log.png
│   └── sentiment_vs_trades.png
├── ds_report.pdf           # Final report summarizing insights
└── README.md               # Project documentation
```

---

## ⚙️ How to Run the Project

1. **Open the Notebook in Google Colab**

   * [Colab Notebook Link]((https://colab.research.google.com/drive/13jKEUeIxo4Nioq8M-AYpeA_-mwtN45pD))
   * Set access to *“Anyone with the link can view”*.

2. **Upload CSV Files**

   * Place the provided datasets inside `/csv_files/` or upload directly in Colab.

3. **Run All Cells**

   * The notebook will automatically generate plots and save them in `/outputs/`.

4. **Review Outputs**

   * Check all PNG files in `/outputs/` for visual insights.

5. **Read the Report**

   * Refer to `ds_report.pdf` for the final conclusions and trading insights.

---

## 📈 Key Insights

* Most trades yield **near-zero profit**, implying frequent low-margin trading.
* Trade sizes are **heavily right-skewed** — a few large trades dominate total volume.
* **Greed phases** show higher leverage and trade sizes.
* **Fear phases** correspond with lower activity and reduced risk exposure.
* Sentiment impacts **risk appetite**, not necessarily **profitability**.

---

## 🧾 Requirements

The notebook uses standard Python libraries available in Google Colab:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

No manual installation is required.

---

## 🧑‍💻 Author

**Name:** Your Full Name
**Project Folder:** `ds_adyant_saraswat`
**Colab Notebook:** [Link to Colab](PASTE_YOUR_COLAB_LINK_HERE)
**GitHub Repository:** [Link to Repo](PASTE_YOUR_GITHUB_LINK_HERE)

---


