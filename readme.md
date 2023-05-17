# Syntactic Processing - Assignment

## Problem Statement

A health-Tech Company ‘BeHealthy’ aims to connect the medical communities with millions of patients across the country.

‘BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions.

‘BeHealthy’ provides medical services, prescriptions and online consultations and generating huge data day by day.

# Objective: 
You need to build a custom NER to get the list of diseases and their treatment from the dataset.


## Table of contents
Syntactic Processing - Assignment
Data preprocessing
Identifying Entities in Healthcare Data
Data Preprocessing
Construct the proper sentences from individual words and print the 5 sentences.
Count the number of sentences in the processed train and test dataset
Count the number of lines of labels in the processed train and test dataset.
Concept Identification
Extract those tokens which have NOUN or PROPN as their PoS tag and find their frequency
Print the top 25 most common tokens with NOUN or PROPN PoS tags
Defining features for CRF
Getting the features
Write a code/function to get the labels of a sentence
Define input and target variables
Define the labels as the target variable for test and the train dataset
Build the CRF Model
Evaluation
Identifying Diseases and Treatments using Custom NER
Predict the treatment for the disease name: 'hereditary retinoblastoma'




## library
# Import Basic libariries
import numpy as np
import pandas as pd
import struct
import array
import warnings
warnings.filterwarnings("ignore")
!pip install pycrf
!pip install sklearn-crfsuite
import spacy
import sklearn_crfsuite
from sklearn_crfsuite import metrics

--- 

# Result
Disease	Treatments
0	breast cancer	[undergone subcutaneous mastectomy and immedia...
1	ovarian cancer	[undergone subcutaneous mastectomy and immedia...
2	hereditary retinoblastoma	[radiotherapy]
3	unstable angina or non-q-wave myocardial infar...	[roxithromycin]
4	coronary-artery disease	[antichlamydial antibiotics]

# conclusion :

Treatments for 'hereditary retinoblastoma' is/are 'radiotherapy'


# Submitted by 
karan singh bisht