# Formula 1 Lap Times – Final Project

Final project for a data visualization / data exploration course.  
Analysis of Formula 1 lap times with static and interactive charts in a Jupyter notebook.

---

## 1. Project Overview

This project:

- loads and cleans a Formula 1 lap-time dataset  
- explores lap time distributions and trends across decades  
- compares circuits and continents  
- compares teams and drivers  
- builds interactive Altair visualizations for open-ended exploration  

Main file: **`Final_Project.ipynb`**

---

## 2. Folder / File Structure

.
├── Final_Project.ipynb      # main notebook: cleaning, analysis, visualizations
├── top5_laps_dataset.csv    # dataset used in the notebook
└── README.md                # this file
```

---

## 3. Installation

### Requirements

- Python 3.8+  
- Jupyter Notebook or JupyterLab  

### Python packages

- `pandas`  
- `numpy`  
- `altair`  

Install with:

```bash
pip install pandas numpy altair
```

---

## 4. How to Run the Notebook

1. Ensure these files are in the same folder:

   - `Final_Project.ipynb`  
   - `top5_laps_dataset.csv`  

2. Open a terminal in that folder and start Jupyter:

   ```bash
   jupyter notebook
   ```

3. In the browser, open **`Final_Project.ipynb`**.  
4. Use **Kernel → Restart & Run All** to execute the full workflow from top to bottom.  

The notebook will:

- load the dataset  
- clean and prepare the data  
- compute summary statistics  
- generate static and interactive Altair charts  

If Altair charts do not render, add this near the top of the notebook:

```python
import altair as alt
alt.renderers.enable("default")
```

---

## 5. Dataset Source

- Public Formula 1 statistics from:  
  https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020?resource=download


---
