# Biological Data Visualization with Seaborn

## Overview
This project uses Seaborn and Matplotlib to explore and visualise patterns in the `bacteria_data` dataset — a collection of 50 *Escherichia coli* isolates with antibiotic fitness scores, phenotypic labels, and isolation metadata. The goal is to practise choosing appropriate plot types, mapping variables to visual properties, and presenting biological data clearly.

## Dataset
- **Source:** HackBio Internship 2025 Project Collection
- **URL:** `https://raw.githubusercontent.com/HackBio-Internship/2025_project_collection/main/bacteria.csv`
- **Shape:** 50 rows × 14 columns
- **Key columns:** `sample_id`, `species`, `Isolation origin`, `Phenotype`, `BSL`, `carb_fit`, `cipro_fit`, `genta_fit`, `kan_fit`, `pip_fit`, `labels`

## Tools & Libraries
- Python 3
- Seaborn 0.13.2
- Matplotlib
- Jupyter Notebook

## Project Structure

| Part | Plot Type | Description |
|------|-----------|-------------|
| Part 1 | Distribution Plots | Histograms and KDE plots showing the frequency and density of fitness scores, grouped by Phenotype |
| Part 2 | Relationship Plots | Scatter plots comparing pairs of antibiotic fitness scores, coloured by Labels, Phenotype, and Isolation origin |
| Part 3 | Categorical Plots | Bar plots, box plots, violin plots, and strip plots of fitness scores grouped by categorical variables |
| Part 4 | Heatmap | Correlation matrix of all antibiotic fitness scores to identify co-resistance patterns |
| Part 5 | Faceted Categorical Plot | Faceted box plots breaking down fitness score distributions by Phenotype condition |
| Part 6 | Pair Plot | Pairwise relationship grid across all numeric features, coloured by Labels |

## Key Visualisations

- **Distribution of Carbapenem Fitness** — histogram showing bimodal distribution across isolates
- **Carbapenem vs Piperacillin Fitness** — scatter plots coloured by Labels, Phenotype, and Isolation origin
- **Gentamicin Fitness by Labels, Split by Phenotype** — faceted box plot revealing condition-specific differences
- **Correlation Heatmap** — `carb_fit` and `pip_fit` show a strong positive correlation (0.91), suggesting potential co-resistance
- **Pairwise Relationship Grid** — full overview of relationships between all numeric columns

## Key Findings
- `carb_fit` and `pip_fit` show a strong positive correlation of **0.91**, indicating co-resistance between carbapenem and piperacillin
- `cipro_fit` shows a highly concentrated distribution near 0, with most isolates having very low ciprofloxacin fitness scores
- Pathogenic strains and Commensal strains display overlapping but distinct fitness distributions across several antibiotics
- Isolation origin (urine, blood, faeces, animal) does not strongly separate fitness scores in scatter plots, suggesting host source alone is not predictive of resistance level

## How to Run
1. Clone this repository
2. Open `Biological_Data_Visualization_with_Seaborn.ipynb` in Jupyter Notebook
3. Run all cells from top to bottom (`Kernel → Restart & Run All`)
4. No local dataset download needed; data loads directly from the GitHub URL in the notebook.
