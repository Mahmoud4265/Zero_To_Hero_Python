# 🍕 Food Delivery Analytics Pipeline

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Vectorized%20Ops-013243.svg?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg?style=for-the-badge)]()

> 📌 **Author:** Mahmoud  
> 🎯 **Project Scope:** End-to-end mini data cleaning, processing, and filtering pipeline for restaurant delivery sales using NumPy and Pandas.

---

## 📖 Overview

The **Food Delivery Analytics Pipeline** is a hands-on data manipulation project designed to process raw restaurant sales data. It demonstrates the seamless integration between **Pandas DataFrames** and **NumPy N-dimensional arrays** to execute high-performance vectorized operations, price adjustments, and dynamic filtering.

---

## 🛠️ Pipeline Architecture & Key Tasks

```
  Raw Delivery Dataset (Pandas DataFrame)
                 │
                 ├──► 1. Rating Analytics (NumPy Vectorized Mean)
                 │
                 ├──► 2. Price Optimization (Argmin Index Search & In-Place Update)
                 │
                 └──► 3. Budget Filtering (Boolean Masking < 150 EGP)
```

### 1️⃣ **Rating Analytics**
* Extracted the `Rating` column as a 1D NumPy array for fast computation.
* Computed the overall **Average Food Rating**: `4.11 / 5.00`.

### 2️⃣ **Price Modification & Anomaly Adjustment**
* Located the index of the cheapest meal in the dataset using NumPy's `argmin()` function.
* Dynamically modified the record in-place within the DataFrame (`df.loc[...]`), setting its price to `0 EGP` for promotional tracking.

### 3️⃣ **Budget-Friendly Meal Extraction**
* Applied boolean indexing to filter out meals priced below **150 EGP**.
* Generated a filtered subset showing high-value, affordable options.

---

## 📊 Dataset Structure & Output Highlights

### 📋 Full Modified Dataset

| OrderID | Item | Price (EGP) | Rating |
| :---: | :--- | :---: | :---: |
| 101 | Burger Combo | 150 | 4.5 |
| 102 | Pizza Large | 280 | 3.8 |
| 103 | Pasta Alfredo | 190 | 4.2 |
| 104 | Shawarma Wrap | **0** *(Cheapest Updated)* | 4.7 |
| 105 | Sushi Set | 450 | 4.9 |
| 106 | Burger Combo | 150 | 4.0 |
| 107 | Pizza Large | 280 | 4.6 |
| 108 | Salad Bowl | 120 | 3.5 |
| 109 | Shawarma Wrap | 90 | 4.8 |
| 110 | Sushi Set | 450 | 2.1 |

---

### 📌 Filtered Results: Budget-Friendly Meals (< 150 EGP)

| OrderID | Item | Price (EGP) | Rating |
| :---: | :--- | :---: | :---: |
| 104 | Shawarma Wrap | 0 | 4.7 |
| 108 | Salad Bowl | 120 | 3.5 |
| 109 | Shawarma Wrap | 90 | 4.8 |

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Mahmoud4265/Zero_To_Hero_Python.git
   cd Zero_To_Hero_Python/Numpy_Mastery
   ```

2. Run the script / open the notebook:
   ```bash
   python food_delivery_analytics.py
   ```
   *or open in Jupyter Notebook:*
   ```bash
   jupyter notebook food_delivery_analytics.ipynb
   ```

---

<div align="center">

⭐ **Part of the Zero_To_Hero_Python Mastery Series** ⭐

</div>
