# Real-world Data Wrangling

Project notebook: `Data_Wrangling_Project_Starter.ipynb`

## What’s inside
- Kaggle security telemetry (40k rows) gathered programmatically via Kaggle REST; saved raw at `data/raw/kaggle_cyber_security_attacks*`.
- MITRE ATT&CK Enterprise techniques scraped with BeautifulSoup; saved raw at `data/raw/mitre_enterprise_techniques_raw.csv`.
- Cleaning, assessment, merging, visuals, and bonus graph/GraphQL live in the notebook.
- Clean outputs: `data/processed/cleaned_cyber_attacks_with_mitre.csv`, `mitre_enterprise_clean.csv`.
- Optional graph export: `data/processed/cyber_attack_graph.graphml`.

## Running
1. Open `Data_Wrangling_Project_Starter.ipynb` in Jupyter.
2. Run all cells; dependencies are installed in the first cell (includes pandas, seaborn, networkx, graphql-core, bs4, requests).
3. Plots and GraphQL query outputs render in the final section; nbconvert execution was validated locally.

## Rubric checklist (quick pass)
- Problem statement filled; two related datasets via two methods (Kaggle download + HTML scraping) with >500 rows each.
- Two quality + two tidiness issues identified, justified, cleaned, and validated.
- Unnecessary fields removed; datasets combined; final dataset has >4 variables.
- Raw vs cleaned stored with clear filenames.
- Research question answered with two visuals and interpretations.
- Reflection completed; all “FILL IN” placeholders resolved.

## Key files
- Notebook: `Data_Wrangling_Project_Starter.ipynb`
- Raw data: `data/raw/`
- Cleaned data: `data/processed/`
