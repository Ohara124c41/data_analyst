# Investigate a Dataset – FBI NICS Background Checks

This repository contains the working files for the Udacity *Investigate a Dataset* project. The current analysis focuses on the FBI’s National Instant Criminal Background Check System (NICS) dataset and the accompanying U.S. Census facts table.

## Project Structure

- `Investigate_a_Dataset.ipynb` – primary notebook with the full analysis, covering introduction, data wrangling, exploratory questions, and conclusions.
- `data/gun_data.csv` – monthly state-level background-check counts (Nov 1998–Sep 2017).
- `data/us_census_data.csv` – 2016 state-level demographic metrics used to create per-capita features.

## Reproducing the Notebook

1. Use Python 3.12.6.
2. Install dependencies if they are not already present:
   ```bash
   pip install numpy pandas seaborn matplotlib nbconvert
   ```
3. Launch the notebook (e.g., `jupyter notebook Investigate_a_Dataset.ipynb`) to explore interactively.
4. To run the full notebook headlessly and confirm it executes without errors:
   ```bash
   python -m nbconvert --to notebook --execute Investigate_a_Dataset.ipynb --output /tmp/Investigate_a_Dataset-output.ipynb
   ```
5. Export an HTML report for submission:
   ```bash
   python -m nbconvert --to html Investigate_a_Dataset.ipynb
   ```

## Key Questions Investigated

1. **Throughput:** How has total NICS workload evolved since 1999, and what compound annual growth rate does that imply?
2. **Load distribution:** Which states produced the highest per-capita loads in 2016, and how do those relate to census demographics (density, income, veteran share, poverty)?
3. **Growth hotspots:** Which states saw the steepest growth between 2010 and 2016, and do they overlap with today’s per-capita heavyweights?

Each question has an accompanying narrative, statistics, and visualizations inside the notebook.

## Notes & Limitations

- NICS counts include permit rechecks and other transaction types, so they should be interpreted as workload rather than direct firearm sales.
- Census data covers only the 50 U.S. states, so District of Columbia and territories are excluded from per-capita comparisons.
- 2017 gun-check data is partial (through September), so year-level comparisons stop at 2016 to keep annual totals consistent.

Feel free to build on this notebook by adding additional census features, policy annotations, or richer statistical modeling.
