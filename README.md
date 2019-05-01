# Cardiovascular disease diagnosis

For the Dartmouth class COSC 89.20, Data Science for Health. Project members are Srishti Bagchi, Rachael Chacko, and Cara Van Uden.

## Overview

Cardiovascular disease is the leading cause of death throughout the United States, with an estimated 840,768 deaths in 2016. However, through simple lifestyle changes and screening, nearly 200,000 deaths per year could be avoided. In this paper, we explore several machine learning approaches to detect the presence of cardiovascular disease using only standard health information. We leverage both traditional machine learning and state-of-the-art deep learning techniques. The machine learning techniques include a support vector machine (SVM) with a Gaussian RBF kernel, a Naive Bayes classifier, and a random forest (RF) classifier. For our deep learning technique, we also use a multilayer feedforward neural network for this cardiovascular disease detection.

In addition to using these methods to detect cardiovascular disease, we will also investigate which data features are most indicative of disease. Our dataset has standard health information and information on the presence/absence of cardiovascular disease for over 70,000 patients. Here, our objective is not only to design a classifier to identify the presence of cardiovascular disease but also to determine which features and types of data (demographic, examination, and social history) are most useful for predicting disease. With the information gained from this study, physicians could potentially alter their current case history methods to obtain more useful data from their patients. The results from this paper could also aid in streamlining the diagnostic process and improving diagnostic accuracy. 

Similar studies have also generated models to predict heart disease based off of more detailed examination data, such as that obtained from ECG, fluoroscopy, and myocardial scintigraphy. While these tests can provide detailed data, they can often be expensive to both patients and healthcare facilities and may not always be useful toward the diagnostic process. If we can demonstrate that our model can achieve a similar level of accuracy with data that can be obtained more quickly and easily than that from the typical medical exam (especially if this information could be instantaneously gathered via a mobile health device such as a FitBit), then this technology could streamline the diagnostic process and bring medicine to the home.

## Dataset

The cardiovascular disease dataset is an open-source [dataset](https://www.kaggle.com/sulianova/cardiovascular-disease-dataset) found on Kaggle. The data consists of 70,000 patient records (34,979 presenting with cardiovascular disease and 35,021 not presenting with cardiovascular disease) and contains 11 features (4 demographic, 4 examination, and 3 social history):

- Age (demographic)
- Height (demographic)
- Weight (demographic)
- Gender (demographic)
- Systolic blood pressure (examination)
- Diastolic blood pressure (examination)
- Cholesterol (examination)
- Glucose (examination)
- Smoking (social history)
- Alcohol intake (social history)
- Physical activity (social history)

Some features are numerical, others are assigned categorical codes, and others are binary values. The classes are balanced, but there were more female patients observed than male patients. Further, the continuous-valued features are almost normally distributed; however, most categorical-valued features are skewed towards "normal," as opposed to "high" levels of potentially pathological features. 

## TODONE
RF and SVM from EDA

## TODO

#### Paper

Expand related works:

https://ieeexplore.ieee.org/abstract/document/4358915/
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4468223/
https://link.springer.com/article/10.1007/s10916-016-0536-z
https://www.sciencedirect.com/science/article/pii/S093336571100056X

#### Code
- Predict on cardiovascular disease (target) based on original data (Rachael)
  - improving RF/SVM
  - trying DNN
  - Naive Bayes or odds ratio to get prob/risk score assigned to each class

- Predicting other target vars (BMI, blood pressure) in our dataset (Srishti)
  - Naive Bayes or odds ratio to get prob/risk score assigned to each class

- Combining with UCI dataset (Cara)
  - train to predict UCI blood sugar (bin), heart rate acheived during exercise (cont), exercise-induced angina (bin) with subset of our data
  - fill in our data with these vals using the trained model
  - see if this improves prediction

## References
