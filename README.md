# Ivan Rey Pestana — Data Portfolio

**Data Science | Machine Learning | Data Visualization | Operations Analytics**

Hi! I'm Ivan Rey Pestana, a data-focused student with hands-on experience applying Python, statistical modeling, and visualization tools to real-world datasets. This repository collects my individual and collaborative projects spanning machine learning, exploratory data analysis, and operational process improvement.

---

## Projects

| # | Project | Tools | Description |
|---|---------|-------|-------------|
| 1 | [F1 Lap Times Analysis](#1-formula-1-lap-times-analysis) | Python, Altair, pandas | End-to-end EDA of 70 years of F1 data with interactive charts |
| 2 | [Movie Ratings — ML Classification](#2-movie-ratings--ml-classification) | Python, scikit-learn, matplotlib | Logistic Regression & Decision Tree to predict top-rated films |
| 3 | [Car Price Analysis Report](#3-car-price-analysis-report) | Python / statistical analysis | Regression analysis and pricing insights from car market data |
| 4 | [OFX Legends Reslot Analysis](#4-ofx-legends-reslot-analysis) | Operations research | Process optimization and TO-BE workflow design |

---

## 1. Formula 1 Lap Times Analysis

**File:** `Final_Project.ipynb` · **Dataset:** `top5_laps_dataset.csv`

End-to-end data exploration of Formula 1 lap times from 1950–2020. The notebook answers three core questions:

1. How are F1 lap times distributed overall, and how have they changed across decades?
2. How does circuit design (layout, continent, track type) affect lap performance?
3. Which teams and drivers stand out when controlling for car and conditions?

**My contributions** (group project with J. Cart, G. Jaimes, I. Gomez, J. Czemeinski):
- Data cleaning pipeline (outlier removal, millisecond → second conversion, decade binning)
- Correlation heatmap and podium-rate segmentation analysis
- Interactive Altair charts (linked brush scatter, team dropdown selector)
- Written interpretations for all visualization sections

**Key findings:**
- Starting grid position and final race position are positively correlated (r ≈ 0.50)
- Average lap times have decreased steadily since the 1950s, with the sharpest improvement in the 1980s–2000s driven by turbo and aerodynamic advances
- High-speed circuits (Monza, Spa) show lap times 30–50 seconds faster than technical street circuits (Monaco, Singapore)
- Hamilton and Verstappen rank among the fastest average lap times in the modern hybrid era

**Stack:** `pandas` · `altair` · `numpy` · `seaborn` · `matplotlib`

### Run it
```bash
pip install pandas numpy altair seaborn matplotlib
jupyter notebook Final_Project.ipynb
```

---

## 2. Movie Ratings — ML Classification

**File:** `BigDataMoviesCleaned.ipynb` · **Dataset:** `movies.csv` (see source below)

Binary classification task: predict whether a movie will be "top-rated" (IMDb rating ≥ 8.5) using features like genre, year, runtime, budget, and box office gross. Two models are compared head-to-head.

**Models trained:**
- Logistic Regression — 75% accuracy; struggles with the minority class (AUC ≈ 0.51)
- Decision Tree — 73% accuracy; similar class imbalance issues

**Key finding:** Both models are limited by a heavily imbalanced dataset (few top-rated movies). The analysis clearly identifies this as the bottleneck and recommends class balancing (SMOTE or weighted loss) as the next step.

**Dataset source:** [`movies.csv` from Kaggle — IMDB Movies Dataset](https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows)  
Download and place `movies.csv` in the same folder before running.

**Stack:** `pandas` · `numpy` · `scikit-learn` · `matplotlib` · `seaborn`

### Run it
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
# Download movies.csv from the Kaggle link above
jupyter notebook BigDataMoviesCleaned.ipynb
```

---

## 3. Car Price Analysis Report

**File:** `Final_CarPrice_Report.pdf`

Statistical analysis of used car pricing data. The report covers:
- Feature correlation analysis (mileage, age, brand vs. price)
- Regression modelling for price prediction
- Actionable pricing insights for buyers and sellers

*(PDF — view directly on GitHub)*

---

## 4. OFX Legends Reslot Analysis

**File:** `OFX Legends Reslot Analysis TO-BE Report.pdf`

Operational process improvement study. Designed and documented a TO-BE (future-state) workflow for a reslotting operation, including bottleneck identification, capacity analysis, and recommended process changes.

*(PDF — view directly on GitHub)*

---

## Tech Stack Overview

| Area | Tools |
|------|-------|
| Data manipulation | `pandas`, `numpy` |
| Machine learning | `scikit-learn` |
| Visualization | `altair`, `matplotlib`, `seaborn` |
| Notebooks | Jupyter |
| Languages | Python 3.8+ |

---

## Contact

- **GitHub:** [github.com/ReyPestana](https://github.com/ReyPestana)
- **Email:** ivanrey1809@gmail.com
