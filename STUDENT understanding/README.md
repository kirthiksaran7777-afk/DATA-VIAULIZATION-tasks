# Student Performance Data Understanding, Cleaning & Feature Engineering

##  Project Overview

This project focuses on understanding, cleaning, and transforming student performance data.

The analysis includes cleaning categorical features, calculating statistical measures for student subject scores, creating new performance-related features, and detecting extreme outliers in student performance.

The main goal is to convert raw student data into a clean and structured dataset that can be used for further analysis and machine learning.

---

##  Objectives

The main objectives of this project are:

1. Clean categorical features in the student dataset.
2. Standardize categorical values for consistent analysis.
3. Calculate statistical measures for subject scores.
4. Create total marks and percentage performance features.
5. Detect extreme performance outliers.
6. Understand the overall distribution of student scores.
7. Prepare the dataset for further analysis and modeling.

---

##  Dataset

**Dataset Name:** `StudentsPerformance.csv`

The dataset contains information about students' demographic and educational background along with their subject scores.

### Main Features

* Gender
* Race/Ethnicity
* Parental Level of Education
* Lunch
* Test Preparation Course
* Math Score
* Reading Score
* Writing Score

---

##  Data Cleaning

The following categorical features are cleaned and standardized:

### 1. Gender

Possible values:

```text
male
female
```

Values are standardized to maintain consistency.

### 2. Race/Ethnicity

Race/ethnicity categories are checked for:

* Missing values
* Incorrect formatting
* Inconsistent labels

### 3. Parental Level of Education

Education categories are standardized for analysis.

Example categories:

```text
some high school
high school
some college
associate's degree
bachelor's degree
master's degree
```

### 4. Lunch

Lunch categories are cleaned and standardized:

```text
standard
free/reduced
```

### 5. Test Preparation Course

Values are standardized as:

```text
none
completed
```

---

##  Statistical Analysis

Statistical measures are calculated for:

* Math Score
* Reading Score
* Writing Score

The following measures are calculated:

| Statistical Measure | Description              |
| ------------------- | ------------------------ |
| Mean                | Average score            |
| Median              | Middle value             |
| Standard Deviation  | Spread of scores         |
| Q1                  | 25th percentile          |
| Q2                  | 50th percentile / Median |
| Q3                  | 75th percentile          |
| Minimum             | Lowest score             |
| Maximum             | Highest score            |

### Example

```text id="5m3r9a"
Math Score
├── Mean
├── Median
├── Standard Deviation
├── Q1
├── Q2
├── Q3
├── Minimum
└── Maximum
```

---

##  Feature Engineering

New calculated features are created to better understand overall student performance.

### 1. Total Marks

Total marks are calculated using the three subject scores.

```text id="f7n2ka"
Total Marks = Math Score + Reading Score + Writing Score
```

Since each subject has a maximum score of 100:

```text
Maximum Total Marks = 300
```

### 2. Percentage Performance

The overall percentage is calculated as:

```text id="r2z8wp"
Percentage = (Total Marks / 300) × 100
```

This provides a simple overall measure of student performance.

---

##  Outlier Detection

Extreme performance values are identified across subject areas.

Outlier detection can be performed using the **Interquartile Range (IQR)** method.

### IQR Formula

```text id="v9q1bc"
IQR = Q3 - Q1
```

Lower Bound:

```text
Q1 - 1.5 × IQR
```

Upper Bound:

```text
Q3 + 1.5 × IQR
```

Scores outside these boundaries can be flagged as potential outliers.

Outliers should be investigated rather than automatically removed because an extreme score can represent a valid student result.

---

##  Outlier Analysis

Outliers are analyzed across:

* Math scores
* Reading scores
* Writing scores
* Total marks
* Percentage performance

The analysis helps identify unusually high or low performance values.

---

##  Exploratory Analysis

The cleaned dataset can be used to analyze:

* Average score by subject
* Score distribution
* Student performance percentages
* Subject-wise performance variation
* Relationship between subject scores
* Performance outliers
* Impact of test preparation on scores
* Performance patterns across demographic categories

---

##  Technologies Used

* **Python**
* **Pandas** – Data cleaning and feature engineering
* **NumPy** – Numerical calculations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Jupyter Notebook / Google Colab**

---

##  Project Workflow

```text id="q4x1mz"
Student Performance Dataset
          ↓
     Load Dataset
          ↓
   Data Understanding
          ↓
   Clean Categorical Data
          ↓
   Handle Missing Values
          ↓
   Statistical Analysis
          ↓
    Feature Engineering
          ↓
   Calculate Total Marks
          ↓
 Calculate Percentage Performance
          ↓
    Detect Outliers
          ↓
   Exploratory Analysis
          ↓
      Final Dataset
```

---

##  Project Structure

```text id="m5t7pk"
Student-Performance-Analysis/
│
├── StudentsPerformance.csv
├── Student_Performance_Analysis.ipynb
├── README.md
│
└── outputs/
    ├── cleaned_data/
    ├── statistical_analysis/
    └── visualizations/
```

---

##  Expected Outcomes

After completing this project, we can understand:

* The distribution of student scores.
* Average performance in each subject.
* Variation in student performance.
* Overall student percentage.
* Total marks obtained by students.
* Extreme performance values.
* Clean and standardized categorical features.
* Important patterns in student performance data.

---

##  Key Questions

This project attempts to answer:

1. What is the average score in each subject?
2. What are the median and standard deviation of the scores?
3. What are the Q1 and Q3 values for each subject?
4. What is the total score obtained by each student?
5. What is the overall percentage performance?
6. Are there extreme performance outliers?
7. Which subject shows greater variation in scores?
8. What patterns can be identified from the cleaned student dataset?

---

##  Conclusion

The **Student Performance Data Understanding, Cleaning & Feature Engineering** project demonstrates how raw student performance data can be cleaned, analyzed, and transformed into useful features.

Categorical features are standardized, statistical measures are calculated for subject scores, and new features such as **Total Marks** and **Percentage Performance** are created.

Outlier detection helps identify unusually high or low performance values and provides a better understanding of the overall student score distribution.

The resulting cleaned and enhanced dataset can be used for further **exploratory data analysis, visualization, and machine learning applications**.

---

##  Author

**Name:** Kirthik
**Project:** Student Performance Data Understanding, Cleaning & Feature Engineering
**Technology:** Python & Data Analysis
