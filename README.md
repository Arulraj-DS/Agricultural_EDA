####################################################################################################################################################################

Project Summary
----------------

This project analyzes India’s agricultural data using Python, SQL, EDA, and Power BI to uncover trends in crop production, cultivated area, and yield. It identifies high- and low-performing regions and provides clear insights through interactive dashboards. The goal is to support better decision-making for farmers, researchers, and policymakers through data-driven insights.

Technologies Used
------------------

Python – Core programming language

Pandas – Data cleaning, manipulation, and analysis

SQL – Querying and retrieving data from the database

MySQL – Database used to store processed records

Seaborn & Matplotlib – Data visualization in Python

Power BI – Visualizing data using interactive charts and dashboards

Scikit-Learn – Used for checking correlation and normalization

Data Processing
-----------------

The original dataset contained 80 columns and 16,146 rows.

During data cleaning and preprocessing, the following steps were performed:

Checked for Missing & Duplicate Values : The dataset contained no null values and no duplicate records.

Handled Invalid Negative Values (-1) : Certain production and area fields had -1, which is invalid because crop output and land area cannot be negative.

These values were replaced:  -1 → 0

Standardized Column Names
--------------------------

Cleaned column names using strip()

Ensured proper casing and corrected inconsistent naming.

Removed Rows Containing All-Zero Values

Records where all columns had a value of 0 were dropped.

Final row count after cleaning: 16,084 rows

Feature Selection
------------------

Based on project requirements, selected 26 final features.

Final dataset shape:

16,084 rows × 26 columns


Separated Columns by Data Type
--------------------------------

Numeric columns

Object/string columns


Exploratory Data Analysis (EDA)
---------------------------------

Performed detailed EDA to understand patterns and distribution:

➡️ Distribution Analysis

Used Skewness and Kurtosis to study numerical column distribution.

➡️ Outlier Detection

Detected and analyzed outliers using boxplots.

➡️ Correlation Analysis

Generated a correlation heatmap (numeric columns only) to find relationships between area, production, and yield.

➡️ Data Visualization

Using Seaborn and Matplotlib, visualized:

Trends

Distributions

Outliers

Relationships between crops and regions


Database Integration
----------------------

Exported the cleaned dataset to Excel.

Imported the Excel file into MySQL.

Created SQL scripts for: Production trends , Yield analysis , Top/Bottom performing districts , Crop-wise comparisons


#######Power BI Dashboard#######
---------------------------------

Imported the SQL outputs into Power BI and created multiple interactive dashboards.

Visuals Used: 

Line Chart

Multi-Line Chart

Bar Chart

Column Chart

Area Chart

Map Visualization

Matrix (with conditional formatting)


#######Dashboard Highlights#######
-----------------------------------

**Trends in crop production and yield

**State-wise and district-wise performance

**Correlation insights

**Top/Bottom performing regions

**Growth patterns across years
