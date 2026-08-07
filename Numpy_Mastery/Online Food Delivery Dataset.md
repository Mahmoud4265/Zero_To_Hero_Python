# 🍽️ Restaurant Tips & Sales Analysis (EDA)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Visualization-3776AB.svg?style=for-the-badge&logo=python&logoColor=white)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Plotting-11557c.svg?style=for-the-badge)](https://matplotlib.org/)

> 📌 **Author:** Mahmoud  
> 🎯 **Project Scope:** An Exploratory Data Analysis (EDA) pipeline examining customer tipping habits, party sizes, and total bill distributions across different demographics and meal times using the classic `tips` dataset.

---

## 📖 Overview

This project delves into restaurant transaction records to extract key behavioral insights. By examining relationships between customer demographics (gender, smoking status), order timing (day, meal type), and financial outcomes (bill amount, tip value), we reveal core spending patterns and dining trends.

---

## 🛠️ Data Cleaning & Pipeline Steps

1. **Initial Assessment & Structure Check:** Checked missing values (`0 nulls found`) and identified `1 duplicated entry` which was handled using `.drop_duplicates()`.
2. **Feature Categorization:** Inspected unique categories across `day`, `time`, and `smoker` columns.
3. **Statistical Aggregations:** Computed central tendencies (`mean`, `min`, `max`) and grouped total bills across different dimensions.
4. **Data Visualization:** Built informative Bar Charts and Scatter Plots to visualize spending behavior based on party sizes and days of the week.

---

## 📊 Key Insights & Summary Statistics

### 💡 General Spending Metrics
* **Average Total Bill:** `$19.79`
* **Highest Single Bill:** `$50.81`
* **Lowest Single Bill:** `$3.07`

---

### 📈 Group Aggregations (`groupby`)

| Group Dimension | Category | Avg. Total Bill ($) | Insight |
| :--- | :--- | :---: | :--- |
| **Day of Week** | Sun <br> Sat <br> Thur <br> Fri | **21.41** <br> **20.44** <br> 17.68 <br> 17.15 | Weekends (Sun/Sat) generate significantly higher average bill amounts compared to weekdays. |
| **Party Size** | 1 → 6 People | **7.24 → 34.83** | Strong positive linear trend: Larger groups consistently result in larger bills. |
| **Smoker Status** | Yes <br> No | **20.76** <br> 19.19 | Smoking tables spend slightly more on average than non-smoking tables. |
| **Gender** | Male <br> Female | **20.74** <br> 18.06 | Male customers pay higher average total bills in this dataset. |

---

## 🎨 Visualizations Highlight

The analysis includes two complementary visualizations:

1. **Average Total Bill by Day (Bar Plot):** Highlights the revenue peak during Sunday and Saturday dinners.
2. **Party Size vs. Total Bill (Scatter Plot grouped by Sex):** Demonstrates how individual and group dynamics scale with spending across male and female payers.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/Mahmoud4265/Zero_To_Hero_Python.git](https://github.com/Mahmoud4265/Zero_To_Hero_Python.git)
   cd Zero_To_Hero_Python/Pandas_Mastery
Run the script / Jupyter Notebook:

Bash
jupyter notebook Online Food Delivery Dataset.ipynb