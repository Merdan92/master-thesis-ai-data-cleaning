# AI-based Data Cleaning: Outlier Detection & Inconsistency Repair (Master Thesis)

This repository contains the full implementation, datasets, and experimental results for the Master's Thesis: **"Vergleichende Analyse auf Künstlicher Intelligenz basierender Methoden zur Datenbereinigung"**.

The project evaluates traditional Statistical/ML methods against modern AI approaches (LLM, TabPFN) for cleaning tabular data and detecting outliers.

## 📂 Repository Structure

### 1. Data (`/data`)
* **`rfd_main.csv`**: The original "dirty" dataset (Sourced from Kaggle).
* **`rfd_main_cleaned.csv`**: The reference "clean" dataset provided by the original author.
* **`rfd_main_for_hc.csv`**: Intermediate dataset prepared specifically for HoloClean processing.

### 2. Experiments (`/notebooks`)
The Jupyter Notebooks are organized by Research Question (Forschungsfrage) and processing steps:

#### A. Exploratory Data Analysis (EDA)
* **`Datenprofilierung.ipynb`**: Initial profiling of the dataset structure, missing values, and error distribution.

#### B. Experiment 1: Outlier Detection on Raw Data
* **`Forschungsfrage_1_*.ipynb`**: Implementation of IQR, LOF, Isolation Forest (IF), and TabPFN on the uncleaned dataset.

#### C. Experiment 2: Inconsistency Repair (Cleaning)
* **`Forschungsfrage_2_HoloClean.ipynb`**: Data cleaning using constraints and statistical learning.
* **`rfd_constraints.txt`**: Constraint rules file used as input for HoloClean.
* **`Forschungsfrage_2_LLM.ipynb`**: Semantic cleaning using Large Language Models (Claude Sonnet).

#### D. Experiment 3: Outlier Detection on Cleaned Data
* **`Forschungsfrage_3_*.ipynb`**: Re-evaluation of outlier detection methods after the cleaning process to analyze the impact of data quality improvement.

### 3. Results (`/results`)
* Contains the generated CSV outputs, performance metrics, and log files from the experiments.

---
## ℹ️ Data Source & Attribution
The dataset used in this research is based on a public dataset sourced from **Kaggle**. The "dirty" and "cleaned" versions were used to benchmark the performance of the implemented cleaning pipelines.

---
*Master Thesis Project - 2026*
