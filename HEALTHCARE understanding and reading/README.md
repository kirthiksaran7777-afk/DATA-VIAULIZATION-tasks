# Healthcare Data Understanding, Cleaning & Exploratory Analysis

##  Project Overview

This project focuses on understanding, cleaning, and performing exploratory data analysis (EDA) on a healthcare dataset.

The analysis helps identify patterns in patient demographics, medical conditions, hospital admissions, billing amounts, and hospital stay durations.

The main goal is to transform raw healthcare data into clean and useful information for analysis and decision-making.

---

##  Objectives

The main objectives of this project are:

1. Segment patient demographics based on medical conditions.
2. Clean missing values in medical codes.
3. Standardize date attributes for consistent analysis.
4. Categorize hospital admissions based on urgency.
5. Calculate summary statistics for patient billing amounts.
6. Calculate summary statistics for hospital stay duration.
7. Understand important patterns and trends in the healthcare dataset.

---

##  Dataset

**Dataset Name:** `healthcare_dataset.csv`

The dataset contains patient and hospital-related information such as:

* Patient details
* Age
* Gender
* Medical condition
* Admission date
* Discharge date
* Admission type
* Medical codes
* Billing amount
* Hospital stay duration

---

##  Data Cleaning

The following data-cleaning operations are performed:

### 1. Handling Missing Medical Codes

Missing values in medical code columns are identified and handled appropriately.

Possible approaches include:

* Replacing missing values with `"Unknown"`
* Removing records when necessary
* Using appropriate values based on the dataset

### 2. Standardizing Dates

Date columns are converted into a standard date format.

For example:

```text
MM/DD/YYYY
```

is converted into a consistent date format that can be easily analyzed.

### 3. Data Type Conversion

Columns such as dates, billing amounts, and numerical attributes are converted to appropriate data types.

### 4. Duplicate Checking

Duplicate records are identified and removed when necessary.

---

##  Admission Urgency Categorization

Hospital admissions are categorized into three urgency levels:

| Admission Category | Description                             |
| ------------------ | --------------------------------------- |
| Emergency          | Immediate medical attention is required |
| Urgent             | Medical attention is required soon      |
| Elective           | Planned medical treatment or admission  |

This categorization helps understand the distribution of different types of hospital admissions.

---

##  Demographic Segmentation

Patients are segmented according to their medical conditions.

The analysis can include:

* Number of patients per medical condition
* Age distribution
* Gender distribution
* Medical condition frequency
* Relationship between demographics and medical conditions

Example:

```text
Medical Condition → Age Group → Gender → Patient Count
```

---

##  Billing Amount Analysis

Summary statistics are calculated for patient billing amounts.

The analysis includes:

* Mean
* Median
* Minimum
* Maximum
* Standard deviation
* Total billing amount

Example:

```text
Mean Billing Amount
Median Billing Amount
Minimum Billing Amount
Maximum Billing Amount
Standard Deviation
```

---

## 🏥 Hospital Stay Analysis

Hospital stay duration is calculated using admission and discharge dates.

### Formula

```text
Hospital Stay = Discharge Date - Admission Date
```

The analysis includes:

* Average hospital stay
* Minimum stay
* Maximum stay
* Median stay
* Standard deviation

This helps understand how long patients typically remain in the hospital.

---

##  Exploratory Data Analysis

The following analysis can be performed:

### Medical Condition Analysis

* Most common medical conditions
* Number of patients for each condition

### Admission Analysis

* Emergency admissions
* Urgent admissions
* Elective admissions

### Demographic Analysis

* Age distribution
* Gender distribution
* Medical condition by gender
* Medical condition by age group

### Financial Analysis

* Billing amount distribution
* Average billing by medical condition
* Billing amount by admission type

### Hospital Stay Analysis

* Average stay duration
* Stay duration by medical condition
* Stay duration by admission urgency

---

##  Technologies Used

* **Python**
* **Pandas** – Data cleaning and analysis
* **NumPy** – Numerical calculations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Jupyter Notebook / Google Colab**

---

##  Project Workflow

```text
Healthcare Dataset
       ↓
Data Loading
       ↓
Data Understanding
       ↓
Data Cleaning
       ↓
Handle Missing Medical Codes
       ↓
Standardize Date Attributes
       ↓
Categorize Admission Urgency
       ↓
Calculate Hospital Stay
       ↓
Demographic Segmentation
       ↓
Billing & Stay Statistics
       ↓
Exploratory Data Analysis
       ↓
Insights & Conclusions
```

---

##  Project Structure

```text
Healthcare-Data-Analysis/
│
├── healthcare_dataset.csv
├── Healthcare_Data_Analysis.ipynb
├── README.md
│
└── outputs/
    ├── charts/
    └── cleaned_data/
```

---

##  Expected Outcomes

After completing this project, we can understand:

* Distribution of patients across medical conditions
* Demographic patterns among patients
* Number of Emergency, Urgent, and Elective admissions
* Average patient billing amount
* Minimum and maximum billing amounts
* Average hospital stay duration
* Medical conditions associated with longer hospital stays
* Important patterns in healthcare data

---

##  Key Questions

This project attempts to answer questions such as:

1. Which medical condition has the highest number of patients?
2. How are patients distributed by age and gender?
3. How many admissions are Emergency, Urgent, and Elective?
4. What is the average patient billing amount?
5. What is the average hospital stay?
6. Which medical conditions have longer hospital stays?
7. Are billing amounts different across medical conditions?
8. What patterns can be observed from the healthcare dataset?

---

##  Conclusion

The **Healthcare Data Understanding, Cleaning & Exploratory Analysis** project demonstrates how raw healthcare data can be cleaned, transformed, and analyzed using Python.

By handling missing values, standardizing dates, categorizing admission urgency, segmenting patient demographics, and calculating billing and hospital-stay statistics, meaningful insights can be obtained from the dataset.

This project provides a foundation for further healthcare analytics and data-driven decision-making.

---

##  Author

**Name:** Kirthik
**Project:** Healthcare Data Understanding, Cleaning & Exploratory Analysis
**Technology:** Python & Data Analysis
