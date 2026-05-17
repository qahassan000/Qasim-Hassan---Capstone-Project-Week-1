# Qasim-Hassan---Capstone-Project-Week-1
Week 1 — AI & Data Science Salaries Analysis
A complete HR analytics project analyzing global AI/Data Science compensation data (2020–2024) for a fast-growing AI startup preparing to scale its data team. The project covers data engineering, exploratory data analysis, statistical testing, predictive modeling, and an interactive Power BI dashboard.

Repository Contents
FileDescriptionWeek1_Qasim.ipynbMain Jupyter notebook (Parts A–E)cleaned_salaries.csvCleaned, deduplicated dataset exported for Power BIWeek1_Dashboard.pbixPower BI interactive dashboardDashboard_Screenshots.pdf2–3 screenshots of the final dashboardREADME.mdThis file

Reproduction Steps
Requirements

Python 3.9+
Jupyter Notebook or Google Colab
The following Python packages:

pip install pandas numpy matplotlib seaborn scipy scikit-learn
Data
Place the two raw source files in the same directory as the notebook before running:

ds_salaries.csv
global_tech_salary.csv

Running the Notebook

Clone or download this repository.
Place both raw data files in the project root directory.
Open Week1_AI_DS_Salaries_Analysis.ipynb in Jupyter or Colab.
Run all cells top to bottom (Kernel → Restart & Run All).

All cells execute without errors. The final cell exports cleaned_salaries.csv to the working directory.
Power BI Dashboard

Open Week1_Dashboard.pbix in Power BI Desktop (free download at powerbi.microsoft.com).
If prompted to refresh the data source, point it to the cleaned_salaries.csv file in this repository.
All slicers and visuals are interactive — no further configuration required.


Key Findings

Experience level is the strongest salary driver — Senior professionals earn ~88% more than Entry-level ($153K vs $77K median); differences confirmed by one-way ANOVA (p < 0.001).
Medium-sized companies pay a premium — Median salary at Medium companies ($140K) exceeds both Large ($110K) and Small ($70K), reflecting the concentration of well-funded AI scale-ups.
Salaries grew 99% from 2020–2023, then plateaued — Median salary rose from $72K to $143K before a slight contraction in 2024, suggesting post-boom market cooling.

Model Performance
Best model: Gradient Boosting Regressor
Test R² = 0.411 | MAE = $39,175 | 5-fold CV R² = 0.371 ± 0.074
