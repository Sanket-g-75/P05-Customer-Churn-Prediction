# Customer-Churn-Prediction

1. Data
- Data shows there are a total of 9 columns out of which 6 are Numeric and 3 are Categorical
- No need for Data Type of Conversion required as the data is already in the prefered data Type
- No null values indicating there is no need to used the Null Values replacement Methods
- Given dataset has the binary labels 0 and 1

2. EDA
- Checked if the Labels are balanced or imbalanced
- Found the 3rd Standard Deviation bands for the Numerical classes and on analysis
  understood that all the values in all columns lie within these bands
- All the numerical features also have almost equal no. of observations w.r.t to 
  their bins
- All the Categorical features are also equally distributed
- Heatmap shows that there was almost 0 correlation between the features

3. Data Preprocessing 1
- Needed to remove the Name as it is an extension of CustomerID
- Also CustomerID is not relevant for the data as they are like indexes

4. Data Preprocessing 2
4.1 Encoding 
- Converted Location and Gender to One Hot Representations

4.2 Scaling
- Scaled all the numerical data
- Robust Scaler was used because it scales the data as per IQR. This was used because 
  the normal scalers assumes that data is normally distributed

5. Model
5.1 Splitting the Data
- Split the Train and Test Data as 70% and 30%

5.2 Model
- Random Forest Classifier was used as the Classifier as it is better to overfitting problem
  and is scalable to large datasets
- Started with n_estimators as 100 and  max_depth as 5

5.3 Metrics
- Prepared a Metrics Function which gives multiple metrics related to Classification
- Plotted Confusion Matrix 
- Calculated values like Accuracy, Precision, Recall, Specificity, F1 Score, AUC Score
- Also plotted the ROC Curve
- Also tried a Prediction for an Imaginary Observation

5.4 Fine Tuning
- In Fine Tuning, used the GridSearchCV method to test multiple parameters like the n_estimators
  and the max_depth values for Random Forest Classifier
- Best Hyperparameters represented were n_estimators as 300 and max_depth as 4
- Updated the parameters accordingly

5.5 Using XGBoost
- Used XGBoost model as well to test other models 

6. Model Deployment
6.1 Making a Pickle File
- Used pickle to download the model 
- Have created the app.py file such that it can be used to get the local website code 
  to test the model
- Not prepared the interface for the website because of unfamilirity with HTML Coding
