Machine Learning Practical Assignment: Data Preprocessing & Feature Selection

1. Project Title

From Theory to Implementation: Data Preprocessing & Feature Selection on the Loan Prediction Dataset

2. Problem Statement

Retail and commercial banking organizations face high operational risks and delays in manual underwriting. This project automates credit risk assessment by preprocessing applicant profiles and isolating statistically significant predictive signals to classify whether a retail home loan will be approved or rejected.

3. Group Members

Students       Rollno            Contribution
Karan Kumar    CSJMA23001390019  
Tushar Agarwal CSJMA23001390127
Utkarsh Singh  CSJMA23001390050

4. Dataset Description

The dataset contains 614 applicant records with 12 input features and 1 binary target variable (Loan_Status). Features include applicant demographics such as Gender, Education, and Marital Status; financial metrics such as Applicant Income, Coapplicant Income, and Loan Amount; and historical credit information.

5. Dataset Source

Source: GitHub Loan Prediction Dataset

URL: Loan Prediction Dataset

6. Preprocessing Techniques Implemented

Missing Value Imputation: Median imputation for numerical features and mode imputation for categorical features.

Duplicate Detection: Row-wise comparison to identify duplicate observations.

Invalid/Inconsistent Data: Checks for impossible or inconsistent values and categorical formatting.

Categorical Encoding: Manual Label Encoding for suitable binary/ordinal variables and manual One-Hot Encoding for nominal categorical variables.

Outlier Treatment: Detection using IQR bounds and Z-score (|Z| > 3), followed by justified treatment of extreme observations.

Transformation: Log transformation investigated for heavily right-skewed numerical variables.

Feature Scaling: Manual Min-Max Normalization and Z-Score Standardization.

Leakage Prevention: Train-Test Split (80/20) performed before learning preprocessing parameters.

7. Feature-Selection Techniques Implemented

Variance Threshold: Identifies zero-variance and low-variance numerical features.

Pearson Correlation: Measures linear relationships between numerical variables and identifies potentially redundant features.

Chi-Square Test: Evaluates statistical dependence between categorical/discrete features and the categorical target.

ANOVA F-Test: Examines whether numerical feature means differ across loan-approval classes.

Mutual Information (MI): Measures shared information and can capture more general statistical dependencies, including nonlinear relationships.

8. From-Scratch Implementations

The major mathematical operations are implemented manually using Python, NumPy, and Pandas before verification with appropriate library functions.

Descriptive Statistics: Mean, Median, Mode, Variance, Standard Deviation, Range

Missing Value Imputation

Duplicate Detection

Label Encoding

One-Hot Encoding

IQR Outlier Detection

Z-Score Outlier Detection

Min-Max Normalization

Z-Score Standardization

Manual Train-Test Split

Variance Calculation

Pearson Correlation Coefficient

Chi-Square Contingency Table, Expected Frequencies and Degrees of Freedom

ANOVA F-Statistic

Shannon Entropy

Discrete Mutual Information

9. Results

The notebook calculates and displays the exact results after execution, including:

Original and final dataset shape

Missing values before and after treatment

Duplicate observations

Outliers detected using IQR and Z-score

Distribution/skewness before and after transformation

Normalized and standardized values

Training and testing dataset sizes

Variance scores

Pearson correlation values

Chi-Square statistics and degrees of freedom

ANOVA F-statistics

Mutual Information scores

Final selected and removed features

Before-vs-after preprocessing comparison

Optional model-based validation

Note: Numerical results should be taken directly from the executed Colab notebook rather than manually entered into this README.

10. Selected Features

The final selected feature set is determined by combining variance, correlation, Chi-Square, ANOVA, and Mutual Information results from the notebook.

The selected features will be listed here after the final analysis is executed.

11. Key Findings

Credit History: Credit history is expected to be an important signal for loan approval and is evaluated using categorical feature-selection techniques.

Income Distribution: Applicant and co-applicant income distributions are examined for skewness and potential transformation.

Categorical Variables: Categorical features are encoded according to their data type rather than applying one encoding method blindly.

Feature Redundancy: Pearson correlation is used to identify highly correlated numerical features.

Statistical Significance: Chi-Square and ANOVA are used according to the type of feature and target relationship.

Mutual Information: MI provides a broader measure of statistical dependence than Pearson correlation.

Data Leakage: Preprocessing and supervised feature-selection parameters are learned from training data before being applied to the unseen test data.

12. Instructions to Run the Code

Option 1: Google Colab

Open Google Colab.

Select File → Upload notebook.

Upload Loan_Prediction_ML_Practical_Assignment.ipynb.

Run the notebook cell by cell or select Runtime → Run all.

The notebook downloads the dataset directly from the specified GitHub URL.

Option 2: Clone the Repository

git clone https://github.com/your-username/ML-Preprocessing-Feature-Selection.git
cd ML-Preprocessing-Feature-Selection

Open the notebook:

jupyter notebook notebooks/Loan_Prediction_ML_Practical_Assignment.ipynb

Required Libraries

pip install pandas numpy matplotlib seaborn scipy scikit-learn

13. Google Colab Link

[Add Google Colab Link Here]



14. Assignment Compliance

This project follows the practical-assignment requirement:

Understand → Calculate → Code → Verify → Interpret

Ready-made preprocessing and feature-selection functions are not used as the primary implementation. Library functions are used afterward where appropriate for verification, as required by the assignment.

15. References

Loan Prediction Dataset: https://raw.githubusercontent.com/shrikant-temburwar/Loan-Prediction-Dataset/master/train.csv

Machine Learning Practical Assignment: Data Preprocessing & Feature Selection
