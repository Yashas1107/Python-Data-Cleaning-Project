# 🧹 Data Cleaning Using Python

## 📌 Project Overview
This project demonstrates the complete data cleaning process using Python and Pandas.  
The main objective is to transform raw, inconsistent, and messy data into a clean and structured dataset ready for analysis, visualization, and machine learning.

Data cleaning is one of the most important steps in the data analysis pipeline, and this project covers real-world preprocessing techniques commonly used by Data Analysts and Data Scientists.

---

## 🚀 Features
✔️ Handling missing/null values  
✔️ Removing duplicate records  
✔️ Standardizing column names  
✔️ Fixing inconsistent text formatting  
✔️ Cleaning phone numbers and emails  
✔️ Converting data types  
✔️ Removing unnecessary columns  
✔️ Splitting and merging columns  
✔️ Exporting cleaned datasets  

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Jupyter Notebook  

---

## 📂 Project Structure

```bash
Data-Cleaning-Project/
│
├── data/
│   ├── raw_dataset.csv
│   └── cleaned_dataset.csv
│
├── notebooks/
│   └── data_cleaning.ipynb
│
├── screenshots/
│
├── requirements.txt
│
└── README.md
```

---

## 📊 Data Cleaning Steps Performed

### 1️⃣ Importing Dataset
Loaded raw datasets using Pandas for preprocessing and analysis.

```python
import pandas as pd

df = pd.read_csv("dataset.csv")
```

---

### 2️⃣ Handling Missing Values
Identified and managed null values using different techniques.

```python
df.isnull().sum()
df.dropna(inplace=True)
```

---

### 3️⃣ Removing Duplicates
Duplicate records were detected and removed to improve data quality.

```python
df.drop_duplicates(inplace=True)
```

---

### 4️⃣ Standardizing Text Data
Cleaned inconsistent text formatting.

```python
df["Name"] = df["Name"].str.title()
```

---

### 5️⃣ Fixing Data Types
Converted columns into proper data types.

```python
df["Date"] = pd.to_datetime(df["Date"])
```

---

### 6️⃣ Exporting Clean Data
Saved the cleaned dataset for further analysis.

```python
df.to_csv("cleaned_dataset.csv", index=False)
```

---

## 📈 Project Outcome
After cleaning:
- Data became more accurate and reliable
- Inconsistencies were removed
- Dataset became analysis-ready
- Improved overall data quality

---

## 💡 Skills Gained
- Data preprocessing
- Data quality assessment
- Pandas operations
- Real-world data handling
- Data transformation techniques

---

## ▶️ How to Run the Project

### Step 1: Clone Repository

```bash
git clone https://github.com/your-username/data-cleaning-project.git
```

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 3: Run Jupyter Notebook

```bash
jupyter notebook
```

---

## 📷 Sample Output

---

## 🤝 Contributing
Contributions are welcome!  
Feel free to fork this repository and improve the project.

---

## 📜 License
This project is licensed under the MIT License.

---

## ⭐ Support
If you found this project useful, give it a ⭐ on GitHub!
