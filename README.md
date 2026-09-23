## 1. 📈 Shopify Stock Data Analysis

### Shopify Stock Data Understanding, Cleaning & Exploratory Analysis

This section focuses on understanding and preparing Shopify stock data for analysis.

### Activities

* Load the Shopify stock dataset.
* Inspect the dataset structure.
* Display the first and last records.
* Check data types.
* Check dataset information.
* Identify missing values.
* Remove duplicate records where required.
* Convert date columns into the appropriate date format.
* Generate descriptive statistics.
* Examine stock price and trading volume information.

### Key Stock Attributes

* Date
* Open
* High
* Low
* Close
* Adjusted Close
* Volume

### Tools Used

```text
Python
Pandas
NumPy
Matplotlib
```

---

###  Shopify Stock Visualization, Time-Series Analysis & Financial Insights

This section focuses on visualizing stock-price movements and extracting financial insights from the time-series data.

### Analysis Includes

* Stock price visualization
* Open, High, Low and Close price analysis
* Trading volume analysis
* Time-series visualization
* Identification of price movements and trends
* Analysis of changes in stock prices over time
* Financial interpretation of the observed patterns

### Objective

The objective is to understand how Shopify's stock price and trading volume change over time and present the observations through meaningful visualizations.

---

# 2.  Healthcare Data Analysis

## Healthcare Data Understanding, Cleaning & Exploratory Analysis

The healthcare notebook uses the `healthcare_dataset.csv` dataset.

The dataset contains **55,500 records** and includes patient, admission, hospital, insurance, billing, medication, and test-result information.

### Activities

* Load the healthcare dataset.
* Display the first and last records.
* Examine dataset structure.
* Check column names and data types.
* Check missing values.
* Generate descriptive statistics.
* Analyze billing amounts.
* Convert admission and discharge dates into datetime format.
* Calculate hospital stay duration.

### Important Attributes

* Name
* Age
* Gender
* Blood Type
* Medical Condition
* Date of Admission
* Doctor
* Hospital
* Insurance Provider
* Billing Amount
* Room Number
* Admission Type
* Discharge Date
* Medication
* Test Results

The dataset contains admission types such as **Emergency, Elective, and Urgent**.

### Stay Duration

A new feature called `Stay_Days` is created:

```python
df['Stay_Days'] = (
    df['Discharge Date'] -
    df['Date of Admission']
).dt.days
```

This calculates the number of days between admission and discharge.

### Billing Analysis

Descriptive statistics are calculated for `Billing Amount`, including:

* Count
* Mean
* Standard deviation
* Minimum
* Maximum
* Quartiles

The notebook records 55,500 billing observations.

---

##  Healthcare Data Visualization, Cost Relationship & Policy Insights

This section focuses on using visual analysis to understand healthcare costs and relationships within the dataset.

### Analysis Includes

* Healthcare data visualization
* Billing amount analysis
* Hospital stay analysis
* Admission-type analysis
* Medical-condition analysis
* Demographic segmentation
* Cost relationship analysis
* Comparison of healthcare-related attributes

### Objective

The objective is to identify meaningful relationships between healthcare characteristics and billing amounts and use the observed patterns to discuss possible **policy-related insights**.

> **Note:** Policy insights should be treated as analytical observations from this dataset rather than general conclusions about real-world healthcare systems.

---

# 3.  Student Performance Data Analysis

## Student Performance Data Understanding, Cleaning & Feature Engineering

The student performance notebook uses `StudentsPerformance.csv`.

The dataset contains **1,000 student records** and 8 columns.

### Activities

* Load the student performance dataset.
* Display sample records.
* Check data types.
* Inspect dataset information.
* Check missing values.
* Generate descriptive statistics.
* Identify categorical columns.
* Standardize categorical values.
* Create new features for student performance.

### Dataset Attributes

* Gender
* Race/Ethnicity
* Parental Level of Education
* Lunch
* Test Preparation Course
* Math Score
* Reading Score
* Writing Score

The notebook confirms that the dataset contains no missing values in these columns.

### Data Cleaning

Categorical columns are standardized using:

```python
df[col] = df[col].str.strip().str.title()
```

This removes unnecessary spaces and standardizes capitalization.

### Feature Engineering

Two new features are created.

#### Average Score

```python
df['average_score'] = (
    df['math score'] +
    df['reading score'] +
    df['writing score']
) / 3
```

#### Total Score

```python
df['total_score'] = (
    df['math score'] +
    df['reading score'] +
    df['writing score']
)
```

These features provide an overall measure of student performance.

---

# 🛠️ Technologies Used

| Technology                      | Purpose                             |
| ------------------------------- | ----------------------------------- |
| Python                          | Programming and analysis            |
| Pandas                          | Data loading, cleaning and analysis |
| NumPy                           | Numerical operations                |
| Matplotlib                      | Data visualization                  |
| Seaborn                         | Statistical visualization           |
| Google Colab / Jupyter Notebook | Development environment             |

---

# 📁 Project Structure

```text
Data-Analysis-Project/
│
├── Shopify/
│   ├── Shopify_Stock_Analysis.ipynb
│   └── Shopify_Stock_Data.csv
│
├── Healthcare/
│   ├── Healthcare 1.ipynb
│   └── healthcare_dataset.csv
│
├── Student-Performance/
│   ├── Untitled16.ipynb
│   └── StudentsPerformance.csv
│
└── README.md
```

---

# 🔄 Overall Data Analysis Workflow

```text
          Dataset
             ↓
      Data Understanding
             ↓
       Data Inspection
             ↓
       Data Cleaning
             ↓
    Missing Value Checking
             ↓
      Data Transformation
             ↓
   Feature Engineering
             ↓
  Exploratory Data Analysis
             ↓
       Visualization
             ↓
       Relationship Analysis
             ↓
          Insights
```

---

# 🎯 Project Objectives

### Shopify Stock

* Understand stock-market data.
* Clean and prepare stock data.
* Visualize stock-price movements.
* Perform time-series analysis.
* Identify financial patterns from the available data.

### Healthcare

* Understand healthcare records.
* Clean and transform healthcare data.
* Analyze billing and hospital stays.
* Explore relationships between healthcare variables.
* Develop dataset-based policy insights.

### Student Performance

* Understand student demographic and score data.
* Clean categorical attributes.
* Check data quality.
* Create `average_score` and `total_score`.
* Perform feature engineering for performance analysis.

---

# 📊 Key Learning Outcomes

Through these projects, the following Python data-analysis skills are demonstrated:

* Reading CSV and Excel datasets
* DataFrame operations
* Data inspection
* Data cleaning
* Missing-value analysis
* Duplicate detection
* Date and time conversion
* Descriptive statistics
* Feature engineering
* Time-series analysis
* Data visualization
* Relationship analysis
* Interpretation of analytical results

---

# 🚀 How to Run the Project

### 1. Install Python

Install Python 3.x on your system.

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

or use **Google Colab**.

### 4. Upload the Required Dataset

Keep the corresponding dataset in the same working directory as the notebook.

### 5. Run the Notebook

Run the cells sequentially from top to bottom.

---

#  Conclusion

This project demonstrates a complete introductory data-analysis workflow using three different domains:

**Financial Data → Healthcare Data → Educational Data**

The Shopify analysis focuses on **stock understanding, visualization, time-series analysis, and financial insights**.

The Healthcare analysis focuses on **data understanding, cleaning, visualization, cost relationships, and policy insights**.

The Student Performance analysis focuses on **data understanding, cleaning, and feature engineering**.

Together, these notebooks demonstrate how Python can be used to transform raw datasets into structured information and meaningful analytical insights.
