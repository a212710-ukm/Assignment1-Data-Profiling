# Assignment1-Data-Profiling
# Heart Disease Data Profiling

**Course:** TTTC3213 Data Engineering  
**Assessment:** Assignment 1 – Data Profiling (EDA) Report  
**Dataset:** Heart Failure Prediction Dataset (Heart Disease)

## Project Overview

This project examines the quality of cardiovascular patient records for a healthcare clinic before the data is used for heart disease risk assessment. It focuses on identifying and addressing missing or invalid values, examining outliers, checking data consistency, and assessing privacy and bias risks.

The main questions are:
- What data quality issues exist in the heart disease dataset?
- How should these issues be handled while preserving useful clinical information?
- What limitations remain before the dataset can be used for further analysis or machine learning?

## Dataset

- **Source:** Kaggle – Heart Failure Prediction Dataset
- **URL:** https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction
- **File:** `heart.csv`
- **Size:** 918 rows and 12 columns
- **Target variable:** `HeartDisease` (0 = no heart disease, 1 = heart disease)

The CSV file was obtained from Kaggle and used for data profiling in a Jupyter notebook.

## Project Files

Keep the following files in the same folder:

- `README.md`
- `TTTC3213_Group_Project.ipynb`
- `heart.csv`

**Important:** The notebook loads data using `pd.read_csv("heart.csv")`, so the dataset must be available in the notebook's working directory.

## Instructions to Run

### Option 1: Google Colab (Recommended)

1. Open https://colab.research.google.com/.
2. Select **File → Upload notebook** and upload `TTTC3213_Group_Project.ipynb`.
3. In the left sidebar, select the **Files** icon and upload `heart.csv` into the current Colab session.
4. Select **Runtime → Run all** to execute the notebook from top to bottom.
5. Review the data quality checks, tables, and diagnostic charts.

**Note:** Colab's temporary files may be removed when the runtime resets. Upload `heart.csv` again if needed.

### Option 2: GitHub Codespaces / Jupyter Notebook

1. Open the repository in GitHub Codespaces or download it to a computer with Python and Jupyter installed.
2. Ensure the notebook and `heart.csv` are in the same working directory.
3. Install the required Python libraries if necessary using `pip install pandas numpy matplotlib seaborn ipykernel`.
4. Open `TTTC3213_Group_Project.ipynb` and select a Python kernel.
5. Select **Run All** to execute the notebook.

## Data Profiling Tasks

1. **Dataset Overview:** Examine the dataset structure, data types, and descriptive statistics.
2. **Missing Values:** Identify invalid zero values in cholesterol and resting blood pressure, apply median imputation, and create missing-value flags.
3. **Outlier Detection:** Use the IQR method and boxplots to identify unusual clinical measurements and justify their handling.
4. **Other Data Quality Issues:** Check duplicate records, incorrect data types, inconsistent categories, and invalid values.
5. **Diagnostic Visualizations:** Generate charts showing invalid zero values, outliers, and demographic distributions.
6. **PII and Bias Risks:** Examine sensitive health information, gender imbalance, and potential sampling bias.
7. **Conclusion:** Evaluate the dataset's suitability and remaining limitations.

This assignment focuses on data profiling and quality assessment, not on training or deploying an ML model.

## Group Members

1. **NUR ATIERAH BINTI MOHD ALI HANAFIAH** (A212621)
2. **NOOR DINAH BINTI MD SAIFUL FADLY** (A212710)
3. **NURIN IMANINA BINTI ZAHARUDDIN** (A212774)
4. **NUR IRDINA SAFIYA BINTI ROSLAN** (A213601)
