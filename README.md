# Social-Media ETL with Apache Pig

A structured Apache Pig ETL project for handling big data from social-media with supplementary Jupyter notebook-scripts for timestamp calculation. Demonstrates end-to-end big-data ingestion, transformation, and analysis workflows. 

## Contents
`pig/`  
- Modular Pig Latin scripts (`Task_A` → `Task_H`) that load CSVs, filter and aggregate user/page data, join datasets, and output results. Added them here as .txt files.
     
`utils/`  
- `compute_timestamp.ipynb` - Generates “90-days-ago” timestamp along with the latest one, stored in `ninety_days_ago_timestamp.txt`.   
- `dataset_creation.ipynb` - Creates our synthetic data for our analysis as described in the `data/data_overview.md`.   
     
`data/`
- Subsets of the actual data, added the CSVs (`subset_FaceInPage.csv`, `subset_Associates.csv`, `subset_AccessLogs.csv`). Described each one of them in detail in the `data/data_overview.md`.

`output/`
- Outputs of Pig Latin scripts from (`Task_A` → `Task_H`).

## Tasks Summary

| Task | Focus |
|------|-------|
| A | Filter users by nationality |
| B | Find top 10 most visited pages |
| C | Count users by country code |
| D | Match owners with relationship counts |
| E | Calculate total and distinct page accesses per user |
| F | Identify users who haven’t visited their friend’s page |
| G | Detect inactive users based on access timestamps |
| H | Determine whether an owner is 'More Popular' based on relationships |
