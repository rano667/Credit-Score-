# Credit Score Analysis and FICO Score Calculation

This project focuses on an **Exploratory Data Analysis (EDA)** and a **hypothetical FICO score calculation** using a customer credit dataset. The goal is to analyze various customer features, clean the data, engineer new features, and calculate a hypothetical FICO score based on key factors such as **Payment History**, **Amounts Owed**, **Length of Credit History**, **New Credit Accounts**, and **Types of Credit Used**.

## Project Overview

The project involves:
1. **Data Cleaning**: Addressing missing values, outliers, and anomalies within the dataset.
2. **Feature Engineering**: Creating key features that influence a customer’s credit score.
3. **Hypothetical FICO Score Calculation**: Using a weighted approach to simulate the FICO score based on engineered features.
4. **Analysis and Insights**: Identifying customer risk categories, score distribution, and potential areas for intervention.

### Links
- **Colab Notebook**: [Click here to view the notebook](https://colab.research.google.com/drive/1cb9-_dLbn5AHMy5bHBD6RkQoE9Z1Sndk?usp=sharing)
- **Dataset**: [Download the dataset](https://drive.google.com/file/d/1pljm6_3nxcFS9UMIFm124HBsjNZP6ACA/view?usp=sharing)
- **Data Dictionary**: [View the Data Dictionary](https://docs.google.com/spreadsheets/d/1ZuK6o1MXFLmnhkFuDEedasDfVqu9ISPV/edit#gid=688359417)

## Dataset Overview

The dataset contains customer information with features such as:
- **SSN**
- **Annual Income**
- **Monthly In-Hand Salary**
- **Number of Bank Accounts**
- **Number of Credit Cards**
- **Payment History**
- **Credit Utilization**
- **Amount Owed**
- **Length of Credit History**

The dataset was cleaned and processed to handle invalid entries, missing data, and inconsistencies. The processed features were used to calculate a hypothetical FICO score.

## Data Cleaning

Several cleaning steps were undertaken:
- **Invalid SSNs** were replaced with the most frequent SSN per customer.
- **Missing values** were handled by replacing them with appropriate statistics such as the median.
- **Outliers** in features like the number of credit cards and loans were clipped to ensure data integrity.
- **Special characters and anomalies** (e.g., trailing underscores in numeric fields) were removed.

## Feature Engineering

The key features used in the FICO score calculation were:
1. **Payment History Score**: Evaluates the customer's payment consistency and history.
2. **Amounts Owed Score**: Assesses the customer’s debt relative to their credit limits.
3. **Length of Credit History Score**: Reflects the duration of the customer's credit history.
4. **New Credit Accounts Score**: Accounts for new credit opened recently by the customer.
5. **Types of Credit Used (Credit Mix)**: Considers the diversity of credit used (e.g., loans, credit cards).

### FICO Score Calculation
A weighted combination of the above factors was used to compute a hypothetical FICO score:
- **Payment History**: 35% of the score
- **Amounts Owed**: 30% of the score
- **Length of Credit History**: 15% of the score
- **New Credit Accounts**: 10% of the score
- **Types of Credit Used**: 10% of the score

The final FICO score was calculated for each customer in the dataset.

## Analysis & Insights

Key insights from the analysis:
1. The majority of FICO scores are concentrated between **500 and 720**, with a median score of **620**.
2. **60%** of the customers fall into the **Fair Risk** category, while **30%** are classified as **Poor Risk**, and **10%** as **Good Risk**.
3. There are very few outliers, indicating a relatively consistent credit score distribution.
4. Customers in the **Fair Risk** category could benefit from targeted financial counseling or credit improvement programs.

## Visualizations

Several visualizations were used to support the analysis:
- **Histograms** and **box plots** show the distribution of FICO scores and the presence of outliers.
- **Risk Category Breakdown** highlights the distribution of customers across different risk levels.

## Conclusion

This analysis provides valuable insights into customer credit behavior and risk levels. The hypothetical FICO score calculation offers a simulated view of creditworthiness, useful for understanding the key factors influencing credit scores.

## How to Use

1. Clone the repository.
2. Use the **Colab Notebook** to run the code and explore the analysis.
3. The **dataset** can be downloaded from the provided link.
4. Refer to the **data dictionary** for understanding the features.

