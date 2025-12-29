# Cost-AwareMachineLearning-AirQuality-Cybersecurity
Applied machine learning project covering regression and classification under real-world cost constraints. Part 1 predicts CO pollution using sensor data while balancing accuracy vs hardware cost. Part 2 detects cyber attacks from network flows using cost-sensitive classifiers and threshold tuning.


# Cost-Aware Machine Learning for Air Quality & Cybersecurity

This repository contains an applied machine learning project focused on building
interpretable and cost-sensitive models for two real-world problems:
air pollution monitoring and cyber attack detection.

---

## Project Structure

- `q1/` – Air pollution regression task (Dataset 1)
- `q2/` – Cyber attack classification task (Dataset 2)
- `README.md` – Project overview

---

## Part 1: Air Pollution Monitoring (q1)

**Goal:**  
Predict ground-truth CO concentration using low-cost environmental sensors while
balancing prediction accuracy against hardware cost.

**Key steps:**
- Data cleaning and missing value imputation
- Correlation and multicollinearity analysis
- OLS, Ridge, Lasso, and Kernel Ridge regression
- Model comparison using R², MAE, and RMSE
- Sensor cost vs accuracy analysis using Lasso paths
- Selection of low-cost and high-performance sensor configurations
- Cost-sensitive alert threshold analysis

**Main findings:**
- Regularisation improves stability and interpretability
- Lasso enables effective sensor selection under budget constraints
- Increasing sensor cost yields diminishing returns beyond a threshold

---

## Part 2: Cyber Attack Detection (q2)

**Goal:**  
Detect malicious network traffic while minimising expected cost, where false
negatives are far more expensive than false positives.

**Key steps:**
- Exploratory analysis and class balance assessment
- Logistic and penalised logistic regression
- Linear and kernel SVMs with cross-validation
- Feature stability analysis via bootstrapping
- ROC-based threshold tuning for cost minimisation
- Model comparison under asymmetric costs

**Main findings:**
- Penalisation improves feature stability and robustness
- Kernel methods achieve stronger detection performance
- Cost-aware threshold tuning significantly reduces expected loss

---

## Technologies Used

- Python
- NumPy, Pandas
- Scikit-learn
- Statsmodels
- Matplotlib / Seaborn

---

## Notes

- Dataset 1 corresponds to **q1**
- Dataset 2 corresponds to **q2**
- All models are evaluated using an 80/20 train-test split
- Hyperparameters are selected via cross-validation

---
