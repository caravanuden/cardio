# Parkinson's diagnosis

For the Dartmouth class COSC 89.20, Data Science for Health.

## Dataset

We're using the open-source Kaggle dataset [Tappy Keystroke Data with Parkinson's Patients](https://www.kaggle.com/valkling/tappy-keystroke-data-with-parkinsons-patients). This is the keystroke dataset for the study titled 'High-accuracy detection of early Parkinson's Disease using multiple characteristics of finger movement while typing'. This research paper is [published](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0188226#sec008) in PLOS ONE.

The dataset contains keystroke logs collected from over 200 subjects (103 PD subjects (32 with mild PD severity) and the remainder non-PD controls), with and without Parkinson's Disease (PD), as they typed normally on their own computer (without any supervision) over a period of weeks or months (having initially installed a custom keystroke recording app, Tappy). This dataset has been collected and analyzed in order to indicate that the routine interaction with computer keyboards can be used to detect changes in the characteristics of finger movement in the early stages of PD.

## Goal

Here, we will replicate the PLOS ONE study. We will extend their work by seeing which behavioral markers of PD are first present in early-stage (non-severe) PD and see how these behavioral markers change with increased severity of the disease. We will also potentially extend the previous ML models to implement  PD classification with a deep neural network (DNN). 
