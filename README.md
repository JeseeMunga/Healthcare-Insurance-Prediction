# Healthcare Insurance Cost Analysis & Prediction
  

---

## Project Overview

This project analyzes a healthcare insurance dataset to understand the factors influencing medical insurance charges and to build predictive models for estimating insurance costs based on individual characteristics.  

The analysis combines **Exploratory Data Analysis (EDA), data preprocessing, regression modeling, and feature importance** to derive actionable insights for healthcare and insurance stakeholders.

---

## Dataset

The dataset contains 1,338 records and 7 columns:

| Column Name | Description |
|-------------|-------------|
| Age         | Age of the insured person |
| Sex         | Gender of the insured individual (male or female) |
| BMI         | Body Mass Index |
| Children    | Number of dependents covered under the insurance policy |
| Smoker      | Smoking status (yes/no) |
| Region      | Geographical region of insurance coverage |
| Charges     | Total medical insurance costs (target variable) |

 

---

## Objectives

Key questions addressed in this project:

1. Does age increase insurance costs?  
2. How much more do smokers pay compared to non-smokers?  
3. Does BMI influence insurance charges?  
4. Do people with more children pay more?  
5. Are there gender differences in charges?  
6. Which region has the highest costs?  
7. Which factors are the most important in predicting insurance charges?

---

## Tools & Libraries

- **Python 3.10+**  
- **Pandas** – Data manipulation  
- **NumPy** – Numerical computations  
- **Seaborn & Matplotlib** – Data visualization  
- **Scikit-learn** – Machine learning models & evaluation metrics

---

## Methodology

1. **Exploratory Data Analysis (EDA)**  
   - Distribution of charges, age, BMI, and children  
   - Relationships between categorical variables and charges  
   - Correlation analysis for numeric features  

2. **Data Preprocessing**  
   - One-hot encoding of categorical variables (`sex`, `smoker`, `region`)  
   - Train-test split (80% train, 20% test)

3. **Modeling**  
   - Linear Regression  
   - Decision Tree Regression  
   - Random Forest Regression  
   - Gradient Boosting Regression  

4. **Model Evaluation**  
   - Metrics: R², RMSE, MAE  
   - Comparison of performance for all models

5. **Feature Importance**  
   - Identify the most influential features driving insurance charges

---

## Results

| Model               | R²       | RMSE   | MAE   |
|--------------------|----------|--------|-------|
| Gradient Boosting   | 0.8815   | 4,289  | 2,424 |
| Random Forest       | 0.8682   | 4,523  | 2,533 |
| Linear Regression   | 0.7814   | 5,825  | 4,311 |
| Decision Tree       | 0.7293   | 6,483  | 3,057 |

**Top features driving insurance charges:**

1. Smoking status (`smoker_yes`)  
2. Age  
3. Body Mass Index (BMI)

---

## Insights

- **Smokers** pay significantly higher insurance charges than non-smokers.  
- **Older individuals and higher BMI** correlate with higher charges.  
- Number of **children and region** have smaller effects on costs.  
- **Gradient Boosting** provides the best predictive performance for this dataset.  
- Linear Regression is still useful for **interpreting feature effects** in reports.

**Business Value:**  
This analysis can help insurance companies:

- Estimate premiums for individuals based on their demographics and lifestyle  
- Identify high-risk groups for targeted interventions  
- Understand the most influential factors affecting healthcare costs

---

## How to Run

1. Clone the repository:  
```bash
git clone <your-repo-url>
