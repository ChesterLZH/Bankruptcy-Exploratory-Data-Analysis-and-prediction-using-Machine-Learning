## <strong>Company Insolvency Exploratory Data Analysis and prediction using Machine Learning</strong>
This notebook aims to analyse the financials of 9792 Polish companies, and the solvency status of these companies to determine and predict insolvency risk.<br>
The final model was then compared against a dummy model and the Altman Z-Score to test its effectiveness using a test scenario<br>
<br>
The data of the companies are taken from the UCI Machine Learning Repository Repository: http://archive.ics.uci.edu/ml/datasets/polish+companies+bankruptcy+data

# Approach
1. Exploratory Data Analysis (EDA)
  - Understand data distributions and correlations between data and insolvency risk
2. Design Classification ML Model
  - Plan ML model using results from EDA
  - Selecting ML model 
  - Upsampling
  - Hyperparameter tuning
3. Analysis
  - Tuned model compared against dummy model to test for prediction accuracy
  - Tuned model compared against Altman's Z-Score in a test scenario to test for prediction accuracy

# Metric
1. Measuring Return of Investment (ROI) of ML model predictions or Altman's Z-Score to approve or deny loans in test scenario
2. ROI made from ML model predictions measured against ROI made from Altman's Z-Score predictions

# Conclusion
The tuned Gradient Boosting Classifier Model was more accurate in approving profitable loans, compared to using the Altman's Z-Score, and produced a greater ROI<br>
<br>
**Tuned Gradient Boosting Classifier Model:**<br>
f1 score: 0.201<br>
Final cash: $644500<br>
Approved loans: 2381<br>
Denied loans: 100<br>
Repaid loans: 2329<br>
Defaulted loans: 52<br>
<br>

**Altman's Z-Score:**<br>
f1 score: 0.098<br>
Final cash: $555500<br>
Approved loans: 2224<br>
Denied loans: 257<br>
Repaid loans: 2171<br>
Defaulted loans: 53<br>

