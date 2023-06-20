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
## Visualization of patients the likelyhood to have a stroke by age
![1st](https://github.com/Osmayda/Modeling/assets/129660519/bbafc1ee-8524-45d8-a964-b64b769b3443)
- People over 40 are more prone to having a stroke.

## Visualization of Stroke and BMI
![2nd vid](https://github.com/Osmayda/Modeling/assets/129660519/bc5e8325-2b7b-4053-a5bc-3d760dd9d948)
- Individual with lower BMI are more likely to have a stroke.

## Heart Disease and likelihood of Stroke
![image](https://github.com/Osmayda/Modeling/assets/129660519/b91dae96-8681-4156-82bb-a6420ae9504d)
0 if the patient doesn't have any heart disease
1 if the patient has a heart disease
-patients with no heart disease are more likely to have a stroke. This could be because patients with no heart disease probably do not check their heart health as frequently. Patients with heart disease are probably under medications and can it be assumed that they are under a doctor's care that would keep them better informed of how to prevent strokes.


# **Machine Learning Model Training Results**
#Metrics for best Model
- 94% accuracy
- 0.99 false negative
- .0025 false positive

# **Summary**
- The best model was KNN for this business problem. The KNN model is 94% accurate and has the lowest false negative results. In the models we want reduce false negatives as it means that patients are not being advised to the likelyhood of a stroke when they should be alerted. So reducing false negative is the best thing to do for this business problem. 


# **Recommendation**
- The best model overall is PCA with an accuracy of 93%. 
