# 🐼 100 Pandas Puzzles - My Solutions & Deep Dive

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Status](https://img.shields.io/badge/Status-Completed%20(60/60)-success)](#)

> **"Solving the famous 100 Pandas Puzzles challenge to master vectorization, data manipulation, time-series, and visualization."**

---

## 📌 About The Repository

This repository contains my personal solutions and optimization notes for the community-favorite **100 Pandas Puzzles** (created by [ajcr](https://github.com/ajcr/100-pandas-puzzles)). 

*(Fun Fact: Despite the name, the challenge actually consists of **60 core puzzles** covering the most critical 80% of Pandas functionalities!)*

---

## 🚀 Covered Topics & Roadmap

- [x] **01-10: Fundamental DataFrame Operations** (Creation, Indexing, Selection)
- [x] **11-17: Filtering & Data Cleaning** (Slicing, Conditional Logic, Null Handling)
- [x] **18-24: Aggregations & GroupBy** (Summary Statistics, Pivot Tables)
- [x] **25-34: String & Text Processing** (Regex, Cleaning Strings)
- [x] **35-40: Advanced MultiIndexing** (Slicing MultiIndex DataFrames)
- [x] **41-50: Reshaping & Custom Logic** (Melting, Pivoting, Custom Functions)
- [x] **51-55: Matrix Operations & Game Logic** (Minesweeper Board & 2D Convolutions)
- [x] **56-60: Plotting & Time Series** (Log Scale, Scatter, OHLC Candlesticks & Rolling Averages)

---

## 💡 Key Takeaways & Advanced Techniques

Here are a few high-value Pandas tricks applied throughout this repository:

1. **Avoid Loops at All Costs:** Leveraging **Vectorization** and `NumPy` broadcasting (e.g., in Matrix/Minesweeper puzzles) dramatically speeds up execution.
2. **Time Series Handling:** Efficiently aggregating financial data with `.resample('1h').ohlc()` for candlestick chart plotting.
3. **Optimized Grouping:** Using `.transform()` to perform group-level imputations and operations without breaking DataFrame shape.
4. **MultiIndex Slicing:** Navigating hierarchical DataFrames using `IndexSlice`.

---

## 🛠️ How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/100-pandas-puzzles-solutions.git](https://github.com/YOUR_USERNAME/100-pandas-puzzles-solutions.git)
   cd 100-pandas-puzzles-solutions


1.Create and activate a virtual environment:
Bash:
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

2.Install dependencies:

Bash:
pip install pandas numpy matplotlib scipy notebook

3.Launch Jupyter Notebook:

Bash: 
jupyter notebook

🤝 Acknowledgments
Puzzles repository by ajcr/100-pandas-puzzles.

Inspired by the original 100 NumPy Exercises.

⭐ If you find these solutions helpful, feel free to give this repo a star!