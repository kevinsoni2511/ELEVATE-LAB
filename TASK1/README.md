# 🧹 Data Analyst Internship – Task 1  
### 📊 Data Cleaning & Preprocessing – *Medical Appointment No Show Dataset*

---

## 🎯 Objective
The goal of this task is to **clean and preprocess a raw dataset** by identifying and fixing common data quality issues such as missing values, duplicates, inconsistent text, incorrect data types, and unformatted date columns.

This ensures that the dataset is ready for analysis or predictive modeling.

---

## 🧰 Tools Used
- **Language:** Python  
- **Libraries:** Pandas  
- **IDE/Notebook:** Jupyter Notebook / Google Colab  
- **Dataset:** `MEDICAL_APPOINMENT_NO_SHOW.csv`

---

## ⚙️ Steps Performed

### 1️⃣ Import & Load Dataset
- Loaded the raw CSV file using Pandas.  
- Checked initial shape and dataset info.

### 2️⃣ Handle Missing Values
- Identified missing values using `.isnull()`.  
- Dropped records with null entries using `dropna(inplace=True)`.

### 3️⃣ Remove Duplicates
- Checked for duplicate rows using `.duplicated()`.  
- Removed them using `drop_duplicates(inplace=True)`.

### 4️⃣ Standardize Column Names
- Converted all column names to lowercase.  
- Replaced spaces with underscores for consistency.

### 5️⃣ Clean & Standardize Text Values
- Converted text to lowercase and trimmed whitespace.  
- Fixed inconsistent values in:
  - **Gender:** “f/m” → “female/male”  
  - **No-show:** “yes/no” → “no_show/showed_up”

### 6️⃣ Convert Dates to Consistent Format
- Converted date columns (`ScheduledDay`, `AppointmentDay`) to `datetime` objects using `pd.to_datetime()`.

### 7️⃣ Correct Data Types
- Converted `Age` column to integer.  
- Ensured proper datatypes for all numeric and categorical features.

### 8️⃣ Final Verification
- Verified column data types and dataset structure using `.info()`.  
- Ensured clean, standardized, and ready-to-use dataset.

---

## 📊 Summary of Changes
| Step | Action | Status |
|------|---------|--------|
| Missing Values | Removed using `dropna()` | ✅ |
| Duplicates | Removed using `drop_duplicates()` | ✅ |
| Text Standardization | Applied lowercase + cleaned spacing | ✅ |
| Gender Normalization | `f/m → female/male` | ✅ |
| No-show Standardization | `yes/no → no_show/showed_up` | ✅ |
| Date Conversion | Converted to `datetime` | ✅ |
| Data Type Fix | `Age → int` | ✅ |

---

## 💾 Output Files
- `MEDICAL_APPOINMENT_NO_SHOW.csv` → *Raw Dataset*  
- `medical_appointment_cleaned.csv` → *Cleaned Dataset (Final)*  
- `MEDICAL_APPOINMENT_NO_SHOW.ipynb` → *Python Script Implementation*

---

## 🧩 Key Learnings
- Handling missing and duplicate data effectively.
- Text normalization and categorical standardization.
- Date formatting and type conversions in Pandas.
- Importance of data preprocessing before analysis or modeling.

---

## 👩‍💻 Author
**Name:** KEVIN HARSHADBHAI SONI  
**Role:** Data Analyst Intern  
**Task:** 1 – Data Cleaning & Preprocessing  

---


> “Clean data is the foundation of every great analysis.” 🚀
