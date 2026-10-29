# Python DA Assignment 2 – Data Visualization

## 📌 Project Overview

This project focuses on data analysis and visualization using Python. The Seaborn `taxis` dataset is used to explore taxi trip information and identify patterns through different types of charts.

The assignment covers data loading, inspection, missing-value handling, and visualization using Matplotlib, Pandas, and Seaborn.

## 🎯 Objectives

* Load and explore the Taxis dataset.
* Inspect dataset dimensions, column names, and data types.
* Identify and handle missing values using appropriate techniques.
* Visualize fare trends over time.
* Compare total fares across pickup boroughs.
* Analyze trip distributions by payment method.
* Examine the distribution of trip distances and tips.
* Explore relationships and correlations between numerical variables.
* Compare fare distributions across payment methods.

## 🛠️ Technologies Used

* **Python** – Programming language
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical data visualization
* **Jupyter Notebook** – Interactive coding environment
* **GitHub** – Version control and project hosting

## 📂 Dataset

**Dataset Name:** Taxis Dataset

**Source:** Seaborn built-in dataset

The dataset is loaded directly using:

```python
import seaborn as sns

df = sns.load_dataset("taxis")
```

It contains information about taxi trips, including pickup and drop-off timestamps, locations, trip distance, fare, tips, tolls, total amount, and payment method.

No separate CSV file is required because the dataset is loaded directly from Seaborn.

## 📊 Tasks Performed

### 1. Dataset Loading and Inspection

* Loaded the Taxis dataset using Seaborn.
* Displayed the first five rows.
* Examined dataset dimensions and column names.
* Inspected data types and dataset structure.

### 2. Handling Missing Values

* Identified columns containing missing values.
* Removed rows with missing values in essential columns.
* Used median imputation for numerical columns.
* Used mode imputation for categorical columns.
* Checked the dataset for remaining missing values.

### 3. Visualizations Using Matplotlib and Pandas

**Line Chart – Fare Over Time**

* Visualized fare amounts against pickup timestamps.

**Bar Chart – Total Fare by Pickup Borough**

* Compared total fares across pickup boroughs.

**Pie Chart – Trips by Payment Method**

* Displayed the proportion of trips associated with different payment methods.

**Histogram – Distance Distribution**

* Examined the distribution of taxi trip distances using 20 bins.

**Box Plot – Tip Distribution by Pickup Borough**

* Compared tip amounts across pickup boroughs and identified potential outliers.

### 4. Visualizations Using Seaborn

**Count Plot – Trips by Pickup Borough**

* Compared the number of trips originating from different pickup boroughs.

**Scatter Plot – Distance vs Fare**

* Explored the relationship between trip distance and fare, with colors representing pickup boroughs.

**Heatmap – Correlation Analysis**

* Visualized correlations between distance, fare, tip, tolls, and total amount.

**Pair Plot – Pairwise Relationships**

* Examined relationships among distance, fare, tip, and total amount.
* Used pickup zones to distinguish observations.

**Violin Plot – Fare Distribution by Payment Method**

* Compared fare distributions across payment methods.

## 📈 Key Learning Outcomes

Through this assignment, I gained practical experience in:

* Loading and inspecting datasets using Pandas and Seaborn.
* Identifying and treating missing values.
* Working with numerical and categorical variables.
* Converting timestamps into datetime format.
* Performing grouping and aggregation operations.
* Creating different types of data visualizations.
* Analyzing relationships between numerical variables.
* Interpreting distributions, correlations, and potential outliers.
* Presenting data analysis results through visual representations.
