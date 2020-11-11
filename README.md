# Patient selection for diabetes drug testing

## Project Overview
This project was part of the path to finish Udacity´s nanodegree: "AI for Healthcare", in which skills acquired in the " Applying AI to EHR Data" course were applied to build a regression model that can support patient's selection for testing a new drug. 
The model was trained using a GPU for fast training of deep learning architecture, and access to a curated [dataset](https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008) that [has been modified for this course](https://github.com/udacity/nd320-c1-emr-data-starter/tree/master/project/data_schema_references). 


## Background
EHR data is becoming a key source of real-world evidence for the pharmaceutical industry and regulators to make decisions on clinical trials. 
This project proposes that a healthcare startup has created a groundbreaking diabetes drug ready for clinical trial testing. The drug needs to be administered over at least 5-7 days of time in the hospital with frequent monitoring/testing and patient medication adherence training with a mobile application. A patient dataset is available from a client partner and it is necessary to build a predictive model that can identify which type of patients the company should focus their efforts testing this drug on. Target patients are people that are likely to be in the hospital for this duration of time and will not incur significant additional costs for the study.
In order to achieve this goal, a regression model to predict the estimated hospitalization time for a patient is built, providing an uncertainty estimate range for that prediction to rank the predictions based off of the uncertainty range.

Expected Hospitalization Time Regression and Uncertainty Estimation Model: Utilizing a synthetic dataset (upsampled, denormalized, with line level augmentation) built off of the UCI Diabetes readmission dataset, students will build a regression model that predicts the expected days of hospitalization time and an uncertainty range estimation and then convert this to a binary prediction of whether to include or exclude that patient from the clinical trial.

This project will demonstrate the importance of building the right data representation at the encounter level, with appropriate filtering and preprocessing/feature engineering of key medical code sets. This project will also require students to analyze and interpret their model for biases across key demographic groups. Lastly, students will utilize the TF probability library to provide uncertainty range estimates in the regression output predictions to prioritize and triage prediction uncertainty levels.

In the end you will be creating a demographic bias analysis to detect if your model has any bias which we know can be a huge issue in working with healthcare data

Dataset
Due to healthcare PHI regulations (HIPAA, HITECH), there are limited number of publicly available datasets and some datasets require training and approval. So, for the purpose of this exercise, we are using a dataset from UC Irvine that has been modified for this course. Please note that it is limited in its representation of some key features such as diagnosis codes which are usually an unordered list in 835s/837s (the HL7 standard interchange formats used for claims and remits).

https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008 Data Schema The dataset reference information can be https://github.com/udacity/nd320-c1-emr-data-starter/tree/master/project/data_schema_references. There are two CSVs that provide more details on the fields and some of the mapped values.


## Project Highlight
This project includes the completion of the following steps:

* Data analysis
* Create categorical features with TensorFlow (TF) feature columns
* Create continuous/numerical features with TF feature columns
* Build deep learning regression model with sequential API and TF probability layers
* Evaluating potential model biases with Aequitas toolkit

## The Project at a glance


