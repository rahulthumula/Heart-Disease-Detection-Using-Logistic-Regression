# Heart-Disease-Detection-Using-Logistic-Regression

This project aims to develop a logistic regression model to predict the presence of heart disease based on various clinical and non-clinical factors. The dataset used in this project is obtained from Kaggle [https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset], which contains 1026 rows of data and 14 columns.

## Dataset Description
The dataset contains the following columns:

age: age of the patient (in years)

sex: sex of the patient (1 = male; 0 = female)

cp: chest pain type (1 = typical angina, 2 = atypical angina, 3 = non-anginal pain, 4 = asymptomatic)

trestbps: resting blood pressure (in mm Hg)

chol: serum cholesterol (in mg/dl)

fbs: fasting blood sugar > 120 mg/dl (1 = true; 0 = false)

restecg: resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy)

thalach: maximum heart rate achieved

exang: exercise induced angina (1 = yes; 0 = no)

oldpeak: ST depression induced by exercise relative to rest

slope: the slope of the peak exercise ST segment (1 = upsloping, 2 = flat, 3 = downsloping)

ca: number of major vessels (0-3) colored by flourosopy

thal: 3 = normal; 6 = fixed defect; 7 = reversable defect

target: presence of heart disease (1 = yes, 0 = no)

## Methodology
The dataset is first preprocessed by scaling the features using StandardScaler from the sklearn.preprocessing library. The scaled dataset is then used to train a logistic regression model using statsmodels library. Backward elimination technique is used to remove features with a high p-value (above 0.05) in order to improve the accuracy of the model.

The accuracy of the final model is 0.8634146341463415, which is obtained by splitting the dataset into training and testing sets using train_test_split() method from sklearn.model_selection library. The confusion matrix is also generated to evaluate the performance of the model.

## Future Scope
In the future, this project can be improved by exploring other machine learning algorithms such as Random Forest, SVM, or Deep Learning algorithms to improve the accuracy of the model. The dataset can also be further analyzed to gain more insights into the factors affecting the presence of heart disease.
