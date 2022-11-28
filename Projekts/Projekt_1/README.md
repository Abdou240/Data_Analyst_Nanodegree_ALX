# Medical Appointments No-Shows

## Overview

The objective of this project is to study a dataset of appointment data for public hospitals in Brazil. The data contains some attributes of patients and indicates whether patients showed up for appointments. The analysis should focus on finding trends that influence the appearance or non-appearance of patients to appointments. Descriptive statistics should be used to answer the following question: What factors do we need to know to predict whether a patient will show up for their scheduled appointment? Predictive analytics is outside the scope of this project.

The original problem description and data set can be found here: 
[Medical Appointment No Shows](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

This project was completed as part of the [Data Analyst Nanodegree](https://www.alxafrica.com/programme_post/data-analyst/) certification from Udacity.

## Details
I examined the dataset and solved some problems, such as unifying names, removing incorrect data, and adding new features based on existing data. I also looked at most of the independent variables in the dataset and made some observations to compare them to each other and to the dependent variable (no_show). Since this was only an exploratory analysis, many potential correlations may remain undetected. The data should be further explored with more advanced statistical analyses to potentially uncover new findings and correlations.

For details, see the analysis documentation [Jupyter Notebook](https://github.com/Abdou240/Project_ALX/blob/main/Projekts/Projekt_1/investigate-a-dataset.ipynb) or [HTML].

## Findings
Key findings are:
- Visit scheduling began on 2015-11-10 and ended on 2016-06-08.
- Visit scheduling began on 2016-04-29 and ended on 2016-06-08.
- The distribution of appointments among weekdays (Monday-Friday) is almost the same, with slightly fewer visits on Thursday and Friday. There are 24 visits on Saturday and none on Sunday.
- On average, patients waited 10 days for an appointment. 50% of patients waited up to 4 days and 75% waited up to 15 days for an appointment. The longest wait was 179 days.
- Nearly 40,000 patients scheduled their visit for the same day.
- Of all patients who scheduled an appointment for the same day (38561 total), 1792 patients did not show up (5%).
- The dataset contains many very young people (most of them are 0 years old), but in general the age of patients is evenly distributed, and the number of patients decreases dramatically for patients over 60 years old.
- The average age of patients is 37. 25% of patients are under 18 years old and most of them are under 55.
- Most patients are not alcoholics.
- Most patients do not have diabetes, but more than alcoholics.
- There are categories for disabilities, with most patients being nondisabled.
- Most patients were not diagnosed with hypertension.
- On average, 20% of appointments were missed.
  - Of 71831 appointments attended by women, 14588 were not attended, a rate of 20%.
  - Of 38685 appointments attended by men, 7723 were missed, a rate of 20%.
- There are patients with multiple appointments. The number of appointments of the top 10 patients ranges from 88 to 55. Considering that the time span of the agreed visits spans 3 months, an appointment is most likely any examination or specialist visit. Thus, within one patient visit to a hospital, there may be multiple appointments scheduled. One of the reasons for no-shows could be that patients are too tired to attend all examinations during a given visit, or that opening hours are insufficient to accommodate all appointments. There could be other reasons as well. The high number of appointments in such a short period of time should be discussed with an SME to conduct additional analysis in this area (or not).
- For all categorical variables, the distributions of show up/not show up look very similar for different categories. There is no clear indication that any one of these variables has a greater impact on appearance/non-appearance than others. The charts confirm a no-show rate of about 20% for most categories.
- The shorter the wait time, the more patients show up. Patients who make an appointment for the same day are much more likely to show up (only about 17% of no-shows).

## Statistical analysis Scope
- Data Processing
- Exploratory Data Analysis (EDA).
- Examination of central tendency and dispersion
- Data visualizations

## Tools
- Python, libraries: numpy, pandas, matplotlib, seaborn, warnings.
- Jupyter Notebook
