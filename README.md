# Exploratory Data Analysis — Palmer Penguins 🐧

An end-to-end EDA project exploring physical measurements of 344 penguins from three species (Adelie, Chinstrap, Gentoo) across three islands in Antarctica.

## Dataset
**Palmer Penguins** — collected by Dr. Kristen Gorman and Palmer Station LTER, packaged by Allison Horst.
Source: https://allisonhorst.github.io/palmerpenguins/

| Column | Description |
|---|---|
| species | Adelie, Chinstrap, Gentoo |
| island | Biscoe, Dream, Torgersen |
| bill_length_mm | Bill length (mm) |
| bill_depth_mm | Bill depth (mm) |
| flipper_length_mm | Flipper length (mm) |
| body_mass_g | Body mass (g) |
| gender | Male / Female |

## What I did
1. **Data inspection** — shape, data types, summary statistics
2. **Data cleaning** — dropped 2 empty rows, filled missing gender using species-wise mode, converted categorical columns
3. **Univariate analysis** — count plots, histograms, skewness
4. **Bivariate analysis** — measurements by species, species per island, gender differences
5. **Correlation analysis** — heatmap and pairplot
6. **Outlier detection** — IQR method

## Key findings
- **Gentoo** penguins are the heaviest (~5 kg), have the longest flippers, and live only on Biscoe island.
- **Flipper length and body mass** are strongly correlated (r = 0.87).
- **Males are heavier** than females in all three species.
- **Simpson's Paradox:** bill length vs bill depth is negative overall (r = −0.24) but positive within every species (r = 0.39 to 0.65). Analysing by group reveals the real pattern.
- No outliers were found using the IQR rule.

## Tools
Python · Pandas · NumPy · Matplotlib · Seaborn · Jupyter Notebook

## How to run
1. Download `EDA_Project.ipynb` and `penguins.csv` into the same folder.
2. Open the notebook in Jupyter and run all cells.
