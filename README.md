# Communicate Data Findings
## by (Chukwunonso Emmanuel Chukwumaeze)
<br>

## Pima Indians Diabetes Dataset

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases, version was downloaded from [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

The datasets consists of several medical predictor variables and one target variable, Outcome. Predictor variables includes the number of pregnancies the patient has had, their BMI, insulin level, age, and so on.

Several constraints were placed on the selection of these instances from a larger database. __In particular:
> * All Patients here are females
> * All Patients are at least 21 years old of Pima Indian heritage.__

I chose to work on all variables:
> The dataset contains about 768 rows with 9 columns. For my analysis I would be working on all rows and columns which includes:
> * __pregnancies__ : Number of times pregnant
> * __glucose__ : Plasma glucose concentration in a 2 hour oral glucose tolerance test. (mg/dL) [Read More about this test here](https://www.mayoclinic.org/tests-procedures/glucose-tolerance-test/about/pac-20394296)
> * __blood_pressure__ : Diastolic blood pressure (mmHg)
> * __skin_thickness__ : Triceps skin fold thickness (mm)
> * __insulin__ : 2-Hour serum insulin(mu U/ml)[Read More about Insulin Tests here](https://medlineplus.gov/lab-tests/insulin-in-blood/)
> * __bmi__ : Body Mass Index (weight in kg/(height in m)^2)
> * __diabetes_pedigree_function__ :  indicates the function which scores likelihood of diabetes based on family history.
> * __age__ : everyone in this dataset is above 21 years old.
> * __diabetes__ : whether individuals have diabetes or not, 0 - No, 1- Yes.


## Summary of Findings
<br>
In the Exploration I found that the variables that showed significant difference with regards to the diabetic outcome included the Insulin, Glucose, BMI and Diastolic Blood Pressure. I also found out that the number of pregnancies didn't correlate with BMI or skin thickness and that there was a positive correlation between BMI and skin thickness.

I had to engineer a new categorical column, grouping the BMI into health-significant categories according to the [CDC guidelines](https://www.cdc.gov/obesity/basics/adult-defining.html)

Upon further investigation I found out that there was no significant relationship between the Diabetes Pedigree Function and the diabetic status of the patients.
I also discovered a unique age distribution among diabetic patients.

## Key Insights for Presentation
<br>
For the presentation I focus on the variables which have the strongest correlation with the diabetes status of a patient. 

I start by looking at the distribution of the diabetes status of the patients, then exploring the BMI  distribution of patients across the diabetes status.

I further go into investigating the influence that age, glucose and insulin levels have on the diabetes outcome of the patients.

I would later go on to investigate the combined effects of Age and BMI on diabetes and the correlation between Glucose, Insulin, BMI and the diabetes status of patients.

I made sure to use positional and non-positional encodings where necessary to highlight the interactions between different variables.
