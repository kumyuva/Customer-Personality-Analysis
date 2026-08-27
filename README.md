# Customer Personality Analysis: Data Cleaning & Preprocessing

*Last Updated: August 27, 2026*

## 📌 Project Overview
This repository contains **Task 1** of a Data Analytics Internship simulation. The primary objective is to clean and prepare a raw dataset for exploratory data analysis (EDA) and machine learning modeling. 

Real-world data is often messy. This project demonstrates practical data wrangling skills, including handling missing values, standardizing formats, and ensuring data integrity using **Python** and **Pandas**.

## 🛠️ Tools & Technologies Used
*   **Python 3.x**
*   **Pandas** (Data manipulation and cleaning)
*   **Jupyter Notebook / Google Colab** 

## 📂 Repository Structure
*   `marketing_campaign.csv` - The original, uncleaned dataset containing 2,240 rows and 29 columns.
*   `customer_personality_cleaned.csv` - The final, processed dataset ready for analysis.
*   `task1_data_cleaning.ipynb` - The Python notebook containing the step-by-step cleaning pipeline.

## 🧹 Key Data Cleaning Steps Performed

1.  **Column Header Standardization:**
    *   Converted all column names to lowercase and replaced spaces/special characters with underscores (e.g., `Year_Birth` -> `year_birth`).
2.  **Missing Value Imputation:**
    *   Identified 24 missing values in the `income` column. 
    *   Imputed these missing values using the **median income (51381.5)** rather than the mean. This preserved the dataset's size (2,240 rows) without introducing outlier bias.
3.  **Date Formatting:**
    *   Converted the `dt_customer` (date of customer enrollment) column from an inconsistent string format (`DD-MM-YYYY`) into a standardized `datetime` format (`YYYY-MM-DD`).
4.  **Data Integrity Checks:**
    *   Verified the dataset for duplicate rows (0 found).
    *   Confirmed all numerical and categorical data types were properly assigned.

## 🚀 How to Run the Code
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/kumyuva/Customer-Personality-Analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Customer-Personality-Analysis
   ```
3. Ensure you have pandas installed:
   ```bash
   pip install pandas
   ```
4. Run the Jupyter Notebook or Python script to view the data transformation process.
