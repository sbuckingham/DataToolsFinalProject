# DataToolsFinalProject
Repository for our COMP 4447 Data Tools Final Project

Health Insurance Claims Denials Analysis

This repository contains code for analyzing health insurance claims denials across different states, insurers, and years using data from the Kaiser Family Foundation (KFF) Transparency Data Working Files (2015-2023). The project focuses on understanding trends in claim applications and denials, preparing the data for analysis, and visualizing key insights.

Project Structure:

/repo-root  
│── data/                           # Folder for raw datasets, in repo broken out to see all 2015-2023 datasets and Topline Survey for contextual information (2015-KFF-Transparency-Data-Working-File.xlsx, 2016-KFF-Transparency-Data-Working-File.xlsx, ..., 2023-KFF-Transparency-Data-Working-File.xlsx; Topline-Survey-of-Consumer-Experiences-with-Health-Insurance.pdf)
│── notebooks/                       # Jupyter notebooks for data processing & analysis    
│   ├── FINAL_NAME_OF_CODE_NOTEBOOK.ipynb      # Data ingestion and preprocessing; exploratory data analysis (EDA) & visualizations  
│── requirements.txt                  # Required dependencies  
│── README.md                         # Project documentation  

Dataset:

The dataset consists of health insurance claims data across multiple years (2015-2023). Each year's data is stored in an Excel file with multiple sheets corresponding to different plan types.

Key Data Considerations:
- Medical Plans & Excluded Medical Plans: These sheets are our focus.
- Dental-only Issuers: These sheets are ignored.
- Metadata Handling: Some years include extra metadata rows before the actual data.
- Column Variability: Features may differ across years, requiring careful alignment.

Setup & Installation:

1. Clone this repository:
   git clone https://github.com/sbuckingham/DataToolsFinalProject.git

2. Create a virtual environment:
   python -m venv venv
   source venv/bin/activate   # On Mac/Linux
   venv\Scripts\activate      # On Windows

3. Install required dependencies:
   pip install -r requirements.txt

Usage:   Run the data preprocessing Jupyter notebook:
   jupyter notebook notebooks/FINAL_NAME_OF_CODE_NOTEBOOK.ipynb


Dependencies:
- Python 3.8+
- pandas
- numpy
- openpyxl
- seaborn
- matplotlib
- Jupyter Notebook


