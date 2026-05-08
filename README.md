# 🧹 Data Cleaning Project using Python

## 📌 Project Overview
This project focuses on cleaning and preprocessing raw data using Python and Pandas.  
The dataset contained missing values, duplicate records, inconsistent formatting, and unnecessary columns which were cleaned and transformed into a structured format ready for analysis.

Data cleaning is an essential step in Data Analytics because accurate insights depend on high-quality data.

---

## 🚀 Objectives
- Improve data quality
- Handle missing values
- Remove duplicate records
- Standardize data formatting
- Prepare dataset for analysis and visualization

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Jupyter Notebook
- Excel / CSV Files

---

## 📂 Project Structure

```bash
Data-Cleaning-Project-1/
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

## 🔍 Data Cleaning Steps Performed

### 1️⃣ Importing Dataset

```python
import pandas as pd

df = pd.read_csv("dataset.csv")
```

---

### 2️⃣ Checking Missing Values

```python
df.isnull().sum()
```

Handled missing values using:
- `dropna()`
- `fillna()`

---

### 3️⃣ Removing Duplicate Records

```python
df.drop_duplicates(inplace=True)
```

---

### 4️⃣ Standardizing Text Data

```python
df["Name"] = df["Name"].str.title()
```

---

### 5️⃣ Cleaning Phone Numbers & Emails

- Removed unwanted characters
- Standardized formatting

---

### 6️⃣ Converting Data Types

```python
df["Date"] = pd.to_datetime(df["Date"])
```

---

### 7️⃣ Removing Unnecessary Columns

```python
df.drop(columns=["Not_Useful_Column"], inplace=True)
```

---

### 8️⃣ Exporting Cleaned Dataset

```python
df.to_csv("cleaned_dataset.csv", index=False)
```

---

## 📊 Project Outcome
After cleaning:
- Dataset became more accurate
- Duplicate and null values were removed
- Data formatting became consistent
- Dataset became analysis-ready

---

## 💡 Skills Demonstrated
- Data Cleaning
- Data Preprocessing
- Data Transformation
- Pandas Operations
- Handling Missing Values
- Data Quality Improvement

---

## ▶️ How to Run This Project

### Step 1: Clone Repository

```bash
git clone https://github.com/Yashas1107/Data-Cleaning-Project-1.git
```

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 3: Open Jupyter Notebook

```bash
jupyter notebook
```

---

## 📷 Screenshots


Example:

```markdown
![Raw Data](screenshots/raw_data.png)
![Cleaned Data](screenshots/cleaned_data.png)
```

---

## 📈 Future Improvements
- Add data visualization
- Automate preprocessing pipeline
- Perform exploratory data analysis (EDA)
- Create dashboard using Power BI

---

## 🤝 Contributing
Contributions are welcome!  
Feel free to fork this repository and improve the project.

---

## ⭐ Support
If you found this project useful, give it a ⭐ on GitHub!

---

## 📜 License
This project is licensed under the MIT License.
