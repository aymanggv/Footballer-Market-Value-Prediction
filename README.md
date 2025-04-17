# ⚽ Football Player Market Value Prediction

This interactive web app predicts the **actual market value** of football players using their FIFA stats. Built with **Streamlit** and powered by **machine learning**, this project provides correlation analysis, feature selection, model building, and insights into undervalued and overvalued players.

---

## 🧠 Project Summary

- 🔍 **Data Collection**: Player data was retrieved via **web scraping** from [SoFIFA.com](https://sofifa.com) using Python (`requests`, `BeautifulSoup`) — see [`FootballData.ipynb`](./FootballData.ipynb).
- 🧼 **Data Cleaning & Engineering**: Unnecessary features were dropped, and columns were renamed and processed for modeling.
- 📊 **Exploratory Analysis**: Heatmaps, pairplots, and correlation matrices to analyze features.
- 🤖 **Modeling**: A **Random Forest Regressor** predicts player market value.
- 📈 **Evaluation & Visualization**: Residual analysis, undervalued vs. overvalued charts, and actual vs. predicted comparisons.

---

## 📂 Dataset Overview

- Extracted from SoFIFA (FIFA player ratings)
- 1000s of professional players with stats like:
  - `Overall Rating`, `Potential`, `Wage`, `Release Clause`
  - `Best Overall`, `International Reputation`
  - Physical attributes: `Height`, `Weight`, `Age`
  - Engineered: `Base Stats`, `Total Stats`, etc.

---

## 🧰 Tech Stack

- **Frontend**: Streamlit
- **Scraping**: BeautifulSoup, requests
- **Data Analysis**: Pandas, Seaborn, Matplotlib
- **Machine Learning**: Scikit-Learn (`RandomForestRegressor`)

---

## 📊 Highlights

- Correlation heatmaps for all and selected attributes
- Pairplots to observe relationships
- Top 10 undervalued and overvalued players
- Residual plots and model evaluation
- Actual vs. predicted market value scatter plots

---

## ✅ Model Performance
- R² Score
- Adjusted R²
- RMSE (Root Mean Squared Error)
- Cross-Validation (5-Fold R² Scores)
