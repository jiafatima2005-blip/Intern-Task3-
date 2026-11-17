# Intern-Task3-
# Predictive Customer Churn Classifier
### Customer Churn Prediction using Random Forest & XGBoost

## Project Overview
This project predicts whether a telecom customer is likely to leave the company (churn) using Machine Learning algorithms.

Two classification models are implemented:
- Random Forest Classifier
- XGBoost Classifier

The project uses data preprocessing, One-Hot Encoding, class imbalance handling, cross-validation, and model evaluation techniques to build and compare predictive models.

## Dataset
**Dataset:** Telco Customer Churn

The dataset contains 7,043 customer records and 21 columns, including:
- Customer demographics
- Account information
- Services subscribed
- Contract details
- Monthly and total charges
- Churn status

**Target Variable:** `Churn`
- `Yes` = Customer left the company
- `No` = Customer stayed with the company

## Technologies & Libraries
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- XGBoost

## Project Workflow

### 1. Data Loading & Exploration
- Load the telecom churn dataset.
- Explore dataset dimensions and columns.
- Analyze churn distribution.
- Identify missing values.

### 2. Data Preprocessing
- Convert `TotalCharges` into numeric format.
- Handle missing values.
- Remove irrelevant `customerID` column.
- Encode the target variable.
- Split data into training and testing sets.

### 3. Feature Engineering
- Separate numerical and categorical features.
- Apply One-Hot Encoding to categorical variables.
- Apply scaling to numerical features.
- Use a preprocessing pipeline.

### 4. Handling Class Imbalance
- Apply SMOTE with the Random Forest pipeline.
- Use class weighting through `scale_pos_weight` with XGBoost.

### 5. Model Training
Train and compare:
- Random Forest Classifier
- XGBoost Classifier

### 6. Cross-Validation
Use Stratified 5-Fold Cross-Validation to evaluate model performance using ROC-AUC.

### 7. Model Evaluation
Evaluate models using:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Classification Report

### 8. Visualizations
Generate:
- Churn distribution plot
- ROC Curve
- Confusion Matrix
- Top 10 Feature Importance plot

## Project Structure

```text
Predictive-Customer-Churn/
│
├── Predictive_Customer_Churn_Classifier.ipynb
├── Telco-Customer-Churn.csv
└── README.md
```

## Installation

Clone the repository:

```bash
git clone <your-repository-url>
cd Predictive-Customer-Churn
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost jupyter
```

## How to Run

1. Download or clone this repository.
2. Keep the notebook and CSV dataset in the same folder.
3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `Predictive_Customer_Churn_Classifier.ipynb`.
5. Run all cells sequentially.

## Expected Results

The project compares Random Forest and XGBoost using cross-validation and test-set evaluation.

The notebook generates:
- Model performance metrics
- ROC curves
- Confusion matrices
- Top 10 important features

**Note:** Actual model performance depends on the dataset and execution environment. No specific accuracy or ROC-AUC score is guaranteed.

## Key Learning Outcomes

- Data preprocessing and feature engineering
- One-Hot Encoding
- Handling imbalanced datasets
- SMOTE and class weighting
- Random Forest and XGBoost
- Stratified Cross-Validation
- ROC-AUC evaluation
- Feature importance analysis

## Author
**Your Name**

## License
This project is intended for educational and learning purposes.
