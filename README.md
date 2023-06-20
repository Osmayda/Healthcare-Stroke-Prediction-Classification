# Prediction of Stroke (Kaggle Dataset)
## by Osmayda Nino | osmaydanino@hotmail.com

# **Objective**
*The data from the Kaggle Dataset on strokes is used to determine whether a patient is likely to get a stroke based on the input parameters like gender, age, various diseases, and smoking status.*

Stakeholders: doctors, hospitals, patients, and insurance companies


The link to the dataset is: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

# **Dataset Description**
1. id: unique identifier
2. gender: "Male", "Female" or "Other"
3. age: age of the patient
4. hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5. heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6. ever_married: "No" or "Yes"
7. work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8. Residence_type: "Rural" or "Urban"
9. avg_glucose_level: average glucose level in blood
10. bmi: body mass index
11. smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"
12. stroke: 1 if the patient had a stroke or 0 if not

# **EDA plots and Observations**
## Visualization of patients the likelihood to have a stroke by age
![1st](https://github.com/Osmayda/Modeling/assets/129660519/bbafc1ee-8524-45d8-a964-b64b769b3443)
- People over 40 are more prone to having a stroke.

## Visualization of Stroke and BMI
![2nd vid](https://github.com/Osmayda/Modeling/assets/129660519/bc5e8325-2b7b-4053-a5bc-3d760dd9d948)
- Individuals with lower BMI are more likely to have a stroke. This could be to the patient not taking extra precautions to prevent a stroke due to the assumption that they are healthy. 

## Heart Disease and likelihood of Stroke
![changed](https://github.com/Osmayda/Modeling/assets/129660519/de697b19-c614-440e-8198-6e94752b8573)
0 if the patient doesn't have any heart disease
1 if the patient has a heart disease
-patients with no heart disease are more likely to have a stroke. This could be because patients with no heart disease probably do not check their heart health as frequently. Patients with heart disease are probably under medications and can it be assumed that they are under a doctor's care that would keep them better informed of how to prevent strokes.


# **Machine Learning Model Training Results**
##Tuned KNN
- Accuracy: 92%
- Recall: 14%

##Tuned Random Forest 
- Accuracy: 73%
- Recall: 80%

##Tuned XGBoost
- Accuracy: 94%
- Recall: 7%

##Tuned Under Sampling XGBoost
- Accuracy: 70%
- Recall: 77%

## Tuned KNN PCA
- Accuracy: 92%
- Recall: 19%

## Tuned Under Sampling PCA KNN
- Accuracy: 73%
- Recall: 69%

# **Summary**
- The best model is the Tuned Random Forest. The Tuned Random Forest model is 73% accurate and has the highest recall percentage. The model can accurately predict strokes 80% of the time. The models also have the lowest false negatives. This means patients who are likely to have a stroke were not advised of the likelihood of a stroke when they should have been alerted. Reducing false negatives so the model accurately predicts strokes is the objection and what is best for this problem.


# **Recommendation**
- The best model overall in predicting strokes is the Tuned Random Forest and I recommend this model for this business problem. 
