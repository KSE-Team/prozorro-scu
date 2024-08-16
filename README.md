
# ProZorro Procurement Data Analysis

## Project Overview

This project focuses on analyzing procurement data from the ProZorro platform. It is structured into two main stages, each implemented in a separate Jupyter notebook.

## Notebooks

### 1. `prozorro_scu_clustering.ipynb`

**Objective:**  
The primary task of this notebook is to process raw procurement data and output it at the SKU (Stock Keeping Unit) level. 
- Dtaset: The project involves analyzing data on office equipment tenders from Prozorro for the years 2023-2024.
- Data: Initially, the dataset contained 518,601 price records, which were cleaned down to 237,260 entries after removing missing values? and ~80,000 - in final.
Objective: The notebook  focused on clustering or other analytical techniques related to this dataset.

**Steps:**
- **Data Loading:** Procurement data is loaded from ProZorro.
- **Data Cleaning:** The raw data is cleaned to remove any inconsistencies or errors.
- **Clustering:** The cleaned data is clustered based on similar goods using k-means metod.
- **Outlier Removal:** Outliers and clusters with fewer than 50 records are removed.
- **Shapiro Test Filtering:** Records where the Shapiro-Wilk test score is less than 95% are filtered out.

**Output:**  
After processing, the dataset contains 80,739 records at the SKU level.

### 2. `analysis.ipynb`

**Objective:**  
This notebook performs a preliminary analysis of the cleaned dataset obtained from the first notebook.

**Steps:**
- **Descriptive Statistics:** The dataset is analyzed to generate summary statistics.
- **Regression Analysis:** Several regression models are run to verify the reliability of the data.

**Output:**  
The analysis provides insights into the data's structure and reliability, setting the stage for more detailed future analyses.

## How to Run the Notebooks

1. Clone the repository:
   ```bash
   git clone https://github.com/KSE-Team/prozorro-scu


