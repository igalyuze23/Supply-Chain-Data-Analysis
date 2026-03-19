# 🚚 Global Supply Chain & Fraud Analysis (Memory-Efficient Approach)

## 📌 Project Overview
This project analyzes a massive dataset of over **180,000 supply chain transactions**. The goal was to extract actionable business intelligence regarding logistics bottlenecks, profitability, and fraud detection. 

Instead of relying on heavy data libraries that load everything into memory, this project was built using **Core Python (Standard Library)** to demonstrate memory-efficient data processing (Stream Processing) and a deep understanding of data structures.

## 🛠️ Technical Highlight: Why Core Python?
Processing 180,000+ rows can be memory-intensive. I optimized the script by:
* Using the built-in `csv.DictReader` to read the file **row-by-row** (Stream Processing) instead of loading the entire dataset into RAM.
* Utilizing **Dictionaries** to aggregate data (counts, sums) on the fly, which keeps the memory footprint minimal.
* Automatically generating a multi-sheet executive report using `openpyxl`.

## 📊 Key Business Insights Discovered
1. **Fraud Detection:** Identified the top targeted product categories for suspected fraud, with **Cleats (560 cases)** and **Men's Footwear (516 cases)** leading the risk chart.
2. **Logistics Bottlenecks:** Discovered that **Central Asia** and **Central Africa** suffer from the highest average delivery delays.
3. **Profitability:** Analyzed the direct impact of delivery status (Late vs. On-Time) on the average profit per order.

## 💻 Technologies Used
* **Python:** Standard Libraries (`csv`, `os`) for memory-efficient data processing.
* **Openpyxl:** For automated Excel reporting.
* **Dataset:** DataCo Smart Supply Chain (Due to GitHub's file size limits, the raw 180k rows CSV is not uploaded, but the script is ready to run on it).

## 🚀 How to Run
1. Download the raw dataset from Kaggle and place `DataCoSupplyChainDataset.csv` in the project folder.
2. Run the Python script.
3. Open the newly generated `Supply_Chain_Report_Basic.xlsx` to view the aggregated business insights.
