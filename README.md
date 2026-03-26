# 🦠 COVID-19 Data Analysis Project

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Pandas](https://img.shields.io/badge/Data-Pandas%20%7C%20Numpy-green)
![DataViz](https://img.shields.io/badge/DataViz-Seaborn%20%7C%20Plotly-purple)

## 📌 Project Overview
This project presents a **Professional End-to-End Exploratory Data Analysis (EDA)** of the COVID-19 pandemic using data from 210 countries. The project walks through everything from raw data cleaning and statistical modeling, to advanced interactive visualizations using Plotly.

---

## 📂 Repository Structure

The project strictly follows a professional Data Science structure:

```text
covid19-data-analysis-project/
│
├── data/
│   ├── raw/                      ← Original covid.csv dataset
│   └── processed/                ← Cleaned dataset output by Notebook 1
│
├── notebooks/                    ← Step-by-step Jupyter Notebooks
│   ├── 01_data_loading_and_cleaning.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_visualizations.ipynb
│   ├── 04_interactive_dashboard.ipynb
│   └── 05_final_report.ipynb
│
├── outputs/
│   └── figures/                  ← Automatically generated charts (.png)
│
├── README.md
├── .gitignore
└── requirements.txt
```

---

## 🏃 Setup & Installation
This project was built using Anaconda. You can easily replicate the environment locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/covid19-data-analysis-project.git
   cd covid19-data-analysis-project
   ```

2. *(Optional)* Create a virtual environment and install requirements:
   ```bash
   pip install -r requirements.txt
   ```
   *Note: If you use Anaconda, all primary packages (pandas, seaborn, plotly) are already included.*

3. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. **Important**: Run the notebooks in sequential order starting from `notebooks/01_data_loading_and_cleaning.ipynb` because each notebook relies on data or images generated from the prior ones.

---

## 🛠️ The Notebooks Explained

| Notebook | Purpose | Key Tools |
|----------|---------|-----------|
| **01** Data Loading & Cleaning | Fix null values, handle types, build `CaseFatalityRate` and `RecoveryRate` features, and export cleaned data. | `pandas`, `numpy` |
| **02** Exploratory Data Analysis | Central tendencies, Outlier checks, Distribution histograms (logarithmic scales), and Correlation Heatmaps. | `seaborn`, `scipy` |
| **03** Advanced Visualizations | Generation of static high-res analytical charts, automatically saving them to the `outputs/figures/` folder. | `matplotlib`, `seaborn` |
| **04** Interactive Dashboard | Dynamic data manipulation, Choropleth World Maps, and Country lookup profiles. | `plotly`, `ipywidgets` |
| **05** Executive Summary | Combines the static generated charts and the dynamic Plotly dashboard into one final cohesive Markdown report. | *Markdown + Dashboard* |

---

## 📈 Key Findings
1. **Testing Correlation:** Extremely strong correlation between total tests and total identified cases.
2. **Skewed Distributions:** The virus impact (cases/deaths) is massively right-skewed; a handful of countries (USA, Brazil, India) drive the global statistical averages.
3. **Fatality Variations:** While the USA holds the highest absolute number of deaths, countries like Mexico and the UK hold significantly higher Case Fatality Rates relative to their population.

---
**Author:** Ahmed Mohamed Abdelhady 

mail: [ahmed.mohamed.abdelhady@gmail.com]

linkedin: https://www.linkedin.com/in/ahmed-mohamed-abdelhady/
