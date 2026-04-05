# 🦠 COVID-19 Data Analysis

A beginner-to-intermediate Python data analysis project exploring global COVID-19 trends using real-world data.

---

## 📌 Overview

This project analyzes COVID-19 cases, deaths, and recoveries using **Pandas** and **Matplotlib/Seaborn**. It is structured as a Jupyter Notebook with step-by-step cells covering data loading, cleaning, visualization, and summary statistics.

---

## 📊 What's Analyzed

| Section | Description |
|---|---|
| Daily Trend | Line chart of global cases, deaths & recoveries over time |
| Top 10 Countries | Horizontal bar chart ranked by total cases |
| Deaths vs Recoveries | Grouped bar chart for the top 10 countries |
| Case Fatality Rate | CFR (%) comparison across top 10 countries |
| Summary Statistics | Global totals and key rates |

---

## 🗂️ Project Structure

```
COVID-19-Data-Analysis/
│
├── covid_analysis.ipynb   # Main Jupyter Notebook
├── covid.csv              # Dataset (from Kaggle)
├── README.md              # Project documentation
│
└── outputs/               # Saved chart images (auto-generated)
    ├── trend_chart.png
    ├── top10_countries.png
    ├── deaths_vs_recoveries.png
    └── cfr_chart.png
```

---

## 🛠️ Tools & Libraries

- **Python 3.10+**
- **Pandas** — data loading, cleaning, grouping
- **Matplotlib** — base plotting and formatting
- **Seaborn** — styled statistical visualizations
- **Jupyter Notebook** — interactive analysis environment

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/your-username/COVID-19-Data-Analysis.git
cd COVID-19-Data-Analysis
```

**2. Install dependencies**
```bash
pip install pandas matplotlib seaborn jupyter
```

**3. Add the dataset**

Download the COVID-19 dataset from [Kaggle](https://www.kaggle.com/) and place `covid.csv` in the root folder.  
Expected columns: `date`, `country`, `cases`, `deaths`, `recoveries`

**4. Launch the notebook**
```bash
jupyter notebook covid_analysis.ipynb
```

---

## 🔍 Key Concepts Practiced

- `pd.read_csv()`, `pd.to_datetime()` — data ingestion
- `.fillna()`, `.drop_duplicates()` — data cleaning
- `.groupby()`, `.sort_values()` — aggregation
- `sns.lineplot()`, `barh()`, `sns.barplot()` — visualizations
- Derived metrics: `active_cases`, `fatality_rate`

---

## 📈 Sample Output

> Charts are saved automatically as `.png` files in the `outputs/` folder after running the notebook.

---

## 📝 Dataset

- Source: [Kaggle COVID-19 Dataset](https://www.kaggle.com/)
- The dataset is **not included** in this repo. Please download and add it manually.

---

## 🙋 About

Built as a learning project to practice **data wrangling and visualization** with Python.  
Feel free to fork it, extend it, or use it as a reference!

---

*Made with Python 🐍 and curiosity 📚*
