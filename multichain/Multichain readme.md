# Multichain Transaction Dataset Generator

This project generates a synthetic dataset of blockchain transactions across multiple chains (e.g., Ethereum, BSC, Solana, Starknet, etc.). It creates 3000 randomly simulated transactions with various metadata like transaction IDs, token transfers, timestamps, transaction fees, and more.

## 📁 Features

* Simulates realistic blockchain transaction data for:

  * Ethereum
  * Binance Smart Chain (BSC)
  * Polygon
  * Starknet
  * Avalanche
  * Solana
* Includes key transaction details:

  * Transaction ID
  * Timestamp
  * From/To address
  * Token
  * Amount
  * Transaction Fee
  * Purpose (`transfer`, `swap`, `stake`, etc.)
  * Status (`success`, `failed`, `pending`)
* Saves dataset as a CSV file
* Visualizes chain distribution using a bar chart

## 🧪 Dependencies

* Python 3.6+
* pandas
* matplotlib
* Google Colab (optional for running interactively)

## 🚀 How to Use

1. Clone or open the script in [Google Colab](https://colab.research.google.com/).
2. Run all cells to generate and preview the dataset.
3. The dataset will be saved as `multichain_transactions_3000.csv`.
4. The CSV can be downloaded directly via Colab using:

```python
from google.colab import files
files.download("multichain_transactions_3000.csv")
```

## 📊 Sample Output

```text
chain     | transaction_id | from_address | to_address | amount | token | transaction_fee | purpose         | status
----------|----------------|--------------|------------|--------|-------|------------------|------------------|--------
Ethereum  | 0xabc...        | 0x123...     | 0x456...   | 856.43 | ETH   | 0.002778         | transfer         | success
Solana    | 0xdef...        | 0x789...     | 0xabc...   | 225.78 | SOL   | 0.000041         | stake            | success
```

## 📈 Data Summary

* Total Transactions: 3000
* Columns: 10
* Typical transaction amounts: 10–1000
* Fee ranges vary by chain

## 🛠 Use Cases

* Blockchain data simulations
* ML model training for fraud detection
* Exploratory Data Analysis (EDA) for Web3
* Synthetic datasets for analytics dashboards

## 📃 License

This project is open source and free to use under the MIT License.

---

Would you like this saved as a file?
