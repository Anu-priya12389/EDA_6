# Healthcare Data Analysis – Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a healthcare dataset containing patient information such as age, gender, medical condition, admission type, billing amount, insurance provider, length of stay, and admission date.

The main purpose of this analysis is to understand the dataset, identify patterns and distributions, and explore relationships between different healthcare-related variables using **Python, Pandas, Matplotlib, and Seaborn**.

---

## 🎯 Objectives

The main objectives of this project are:

- Understand the structure and characteristics of the healthcare dataset.
- Check the dataset size, columns, data types, and missing values.
- Analyze the age and gender distribution of patients.
- Study the distribution of different medical conditions.
- Analyze admission types and their relationship with medical conditions.
- Explore billing amount distributions.
- Compare billing amounts across medical conditions and insurance providers.
- Analyze monthly admission trends.
- Study the correlation between age, length of stay, and billing amount.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** – Data loading, cleaning, grouping, and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical data visualization
- **Jupyter Notebook** – Development environment

---

## 📂 Dataset

The analysis uses the following dataset:

`healthcare_new_preprocessed.csv`

The dataset contains healthcare and patient-related attributes, including:

- `Age`
- `Gender`
- `Medical_Condition`
- `Admission_Type`
- `Billing_Amount`
- `Insurance_Provider`
- `Admission_Date`
- `Length_of_Stay`

---

## 🔍 Analysis Performed

### 1. Dataset Exploration

The dataset is initially explored using:

- `head()` – View the first few records
- `shape` – Check the number of rows and columns
- `describe()` – Generate statistical summaries
- `isnull().sum()` – Check for missing values
- `columns.tolist()` – Display column names
- `info()` – Examine data types and dataset information

---

### 2. Age Distribution

A histogram with KDE is used to understand the distribution of patient ages.

The analysis also compares age distributions between different genders.

**Visualizations:**
- Age Distribution
- Age Distribution by Gender

---

### 3. Gender Distribution

The number of patients in each gender category is calculated and visualized using a bar chart.

This helps understand the overall gender composition of the dataset.

---

### 4. Medical Condition Analysis

The distribution of different medical conditions is analyzed using a bar chart.

The project also examines the distribution of genders across different medical conditions using a count plot.

---

### 5. Admission Type Analysis

The project analyzes the different types of hospital admissions.

A cross-tabulation is created between:

- Medical Condition
- Admission Type

A stacked bar chart is then used to visualize admission types across different medical conditions.

---

### 6. Billing Amount Analysis

The distribution of patient billing amounts is analyzed using a histogram.

A violin plot is used to examine billing amounts across different medical conditions.

The average billing amount for each medical condition is also calculated and visualized.

---

### 7. Insurance Provider Analysis

Billing amounts are analyzed based on insurance providers.

The project uses:

- Violin plots to show billing distributions.
- Grouped averages to calculate the average billing amount for each insurance provider.
- Bar charts to compare average billing amounts.

---

### 8. Monthly Admission Analysis

The `Admission_Date` column is converted into a datetime format.

The admission date is then converted into monthly periods to calculate the number of admissions for each month.

A line chart is used to visualize:

**Monthly Admissions Over Time**

This helps identify changes and trends in hospital admissions across different months.

---

### 9. Correlation Analysis

The following numerical variables are selected:

- `Age`
- `Length_of_Stay`
- `Billing_Amount`

A correlation matrix is calculated to examine the relationships between these variables.

---

## 📊 Visualizations Included

The notebook contains several visualizations, including:

- Age distribution histogram
- Age distribution by gender
- Gender distribution bar chart
- Medical condition distribution
- Medical condition by gender
- Admission type distribution
- Admission type by medical condition
- Billing amount distribution
- Billing amount by medical condition
- Average billing amount by medical condition
- Billing amount by insurance provider
- Average billing amount by insurance provider
- Monthly admissions line chart
- Correlation matrix

---

## 📁 Project Structure

```text
Healthcare-EDA/
│
├── EDA_6.ipynb
├── healthcare_new_preprocessed.csv
└── README.md
```

---

## ▶️ How to Run the Project

### 1. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 2. Place the dataset

Make sure `healthcare_new_preprocessed.csv` is available in the location used by the notebook.

The notebook currently loads the dataset using:

```python
pd.read_csv("/content/healthcare_new_preprocessed.csv")
```

If running locally, update the path accordingly.

### 3. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
EDA_6.ipynb
```

Run the cells sequentially to perform the analysis.

---

## 📌 Key Insights

The analysis focuses on identifying:

- Patient age and gender patterns.
- Distribution of medical conditions.
- Relationships between medical conditions and admission types.
- Differences in billing amounts across medical conditions.
- Differences in billing amounts across insurance providers.
- Monthly trends in hospital admissions.
- Correlations between age, length of stay, and billing amount.

> **Note:** Specific numerical insights depend on the `healthcare_new_preprocessed.csv` dataset used with the notebook.

---

## 🚀 Future Improvements

The project can be extended by:

- Adding more statistical analysis.
- Creating an interactive dashboard using Power BI or Plotly.
- Performing outlier detection.
- Analyzing relationships between additional healthcare variables.
- Creating predictive models based on the healthcare data.
- Adding a heatmap for easier interpretation of the correlation matrix.

---

## 👩‍💻 Author

**Anupriya V**

BCA – Computer Applications

**Project:** Healthcare Exploratory Data Analysis (EDA)
