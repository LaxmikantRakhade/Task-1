# Task-1
# 🧼 Data Cleaning and Preprocessing Summary

**Title:** Data Cleaning and Preprocessing  
**Dataset Used:** `Test.csv`  
**Cleaned File:** `Cleaned_Test.csv`  
**Total Rows:** 5,681  
**Total Columns:** 11  

---

## ✅ Steps Performed During Cleaning

### 1. Removed Duplicate Rows
- Used `drop_duplicates()` to eliminate exact duplicate records.

### 2. Renamed Columns for Consistency
- Converted all column headers to lowercase.
- Replaced spaces with underscores for uniform naming.

### 3. Handled Missing Values
- Filled missing numeric values (e.g., `item_weight`) using the mean.
- Filled missing categorical values (e.g., `outlet_size`) using the mode.

### 4. Standardized Categorical Data
- Unified inconsistent values in `item_fat_content`:
  - `'LF'`, `'low fat'` → `'Low Fat'`
  - `'reg'` → `'Regular'`

### 5. Label Encoding
- Applied `LabelEncoder` from `sklearn` on categorical columns like `item_type`, `outlet_type`.

### 6. Normalized Numeric Columns
- Used `MinMaxScaler` to scale numeric data (e.g., `item_mrp`) to a 0–1 range.

---

## 📁 Final Output

- All missing values handled  
- Duplicate entries removed  
- Data standardized and ready for analysis or machine learning  
