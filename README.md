# AI & ML Internship - Task 2  
## Data Cleaning & Missing Value Handling

### 📌 Objective
To perform data cleaning and handle missing values using Python (Pandas, NumPy) and validate the dataset after preprocessing.

---

## 📂 Dataset Used
**Medical Appointment No Shows Dataset**

Dataset Shape (Before Cleaning): **(110527, 14)**

---

## 🛠 Tools Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  

---

## ✅ Steps Performed

### 1️⃣ Load Dataset
- Loaded the dataset using `pd.read_csv()`
- Verified dataset shape and previewed first few rows

### 2️⃣ Identify Missing Values
- Checked missing values using:
  - `df.isnull().sum()`
  - Missing percentage for each column

### 3️⃣ Visualize Missing Values
- Created a bar chart to visualize missing value count per column
- Since the dataset contains **0 missing values**, the plot was empty

### 4️⃣ Handle Missing Values
- Numerical columns: Median Imputation (`fillna(median)`)
- Categorical columns: Mode Imputation (`fillna(mode)`)

✅ No missing values were found, so no values needed to be filled.

### 5️⃣ Drop High Missing Columns
- Dropped columns having more than **50% missing values**
- Result: No columns were dropped

### 6️⃣ Validate Dataset After Cleaning
- Verified final missing values count = **0**

---

## 📊 Results

### Before Cleaning
- Rows: **110527**
- Columns: **14**
- Total Missing Values: **0**

### After Cleaning
- Rows: **110527**
- Columns: **14**
- Total Missing Values: **0**

---

## 📁 Output Files
- `cleaned_dataset.csv` → Final cleaned dataset  
- `Task2_DataCleaning.ipynb` → Notebook containing all steps  

---

## ✅ Conclusion
The dataset was already clean with **no missing values**.  
All required checks, validation, and cleaning steps were performed successfully, and the cleaned dataset was saved for further ML modeling.
