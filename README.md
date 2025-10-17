# assignment-6-Jerlinchellam12

Name : Jerlin Chellam J

Roll No: DA25C009

Documentation

# Imputation via Regression for Handling Missing Data

## Project Overview

This project focuses on handling missing data in a real-world machine learning scenario and analyzing its impact on classification performance. The dataset used is the **UCI Credit Card Default Clients Dataset**, which contains missing values in several important feature columns.  

As a machine learning engineer, our task is to prepare the data so that diffrent models can be effectively applied. Missing values in key features prevent direct use of standard algorithms, making **data imputation a crucial preprocessing step**.  

This setup demonstrates how the **choice of imputation method** can significantly influence the performance and reliability of predictive models in real-world applications like credit risk assessment.

---

## Objectives
1. Understand the effect of missing data on model performance.  
2. Compare different imputation techniques:  
   - Median Imputation  
   - Linear Regression Imputation  
   - Non-linear Regression Imputation  
3. Evaluate **listwise deletion**.  
4. Analyze the impact of each method on **classification metrics**: accuracy, precision, recall, F1-score.  
5. Recommend the best strategy for handling missing data based on both metrics and conceptual understanding.

---

## Dataset and Methodology
- The dataset contains **24 features** and missing values in some of the records.  
- Missing data handling strategies:
  - **Dataset A (Median Imputation):** Fill missing values with the median.  
  - **Dataset B (Linear Regression Imputation):** Predict missing values using linear regression.  
  - **Dataset C (Non-Linear Regression Imputation):** Predict missing values using a non-linear regression model.  
  - **Dataset D (Listwise Deletion):** Remove all rows with missing values.  

- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, Confusion Matrix.

---


**Observations:**
- Imputation methods retain **all data** while maintaining similar classification performance.  
- Listwise deletion has slightly higher accuracy and recall but loses many rows.  
- Differences among imputation methods are small; non-linear regression (C) performs slightly better than linear (B) or median (A).

---

## Insights

- **Data Retention:** Imputation preserves the dataset, allowing models to learn from all available information.  
- **Bias:** Listwise deletion can bias results if missingness is not completely random.  
- **Choice of Imputation Method:** 
  - Median imputation is simple and effective for roughly linear relationships.  
  - Regression-based imputation is more robust, especially non-linear regression for complex feature dependencies.  
- **Performance vs Completeness:** While deletion sometimes slightly improves metrics, the loss of data makes it less reliable for real-world applications.

---

## Conclusion
- **Best Strategy:** Regression-based imputation, for handling missing data.  
- Balances **classification performance** and **data integrity**.  
- Ensures the model can utilize **all available information** while maintaining statistical consistency.
