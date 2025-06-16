# Customer Churn Prediction – STAR Report

### Situation
A leading company faced significant revenue loss due to customer churn, with an estimated churn rate of 26%. The business required a data-driven solution to identify at-risk customers and proactively reduce churn.

### Task
The objective was to:
- Analyze a large customer dataset (over 7,000 records, 20+ features).
- Build a predictive model to classify customers as likely to churn or not.
- Deploy an interactive dashboard for business users to visualize churn insights and predictions.

### Actions
1. **Data Exploration & Preprocessing**
   - Loaded and cleaned the dataset (`customer_churn_large_dataset.xlsx`).
   - Handled missing values, encoded categorical variables, and performed feature engineering.
   - Visualized key trends (e.g., churn by contract type, tenure, payment method).

2. **Model Development**
   - Split data into training and test sets (80:20 ratio).
   - Trained multiple models (Logistic Regression, Random Forest, XGBoost).
   - Selected the best model based on accuracy, precision, recall, and ROC-AUC.

3. **Evaluation**
   - Achieved an accuracy of **82%**, precision of **79%**, recall of **75%**, and ROC-AUC of **0.86** on the test set.
   - Identified top churn drivers: contract type, tenure, and monthly charges.

4. **Deployment**
   - Saved the trained model as `Model.pkl`.
   - Developed a user-friendly dashboard (`Customer_Churn_Prediction_Dashobard.pbix`) and a web app (`app.py`) for real-time predictions.
   - Provided a Jupyter notebook (`SanketGaikwad_ChurnPrediction.ipynb`) with full code and analysis.

### Results
- **Churn prediction accuracy:** 82%
- **Business impact:** Enables targeted retention strategies, potentially reducing churn by up to 10% and saving significant revenue.
- **Deliverables:** Clean code, interactive dashboard, and deployment-ready model.

---

## Repository Structure

- `SanketGaikwad_ChurnPrediction.ipynb`: Full code and analysis.
- `Model.pkl`: Trained machine learning model.
- `app.py`: Web app for live predictions.
- `Customer_Churn_Prediction_Dashobard.pbix`: Power BI dashboard.
- `customer_churn_large_dataset.xlsx`: Dataset used.
- `Project Info.txt`: Project summary and instructions.




