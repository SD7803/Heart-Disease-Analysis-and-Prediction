#Heart Disease Analysis and Prediction

End to end Machine Learning workflow to predict heart disease using Random Forest Classifier, GUI deployment and model persistence.

This data set dates from 1988 and consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach V. It contains 76 attributes, including the predicted attribute, but all published experiments refer to using a subset of 14 of them. The "target" field refers to the presence of heart disease in the patient. It is integer valued 0 = no disease and 1 = disease.

#Variables used:
1.age
2.sex
3.chest pain type (4 values)
4.resting blood pressure
5.serum cholestoral in mg/dl
6.fasting blood sugar > 120 mg/dl
7.resting electrocardiographic results (values 0,1,2)
8.maximum heart rate achieved
9.exercise induced angina
10.oldpeak = ST depression induced by exercise relative to rest
11.the slope of the peak exercise ST segment
12.number of major vessels (0-3) colored by flourosopy
13.thal: 0 = normal; 1 = fixed defect; 2 = reversable defect
The names and social security numbers of the patients were recently removed from the database, replaced with dummy values.

---------------------------------------------------------------
#Workflow Steps Followed:

1. Import Required Libraries:
   - pandas, numpy, matplotlib, seaborn
   - scikit-learn modules for preprocessing and modeling
   - joblib for model saving
   - tkinter for GUI-based deployment

2. Load Dataset:
   - Read 'heart_data.csv' into a pandas DataFrame
   - Preview head of dataset to understand structure

3. Data Quality Check:
   - Check dataset shape and information
   - Identify missing values and duplicate rows
   - Remove duplicates to ensure clean data

4. Feature Engineering:
   - Split columns into categorical and numerical
   - Encode categorical variables using get_dummies(drop_first=True)

5. Feature Scaling:
   - Apply StandardScaler to normalize continuous features

6. Train Test Split:
   - Split data into training and testing sets
   - Maintain randomness and reproducibility

7. Model Building:
   - Use RandomForestClassifier for prediction
   - Fit model using training data

8. Model Evaluation:
   - Evaluate using Accuracy score
   - Generate Confusion Matrix and Classification Report
   - Visualize performance insights

9. Prediction Testing:
   - Build a sample input vector
   - Predict whether a patient has heart disease or not

10. Model Saving:
    - Save trained model as `model_joblib_heart` using joblib

11. GUI Application (Tkinter):
    - Create a user-friendly interface for prediction
    - Accept input features and display prediction result in real time
---------------------------------------------------------------

