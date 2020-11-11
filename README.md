# Patient selection for diabetes drug testing

## Project Overview
This project was part of the path to finish Udacity´s nanodegree: "AI for Healthcare", in which skills acquired in the " Applying AI to EHR Data" course were applied to build a regression model that can support patient's selection for testing a new drug. 
The model was trained using a GPU for fast training of deep learning architecture, and access to a curated [dataset](https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008) that [has been modified for this course](https://github.com/udacity/nd320-c1-emr-data-starter/tree/master/project/data_schema_references). 


## Background
EHR data is becoming a key source of real-world evidence for the pharmaceutical industry and regulators to make decisions on clinical trials. 
This project proposes that a healthcare startup has created a groundbreaking diabetes drug ready for clinical trial testing. The drug needs to be administered over at least 5-7 days of time in the hospital with frequent monitoring/testing and patient medication adherence training with a mobile application. From an available patient dataset, it is necessary to build a predictive model that can identify which type of patients the company should focus their efforts testing this drug on. Target patients are people that are likely to be in the hospital for this duration of time and will not incur in significant additional costs for the study.
In order to achieve this goal, a regression model to predict the estimated hospitalization time for a patient is built, providing an uncertainty estimate range for that prediction to rank the predictions based off of the uncertainty range.

## Project Highlight
This project includes the completion of the following steps:

* Data analysis
* Create categorical features with TensorFlow (TF) feature columns
* Create continuous/numerical features with TF feature columns
* Build deep learning regression model with sequential API and TF probability layers
* Evaluating potential model biases with Aequitas toolkit

## The Project at a glance
This project is frame in three complementary files: one main code structure (Project) and two supporting files (utils and student_utils). 

The main structure is divided in: 
* Project description 
* Project objectives
* Data preparation, which involves the loading of the dataset, the determination of the dataset level (line or encounter), an exploratory data analysis (EDA), feature selection, splitting the dataset into train, validation and test partitions, demographic representation analysis of the split, the convertion of the dataset splits into TF dataset, among other relevant steps.

![EDA_1](https://github.com/franciscoj-londonoh/Patient-Selection-for-Diabetes-Drug-Testing/blob/main/Images/EHR_data1.png)

* Building vocabulary and creating categorical features with TensorFlow (TF) feature column API
* Continuous/numerical features creation with TF feature columns
* Deep learning regression model building with sequential API and TF probability layers, model prediction, uncertainty and evaluation metrics
* Evaluating potential model biases with Aequitas toolkit, such as race and gender bias analysis for patient selection and Fairness analysis relative to a reference group 
