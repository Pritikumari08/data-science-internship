# Week 3 – Python-Based Machine Learning Model Development and Evaluation Plan

## Project Title

### Customer Churn Analysis and Prediction

## Objective

The objective of this project is to design a comprehensive machine learning development and evaluation plan for predicting customer churn.

The plan covers problem definition, data preprocessing, feature engineering, feature selection, model selection, model training, hyperparameter tuning, evaluation metrics, cross-validation, deployment, monitoring, and model maintenance.

This Week 3 task focuses on planning the machine learning workflow rather than implementing a complete model with real customer data.

---

## Project Background

Customer churn refers to customers discontinuing their use of a company's products or services.

For this hypothetical project, a telecom provider wants to identify customers who are likely to leave so that appropriate retention strategies can be planned.

The problem is treated as a **supervised binary classification problem**, where:

- `1` = Customer churned
- `0` = Customer stayed

The planned dataset contains customer information related to billing, usage, contracts, payments, and customer support.

---

## Machine Learning Workflow

The proposed workflow is:

1. Problem Definition
2. Data Understanding
3. Data Cleaning
4. Data Transformation
5. Feature Engineering
6. Feature Selection
7. Train-Test Split
8. Model Selection
9. Model Training
10. Hyperparameter Tuning
11. Cross-Validation
12. Model Evaluation
13. Deployment Planning
14. Monitoring and Maintenance

---

## Data Preprocessing Plan

The preprocessing strategy includes:

- Data quality checking
- Duplicate detection and removal
- Missing-value handling
- Outlier detection
- Data-type correction
- Categorical encoding
- Numerical feature scaling where required
- Data leakage prevention

A machine learning pipeline is planned so that preprocessing operations are learned only from the training data.

---

## Feature Engineering

Potential engineered features include:

- Charge per minute
- Support intensity
- Price change percentage
- New customer indicator
- Late payment rate
- Usage decline percentage

These features are intended to provide additional information that may help identify potential churn patterns.

---

## Feature Selection

The planned feature-selection techniques include:

- Correlation analysis
- Variance threshold
- Random Forest feature importance
- Permutation importance
- SHAP-based interpretation

Highly redundant or near-constant features will be considered for removal.

---

## Proposed Machine Learning Models

The following models are planned for comparison:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. XGBoost

Logistic Regression will be used as an interpretable baseline, while tree-based ensemble models will be evaluated for their ability to capture nonlinear relationships.

XGBoost is the planned primary candidate, but the final model would be selected only after actual training and validation.

---

## Class Imbalance Handling

The hypothetical dataset contains fewer churned customers than retained customers.

The planned approaches include:

- Class weighting
- Threshold tuning
- Precision-Recall analysis
- SMOTE inside the training pipeline when appropriate

Accuracy alone will not be used to judge the model because of the class imbalance.

---

## Model Evaluation Metrics

The planned evaluation metrics are:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- PR-AUC
- Log Loss / Brier Score

Recall is particularly important because missing a customer who is likely to churn may reduce the effectiveness of a retention strategy.

---

## Validation Strategy

A **stratified 5-fold cross-validation** strategy is planned for model comparison and tuning.

The test dataset will remain separate and will be used only for the final evaluation.

Additional validation checks include:

- Learning curves
- Time-based validation
- Calibration checks
- Subgroup performance checks
- SHAP-based explainability

---

## Hyperparameter Tuning

Hyperparameter tuning is planned using:

- RandomizedSearchCV
- Narrow grid search
- Optional Optuna optimization

For XGBoost, parameters such as the following may be tuned:

- `n_estimators`
- `max_depth`
- `learning_rate`
- `subsample`
- `colsample_bytree`
- `min_child_weight`

---

## Deployment and Maintenance Plan

The deployment concept includes:

- Saving the complete preprocessing and model pipeline
- Serving predictions through an API
- Docker-based packaging
- Monthly customer scoring
- MLflow-based experiment and model tracking

The model would be monitored for:

- Model performance
- Data drift
- Data quality
- API/system health

Retraining would be performed periodically or when monitoring indicates significant model degradation.

---

## Python Tools and Libraries

| Tool / Library | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data processing |
| NumPy | Numerical operations |
| Matplotlib | Visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | ML models, preprocessing and evaluation |
| XGBoost | Gradient boosting |
| Imbalanced-learn | SMOTE and imbalance handling |
| SHAP | Model explainability |
| Optuna | Optional hyperparameter optimization |
| Joblib | Model saving |
| FastAPI | API deployment concept |
| Docker | Application packaging |
| MLflow | Experiment and model tracking |
| Jupyter Notebook | Development and analysis |
| Git/GitHub | Version control |

---

## Expected Outcomes

The Week 3 task is expected to produce:

- A complete machine learning development plan
- A structured preprocessing strategy
- Feature engineering and selection strategy
- Candidate model comparison framework
- Hyperparameter tuning strategy
- Evaluation and validation framework
- Deployment and monitoring plan
- Professional documentation of the ML lifecycle

No real customer dataset or final production model is included in this planning task.

---

## Project Timeline

The planned effort is approximately **32 hours**.

| Phase | Hours |
|---|---:|
| Problem Definition | 3 |
| Data Understanding | 3 |
| Preprocessing | 5 |
| Feature Engineering and Selection | 4 |
| Model Selection and Training | 5 |
| Tuning and Cross-Validation | 4 |
| Evaluation and Interpretation | 4 |
| Deployment Planning and Documentation | 4 |
| **Total** | **32 Hours** |

---

## Deliverables

- `README.md`
- `Week-3-Project-Plan.docx`
- `ML-Development-Workflow.png`
- `Model-Evaluation-Framework.png`
- `Week3-Project-Timeline.png`

---

## Conclusion

Week 3 establishes a structured plan for developing and evaluating a Python-based machine learning solution for customer churn prediction.

The plan covers the complete machine learning lifecycle, from problem definition and preprocessing to model evaluation, deployment planning, monitoring, and maintenance.

The framework can also be adapted to other supervised classification problems such as fraud detection, customer retention, and loan default prediction.
