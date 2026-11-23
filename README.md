# E-Commerce Retail Sales & Consumer Behavior Analysis

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue?style=for-the-badge)](https://matplotlib.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

> An exploratory data analysis (EDA) of high-volume electronics retail transactions across the US, uncovering revenue seasonality, geographic demand hotspots, peak ordering hours, and cross-sell affinities.

---

## 🎯 Business Problem & Core Questions

Retailers handle thousands of transactional records daily. Unlocking insights from this data empowers inventory planners and marketing teams to optimize catalog positioning and promotional timing.
This analysis answers five core business questions:
1. **What was the best month for sales and total revenue?**
2. **Which US city generated the highest sales volume?**
3. **What time of day should marketing campaigns run to maximize conversions?**
4. **Which products are most frequently ordered together (Market Basket Analysis)?**
5. **What product drove the highest volume, and what underlying factors explain it?**

---

## 💡 Key Business Findings

### 1. Monthly Revenue Seasonality
- **December** generated peak sales, driven by holiday gifting (Christmas and New Year promotions).
- **January** recorded the lowest overall sales due to post-holiday consumer spending fatigue.

### 2. Geographic Performance
- **San Francisco (CA)** emerged as the top revenue-generating city, followed by Los Angeles and New York City.
- Factors: Higher disposable income per capita, tech adoption, and customer density.

### 3. Optimal Advertising Schedule
- Order placement exhibits distinct bi-modal peaks throughout the day:
  - **11:00 AM – 1:00 PM**: Lunch break browsing.
  - **6:00 PM – 8:00 PM**: Post-commute evening relaxation.
- *Recommendation*: Schedule digital advertisements 30–45 minutes prior to these peak windows (10:30 AM and 5:30 PM).

### 4. Product Association & Cross-Selling
- The most common co-purchased bundles:
  - **iPhone + Lightning Charging Cable**
  - **Google Pixel + USB-C Charging Cable**
- *Recommendation*: Implement algorithmic checkout recommendations and bundled discount packaging.

### 5. Best-Selling Volume Drivers
- **AAA Batteries (4-pack)** and **AA Batteries (4-pack)** achieved the highest unit sales due to high replacement frequency across household gadgets and consumer electronics.

---

## 🛠️ Data Pipeline & Techniques

- **Data Wrangling**: Combined multi-month CSV logs into a consolidated master dataframe.
- **Feature Extraction**: Extracted `Month`, `Hour`, `City`, and `State` from unstructured timestamps and address strings.
- **Product Bundling**: Applied `itertools.combinations` and grouped order IDs to detect co-occurring pairs.

---

## 📁 Repository Structure

```text
├── Sales Analysis.ipynb   # Complete data cleaning, exploratory analysis, and visualization
├── requirements.txt       # Python dependencies
├── .gitignore             # Git ignore file
└── README.md              # Project documentation
```

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/HarshKumarGuptagit/ecommerce-sales-trend-analysis.git
cd ecommerce-sales-trend-analysis

# Setup environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook "Sales Analysis.ipynb"
```

---

## 👤 Author

**Harsh Kumar Gupta**
- GitHub: [@HarshKumarGuptagit](https://github.com/HarshKumarGuptagit)
- Email: harshkumargupta49@gmail.com
