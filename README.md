# Cardiovascular Risk Prediction
Project Name - Cardiovascular Risk Prediction

Project Status - Complete

Language Used - Python with Pandas, Numpy, Matplotlib, Seaborn, geopy, SKlearn, XGBoost and SHAP libraries

Problem Statement - The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD).
The dataset provides the patients information. It includes over 4,000 records and 15 attributes.

Approach - To explore the data in the dataset and extract useful insights from the dataset based on the insights we will be training various machine learning models on some part of the data and the remaining part of data we will be using for testing the trained machine learning models. For the best performing machine learning models we will try to explain the prediction with the help of one of the model explainability technique - SHAP.

Conclusion - 

We have successfully predicted the risk of 10yr CHD.
As a part of this project we perform data cleaning EDA on this project.
Following are some useful insights from the EDA -
* The risk of CHD increases as the age increases from 35. People with age around 63 are at the highest risk of CHD.
* People belonging to education type 1 are at a higher risk of CHD then type 2 and type 3, people belonging to type 4 education are at the lowest risk of having CHD.
* Even though the number of males are less than number of females in the dataset still males are having more risk of 10yr CHD as compared to females.
* Risk of 10 yr CHD is more for smokers than non smokers.
* People who are on BP Meds are having more chance of having CHD.
* Person having stroke in the past 45% of them has a risk of CHD.
* 14% of the non-diabetic patient are at a risk of TenYearCHD whereas this number increases to 38% in case of diabetic patient.
* Risk of TenYearCHD increases with the increase in Cholestrol level.

Following Machine Learning models are used in this project with their corresponding performance metrics on the test data -

![image](https://user-images.githubusercontent.com/112267616/210786896-97309066-5690-469b-b5f8-d40bf4e0201f.png)

From the above metrics its clear that XG Boost is the best performing model.

SHAP is used to explain the results of XG Boost classifier.

From the charts plotted through SHAP we infer,
* Gender is the most influencing factor in prediction.
* age, cigsPerDay, pulsePressure & heartRate also shows good contribution in prediction.
* Other features are having less contribution in prediction. Least being BPMeds & prevalentStroke.
