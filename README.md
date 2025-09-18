📂 Trader Behavior vs Market Sentiment Analysis

🔹 Overview

This project analyzes the relationship between trader behavior (profitability, trade volume, direction) and market sentiment (Fear vs Greed).
The analysis combines two datasets:

Historical Trader Data (Hyperliquid)

Bitcoin Fear & Greed Index

The objective is to uncover how trading decisions align (or diverge) from overall market sentiment, and to identify signals for smarter trading strategies.

🔹 Project Structure

ds_<your_name>/
├── notebook_1.ipynb       # Main Colab notebook with code & analysis

├── notebook_2.ipynb       # (Optional) Additional experiments

├── csv_files/             # Input & processed CSVs

│   ├── trader_data.csv

│   ├── sentiment_data.csv

│   ├── cleaned_trader_data.csv

│   └── cleaned_sentiment_data.csv

├── outputs/               # Charts, plots, and visualizations

│   ├── trade_side_distribution.png

│   ├── pnl_by_sentiment.png

│   ├── volume_vs_sentiment.png

│   └── buy_sell_sentiment.png

├── ds_report.pdf          # Final summarized report

└── README.md              # Setup & usage instructions

🔹 Setup Instructions

Open in Google Colab

Upload this folder to Google Drive.

Open notebook_1.ipynb in Colab.

Mount Google Drive in Colab

from google.colab import drive
drive.mount('/content/drive')


Navigate to Project Folder

import os
base_path = "/content/drive/MyDrive/ds_<your_name>"
os.chdir(base_path)


Install Dependencies (if needed)

!pip install pandas matplotlib seaborn pypandoc

🔹 Usage

Run all cells in notebook_1.ipynb.

Cleaned CSVs will be stored in csv_files/.

Visual outputs (charts/plots) will be saved in outputs/.

Final report (ds_report.pdf) will summarize insights.

🔹 Key Insights (Preview)

Fear States → More SELL trades, higher volume, lower profitability.

Greed States → More BUY trades, lower volume, higher profitability.

High Volume in Fear → Panic-driven market moves.

Potential for contrarian strategies: buy during Fear, sell during Greed.

🔹 Tools & Libraries

Python (Google Colab)

Pandas, Matplotlib, Seaborn

pypandoc (for report generation)

🔹 Author

👤 Yash Sunilbhai Patel

📧 yashpatelndb@gmail.com
