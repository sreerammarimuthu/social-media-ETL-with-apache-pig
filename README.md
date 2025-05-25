# Social-Media ETL with Apache Pig

A structured Apache Pig ETL project for social-media big data with supplementary Jupyter notebook-scripts for utility tasks (timestamp calculation). Demonstrates end-to-end big-data ingestion, transformation, and analysis workflows. This repository contains:

1. **Pig Queries** (`pig/`):  
   - Modular Pig Latin scripts (`Task_A` → `Task_H`) that load CSVs, filter and aggregate user/page data, join datasets, and output results. Stored them in respective folder as .txt files.
     
2. **Utilities** (`utils/`):  
   - **`compute_timestamp.py`**: Generates “90-days-ago” timestamp along with the current one, stored in `ninety_days_ago_timestamp.txt`.
     
3. **Subsets of Data** (`data/`):  
   - Source CSVs (`subset_FaceInPage.csv`, `subset_Associates.csv`, `subset_AccessLogs.csv`)
  
