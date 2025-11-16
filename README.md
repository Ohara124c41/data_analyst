# Udacity Data Analyst Projects

This repository collects my work across multiple Udacity data analyst projects. Each sub-project is self-contained with its own notebooks, data, and README so you can dive in independently.

## Projects Overview

### 1) Investigate a Dataset (`investigate_dataset`)
- **Goal:** Explore and analyze firearm/census dataset, documenting questions, visualizations, and findings.
- **Artifacts:** `Investigate_a_Dataset.ipynb` (analysis).
- **Notes:** Followed the classic investigative workflow (EDA).

### 2) Cybersecurity Data Wrangling (`cybersecurity_data_wrangling`)
- **Goal:** Gather, assess, clean, and analyze two related datasets (Kaggle Cyber Security Attacks + MITRE ATT&CK). Bonus: export a graph representation.
- **Artifacts:** `Data_Wrangling_Project_Starter.ipynb`, raw/processed data, graph export.
- **Highlights:** Programmatic downloads, data quality/tidiness fixes, MITRE mapping, NetworkX graph export.


### 3) Communicate Nuclear IAEA Data Findings (`communicate_nuclear_IAEA_data`)
- **Goal:** Perform exploratory and explanatory visualizations on nuclear infrastructure and reliance datasets.
- **Datasets:** Kaggle nuclear power plants (locations/reactors) + IAEA nuclear electricity statistics (2022).
- **Artifacts:** `Part_I_exploration.ipynb`, `Part_II_explanatory.ipynb`, HTML exports, README.
- **Highlights:** Question→Visualization→Answer structure, required plot types, merged country-level analysis, matching insights across README and slide-style notebook.

## How to Work with the Repo

1) Clone and enter:
```bash
git clone <repo-url>
cd data_analyst
```

2) Open the relevant project folder and follow its README/notebook instructions. Most notebooks are ready to run with `jupyter` or `nbconvert` (Python 3.11+ recommended).

3) Data: raw/processed data are stored within each project. HTML exports for the communicate_nuclear_IAEA_data project are in `communicate_nuclear_IAEA_data/`.

Feel free to explore any project independently. Issues and enhancements can be tracked per project using normal Git workflows.
