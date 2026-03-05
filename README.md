# COVID-19 Global Data Analysis

Exploratory analysis of the COVID-19 pandemic using Kaggle's public dataset — covering case distribution, death and recovery ratios, testing capacity, and country-level comparisons.

---

## Key Results

| Metric | Value |
|---|---|
| Most affected country (total cases) | USA — 5,032,179 |
| Highest deaths | USA — 162,804 |
| Highest cases per million | Qatar — 39,921.58 |
| Highest death-to-confirmed ratio | Vatican City — 9.42% |
| Highest death-to-recovered ratio | UK — 21.31% |
| Highest testing ratio (tests/cases) | Western Sahara — 13,570.2x |
| 100% recovery rate countries | Macao, New Caledonia, Dominica |
| Lowest recovery rate | Spain — 0.61% |
| Month-over-month recoveries growth | +90.00% |
| Month-over-month active cases growth | +42.10% |

---

## Highlights

- **The USA, Brazil, and India dominate absolute numbers**, but this tells only part of the story — Qatar, French Guiana, and Bahrain show the highest cases per million population, meaning their societies faced proportionally far greater exposure than large nations.
- **Spain and the UK have near-zero recovery rates (0.61% and 0.71%)** despite being high-income countries, which points to systematic differences in how recoveries were recorded rather than actual patient outcomes — this warrants caution when comparing recovery rates across countries.
- **The UK's death-to-recovered ratio of 21.31 is the highest globally**, significantly above second-place Caribbean Netherlands (16.14), suggesting either severe healthcare strain or a reporting methodology that undercounts recoveries relative to deaths.
- **Western Sahara ran over 13,500 tests per confirmed case**, the highest testing ratio in the dataset — a stark contrast to countries where testing was scarce and case counts were almost certainly underreported.
- **Global recoveries grew 90% in a single month**, outpacing both active cases (+42%) and deaths (+31%), which signals that the pandemic curve was bending toward resolution at the time this dataset was captured.
- **Brazil's active case burden remained high relative to its recovery count**, indicating that at this snapshot in time, the outbreak was still accelerating — context that raw total-case rankings alone do not convey.

---

## Notebook Structure

| Section | Description |
|---|---|
| Data Loading | Imports six CSV files from the Kaggle dataset; initial shape and type inspection |
| Data Cleaning | Null value treatment using median imputation; duplicate checks; datetime conversion |
| Q1 — Top Countries by Volume | Bar charts for top 10 countries by cases, deaths, recoveries, and active cases |
| Q2 — Trends Over Time | Line plots tracking global confirmed, deaths, recoveries, and active cases by date |
| Q3 — Cases per Million | Proportional ranking table with gradient styling for cross-country comparison |
| Q4 — Deaths / Recoveries / Active | Side-by-side bar charts for the three metrics across top-10 countries |
| Q5 — Death-to-Confirmed Ratio | Ranked analysis of mortality weight relative to total case load |
| Q6 — Death-to-Recovered Ratio | Identifies countries where deaths are disproportionate to recoveries |
| Q7 — Tests-to-Confirmed Ratio | Measures testing capacity and potential case underreporting by country |
| Q8 — Serious-to-Deaths Ratio | Compares critical cases against fatalities as a proxy for ICU outcomes |
| Q9 — Recovery Rate Variation | Top and bottom recovery rates; highlights reporting inconsistencies |
| Brazil Deep-Dive | Country-level bar chart for Brazil across all four core metrics |

---

## Stack

pandas · numpy · matplotlib · seaborn

---

## How to Run

1. Open [the dataset on Kaggle](https://www.kaggle.com/datasets/imdevskp/corona-virus-report) and click **Copy & Edit** to fork the notebook.
2. Attach the dataset to your notebook session — it will be available at `/kaggle/input/corona-virus-report/`.
3. Confirm all six CSV files are present: `country_wise_latest.csv`, `covid_19_clean_complete.csv`, `day_wise.csv`, `full_grouped.csv`, `usa_county_wise.csv`, `worldometer_data.csv`.
4. Run all cells in order (**Run All**).

---

## Data Source

[Corona Virus Report — Kaggle](https://www.kaggle.com/datasets/imdevskp/corona-virus-report)
