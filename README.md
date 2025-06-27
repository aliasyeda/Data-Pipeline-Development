# Data-Pipeline-Development
*COMPANY* : CODTECH IT SOLUTIONS
*NAME* : SYEDA ALIA SAMIA
*INTERN ID* : CT04DG2786
*DOMAIN* : DATA SCIENCE
*DURATION* : 4 WEEKS
*MENTOR* : NEELA SANTOSH

# 🚢 Titanic Data Pipeline Project

This project demonstrates a complete **ETL (Extract, Transform, Load)** pipeline using the **Titanic dataset** from Kaggle. The goal of this pipeline is to clean and prepare real-world data for further analysis or machine learning applications.

This task was part of a data science internship, where I was assigned to build a preprocessing pipeline that handles missing values, encodes categorical data, scales numerical features, and finally stores the cleaned dataset for future use.


## 📌 Project Overview

The **Titanic dataset** contains information about passengers aboard the Titanic. It includes both numerical and categorical features like age, fare, gender, and embarkation port. However, real-world data is rarely clean. This project focuses on transforming raw Titanic data into a cleaned and structured format, ready for use in machine learning


## ⚙️ Tools and Libraries Used

- **Python** – Core programming language
- **Pandas** – For data manipulation and cleaning
- **Scikit-learn** – For preprocessing tasks like encoding and scaling
- **Jupyter Notebook** – For step-by-step execution and documentation


## 🧩 ETL Pipeline Process

### 🔍 Step 1: Data Extraction
The raw data (`train.csv`) was loaded using the `pandas` library. The dataset contains features such as Passenger ID, Name, Age, Sex, Fare, Embarked, etc.

### 🧼 Step 2: Data Transformation

- **Handling Missing Values**:  
  - Filled missing `Age` values with the column's mean.
  - Filled missing `Embarked` values with the most frequent (mode).
  - Dropped the `Cabin` column due to excessive missing data.

- **Encoding Categorical Data**:  
  - Used `LabelEncoder` to convert `Sex` (male/female) into binary format.
  - Encoded `Embarked` (S, C, Q) into numeric form.

- **Scaling Numerical Features**:  
  - Applied `StandardScaler` to normalize `Age` and `Fare`.

### 💾 Step 3: Data Loading
The cleaned and processed dataset was saved as `processed_titanic_data.csv`. This file can now be used directly for machine learning models or exploratory data analysis.

---

## 📂 Files in This Repository

File Name                        Description                                

train.csv                    :   Original Titanic dataset (from Kaggle)     
titanic_etl_pipeline.ipynb   :   Jupyter Notebook containing all ETL steps 
processed_titanic_data.csv   :   Final cleaned dataset                    
README.md                    :   Project overview and documentation         

---

## ✅ Key Learnings

- How to handle missing values in real datasets
- Converting categorical data into machine-readable format
- Importance of feature scaling before machine learning
- Building and saving a structured data pipeline


## 🙌 Acknowledgements

Dataset provided by [Kaggle Titanic Challenge](https://www.kaggle.com/c/titanic/overview).




