# Week 1 — AI & Data Science Salaries Analysis

A complete HR analytics project analyzing global AI/Data Science compensation data (2020–2024) for a fast-growing AI startup preparing to scale its data team. The project covers data engineering, exploratory data analysis, statistical testing, predictive modeling, and an interactive Power BI dashboard.

---

## Repository Contents

| File | Description |
|---|---|
| `Week1_Qasim.ipynb` | Main Jupyter notebook (Parts A–E) |
| `cleaned_salaries.csv` | Cleaned, deduplicated dataset exported for Power BI |
| `Week1_Dashboard.pbix` | Power BI interactive dashboard |
| `Dashboard_Screenshots.pdf` | 2–3 screenshots of the final dashboard |
| `README.md` | This file |

---

## Reproduction Steps

### Requirements

- Python 3.9+
- Jupyter Notebook or Google Colab
- The following Python packages:

```
pip install pandas numpy matplotlib seaborn scipy scikit-learn
```

### Data

Place the two raw source files in the same directory as the notebook before running:

- `ds_salaries.csv`
- `global_tech_salary.csv`

### Running the Notebook

1. Clone or download this repository.
2. Place both raw data files in the project root directory.
3. Open `Week1_Qasim.ipynb` in Jupyter or Colab.
4. Run all cells top to bottom (`Kernel → Restart & Run All`).

All cells execute without errors. The final cell exports `cleaned_salaries.csv` to the working directory.

### Power BI Dashboard

1. Open `Week1_Dashboard.pbix` in **Power BI Desktop**.
2. If prompted to refresh the data source, point it to the `cleaned_salaries.csv` file in this repository.
3. All slicers and visuals are interactive.

---

## Key Findings

1. **Experience level is the strongest salary driver** — Senior professionals earn ~88% more than Entry-level ($153K vs $77K median); differences confirmed by one-way ANOVA (p < 0.001).
2. **Medium-sized companies pay a premium** — Median salary at Medium companies ($140K) exceeds both Large ($110K) and Small ($70K), reflecting the concentration of well-funded AI scale-ups.
3. **Salaries grew 99% from 2020–2023, then plateaued** — Median salary rose from $72K to $143K before a slight contraction in 2024, suggesting post-boom market cooling.

## Model Performance

Best model: **Gradient Boosting Regressor**  
Test R² = 0.411 | MAE = $39,175 | 5-fold CV R² = 0.371 ± 0.074
