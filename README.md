# cars-data-analysis-python

## Project Overview
This project performs Exploratory Data Analysis (EDA) on a cars dataset using Python and Pandas.

The project focuses on:
- Data cleaning
- Handling missing values
- Filtering data
- Data transformation
- Exploring car features and origins

---

## Technologies Used
- Python
- Pandas

---

## Dataset Information
The dataset contains information about cars such as:
- Make
- Origin
- Cylinders
- Weight
- MPG Highway
- Other vehicle-related attributes

---

## Objectives
- Analyze automobile dataset
- Practice data cleaning techniques
- Handle missing values
- Perform filtering and transformation operations
- Extract meaningful insights from the data

---

## Features Implemented

### 1. Data Exploration
- Display dataset structure
- Check dataset dimensions
- Preview records

```python
data.head()
data.shape
```

---

### 2. Handling Missing Values
Missing values in the `Cylinders` column were replaced using the mean value.

```python
data['Cylinders'].fillna(data['Cylinders'].mean(), inplace=True)
```

---

### 3. Value Counts Analysis
Analyzed different car manufacturers available in the dataset.

```python
data['Make'].value_counts()
```

---

### 4. Data Filtering
Filtered cars based on their origin.

```python
data[data['Origin'] == 'Asia']
```

Filtered multiple origins using `isin()`.

```python
data[data['Origin'].isin(['Asia', 'Europe'])]
```

---

### 5. Removing Unwanted Records
Removed cars with weight greater than 4000.

```python
data[~(data['Weight'] > 4000)]
```

---

### 6. Data Transformation
Increased all values of the `MPG_Highway` column by 3.

```python
data['MPG_Highway'] = data['MPG_Highway'].apply(lambda x: x + 3)
```

---

## Key Learning Outcomes
Through this project, I learned:
- Data cleaning using Pandas
- Handling null values
- Filtering datasets
- Data transformation techniques
- Basic exploratory data analysis

---

## Future Improvements
- Add data visualizations using Matplotlib and Seaborn
- Perform correlation analysis
- Build interactive dashboard
- Add statistical insights and charts

---


## Requirements

Install dependencies using:

```bash
pip install pandas
```

---

## How to Run

```bash
python cars_analysis.py
```

---

## Conclusion
This project demonstrates the use of Python and Pandas for performing exploratory data analysis on automobile datasets. The analysis includes data cleaning, filtering, transformation, and handling missing values to better understand the dataset.

---

## Author
Your Name
