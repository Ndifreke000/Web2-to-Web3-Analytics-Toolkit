# 🚀 Blockchain Transaction Generator

> A simple yet powerful tool to generate randomized blockchain transaction data for testing and development purposes.

## 📋 Overview

This Python script creates a dataset of randomized blockchain transactions that mimic real-world Ethereum-like blockchain activity. The generated data includes transaction IDs, timestamps, wallet addresses, amounts, tokens, and transaction statuses - perfect for testing blockchain applications, data analysis, or educational purposes.

## ✨ Features

- 📊 Generates 1001 random blockchain transactions
- 🔄 Creates realistic transaction IDs and Ethereum-like addresses
- 💰 Includes popular tokens (ETH, USDT, DAI, USDC, WBTC)
- ⏱️ Timestamps within a configurable time range
- 💸 Randomized transaction amounts between 50 and 500
- 🟢 Various transaction statuses (success, failed, pending)
- 💾 Exports data to CSV format

## 🔧 Requirements

- Python 3.6+
- pandas
- numpy
- openpyxl (for Excel export functionality)

## 📥 Installation

```bash
# Install required packages
pip install pandas numpy openpyxl
```

## 🚀 Usage

### In Google Colab

1. Open the notebook in Google Colab
2. Run the installation cell: `!pip install pandas numpy openpyxl`
3. Run the script
4. The CSV file will be automatically downloaded to your local machine

### On Your Local Machine

1. Save the script as `blockchain_generator.py`
2. Run it with Python:

```bash
python blockchain_generator.py
```

3. Find the generated CSV file in your working directory

## 🧩 How It Works

The script generates random blockchain transaction data using these key functions:

- `generate_random_address()`: Creates Ethereum-like wallet addresses
- `generate_random_transaction_id()`: Creates unique transaction hashes
- `generate_random_token()`: Selects a token from a predefined list
- `generate_random_status()`: Assigns a transaction status
- `generate_random_amount()`: Generates transaction amounts
- `generate_random_timestamp()`: Creates timestamps within a specified range

Each transaction record contains:
- `transaction_id`: A unique hash identifying the transaction
- `timestamp`: When the transaction occurred
- `from_address`: The sender's wallet address
- `to_address`: The recipient's wallet address
- `amount`: The amount transferred
- `token`: The cryptocurrency token used
- `status`: The transaction status

## 🛠️ Customization

You can easily modify the script to suit your needs:

- Change the number of transactions (default: 1001)
- Adjust the time range (default: 6-hour period on Jan 1, 2025)
- Modify the token list
- Change the amount range
- Add additional transaction properties

## 📊 Sample Output

The generated dataset includes fields like:

| transaction_id | timestamp | from_address | to_address | amount | token | status |
|----------------|-----------|--------------|------------|--------|-------|--------|
| 0x11a09ecb... | 2025-01-01T14:24:00Z | 0x5d0dba... | 0xbaace... | 381.46 | ETH | success |
| 0xb53cf6d2... | 2025-01-01T14:40:00Z | 0x07df25... | 0x1dcfa... | 72.92 | WBTC | pending |

## 📝 License

This project is available as open source under the terms of the MIT License.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 🙏 Acknowledgements

- Thanks to all the open-source contributors who make projects like this possible
- Special thanks to the pandas and numpy communities

---

Made with ❤️ for blockchain developers and data enthusiasts
