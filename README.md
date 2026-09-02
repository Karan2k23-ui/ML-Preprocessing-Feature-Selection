# Machine Learning Practical Assignment: Data Preprocessing & Feature Selection

## 1. Project Title

**From Theory to Implementation: Data Preprocessing & Feature Selection on the Loan Prediction Dataset**

## 2. Problem Statement

This project preprocesses loan applicant data and identifies statistically significant features to classify whether a home loan will be **approved or rejected**.

## 3. Group Members

| Student        | Roll Number      | Contribution
| -------------- | ---------------- | -------------
| Karan Kumar    | CSJMA23001390019 | Feature Selection + Final Dataset + Validation + Conclusion
| Tushar Agarwal | CSJMA23001390127 | Understanding + Exploration + Data Cleaning + Train/Test Split + Leakage
| Utkarsh Singh  | CSJMA23001390050 | Encoding + Outliers + Transformation + Scaling + Visualization

## 4. Dataset

The dataset contains **614 applicant records**, 12 input features, and the binary target **Loan_Status**. It includes demographic, financial, employment, property, and credit information.

**Source:** [Loan Prediction Dataset](https://raw.githubusercontent.com/shrikant-temburwar/Loan-Prediction-Dataset/master/train.csv)

## 5. Preprocessing

The project implements:

* Missing-value imputation
* Duplicate and invalid-data detection
* Label and One-Hot Encoding
* IQR and Z-score outlier detection
* Log transformation
* Min-Max Normalization
* Z-score Standardization
* 80/20 Train-Test Split
* Data Leakage Prevention

## 6. Feature Selection

The following techniques are implemented from scratch:

* Variance Threshold
* Pearson Correlation
* Chi-Square Test
* ANOVA F-Test
* Mutual Information

## 7. Implementation

Major calculations are implemented manually using **Python, NumPy, and Pandas**, followed by library-based verification.

**Workflow:**
`Understand → Calculate → Code → Verify → Interpret`

## 8. Project Structure

```text
dataset.csv
Loan_Prediction_ML_Practical_Assignment.ipynb
README.md
```

## 9. Run

Upload the notebook to **Google Colab** and select **Runtime → Run all**.

**Libraries:** `pandas numpy matplotlib seaborn scipy scikit-learn`

