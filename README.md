# Drug-Data-Analysis-Sql-Window-Functions-
This project demonstrates the use of advanced SQL concepts, especially window functions, to analyze a pharmaceutical drugs dataset. The objective is to answer real-world analytical questions related to drug effectiveness, satisfaction, reviews, and labeling status.

### Dataset

The analysis is performed on a cleaned drug dataset (drug_clean). The dataset contains information such as:

Drug name

Medical condition (drug_condition)

Drug type (RX / OTC / RX-OTC)

Satisfaction score

Effectiveness score

Number of reviews

Price

Indication (On Label / Off Label)

Note: Column names like Condition and Type were renamed to avoid SQL reserved keywords


## SQL Concepts Used

Window Functions

ROW_NUMBER()

DENSE_RANK()

RANK()

AVG() OVER()

MAX() OVER()

FIRST_VALUE()

Common Table Expressions (CTEs)

Analytical aggregations

Ranking and Top-N analysis

Median calculation using window functions

Rolling and running calculations


## Business Questions Answered

# 1. Average Satisfaction: On-label vs Off-label Drugs

For each medical condition, the project calculates the average satisfaction level of drugs categorized as On Label and Off Label.

# 2. Average Effectiveness of Top 3 Most Reviewed Drugs

For each medical condition:

Drugs are ranked by number of reviews

# Top 3 most reviewed drugs are selected

Average effectiveness is calculated

This highlights the most trusted drugs based on user engagement.

# 3. Median Satisfaction Level per Medical Condition

Calculates the median satisfaction score for each condition

Uses ROW_NUMBER() and COUNT() window functions

Results are sorted in descending order of median satisfaction

# 4. Ranking and Comparison Analysis

The project includes multiple ranking-based insights such as:

Top drugs by review count

Ranking drugs within each condition

Comparing drug metrics against group-level statistics

# 5. Rolling and Window-Based Metrics

Demonstrates advanced analytics such as:

Rolling averages

Difference from group averages

Difference from top-performing drugs

These techniques are useful for trend analysis and benchmarking.


# How to Use

Load the dataset into a SQL database (MySQL / PostgreSQL)

Run queries from drugs_sql.txt

Review results for each analytical question

Modify queries to explore additional insights

# Skills Demonstrated

Advanced SQL querying

Window functions and analytical SQL

Data aggregation and ranking

Business-focused data analysis

Clean and readable SQL coding style

# Key Learnings

When to use window functions vs GROUP BY

How to calculate median in SQL

How to perform Top-N analysis correctly

Importance of proper partitioning and ordering

# Author

Sayli Munde
Aspiring Data Analyst | SQL | Python | Power BI | Tableau
