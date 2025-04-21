## 🧹 **Data Cleaning & Preprocessing: Customer Personality Analysis**
## 📁 **Dataset Source** - Kaggle dataset(https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis/data)
## **Platform Used**: Google Sheets
## *Problem Statement*

Customer Personality Analysis is a detailed analysis of a company’s ideal customers. It helps a business to better understand its customers and makes it easier for them to modify products according to the specific needs, behaviors and concerns of different types of customers.

Customer personality analysis helps a business to modify its product based on its target customers from different types of customer segments. For example, instead of spending money to market a new product to every customer in the company’s database, a company can analyze which customer segment is most likely to buy the product and then market the product only on that particular segment.
## 📌 Objectives

The main goal of this project was to **clean and preprocess** the raw dataset to prepare it for further analysis and modeling. Specific objectives included:

- Handling missing values
- Standardizing inconsistent data formats
- Formatting date columns
- Creating new columns for analysis
- Ensuring all entries were analysis-ready
## 🔧 Cleaning & Preprocessing Steps

### 1. 🗓️ Formatting `Dt_Customer`
- **Original Problem**: The `Dt_Customer` column had dates in inconsistent formats (`MM/DD/YYYY`, `YYYY-MM-DD`, `DD-MM-YYYY`, etc.).
- **Solution**:
  - A new column `Formated Dt_Customer` was created using formulas to **standardize all entries to `DD-MM-YYYY`**.
  - Used string functions in Google Sheets: `SPLIT`, `JOIN`, `TEXT`, `IF`, and `ARRAYFORMULA`.

### 2. ❓ Handling Missing Values
- Checked for null/empty values across all columns.
- Ensured the `Dt_Customer` and other key fields were populated.
- Blank values were flagged for further cleaning or imputation.

### 3. ✂️ Data Trimming and Consistency
- Removed trailing/leading spaces.
- Standardized text capitalization where needed (e.g., for categorical fields).
- Ensured numerical columns were correctly typed (e.g., `Income`, `Spending`).

### 4. 🆕 Derived Columns
- Created new columns such as:
  - `Year_Joined`: Extracted from `Formated Dt_Customer`
## 🗂️ Files Included

- `Customer Personality Analysis cleaned.csv` *(optional, if you export it)*
## ✍️ Author

**[Jeshwanth Chintalapudi]**  
Data Analyst
