# RISK ASSESSMENTS OF AIRPLANES 


# Overview
The Repo helps to advise our company in expanding in new industries to diversify its portfolio. 
This repo shows the relationship between airplanes make, mode, Injury Severity, number of engine, Engine Type and purpose of flight. 
The total fatal induries, total minor injuries and total serious injuries were also analysed and represented. 
The aim of the analysis is to identify the potential airplane with the lowest risk for the company to start this new business endeavor. 

# Business Problem


# The Data
The data analysed was extracted from Kaggle: 
https://moringa.instructure.com/courses/804/pages/phase-1-project-description?module_item_id=126432
The data had two sheets: 
	Aviation.csv
	US_state_code

# Questions to consider

1. Does the purpose of the fligt affect the safety score of the plane?
2. Is there a correlation between the safety score and the number of engine as well as the type of engine? 
3. Is there a relationship between make and model and the safety score? 

# Description of the data
import Pandas as pd ... for data analysis and manipulation.
import Numpy as np ... for mathematical functions especially when dealing with arrays.
import seaborn as sns ... for data visualization
import matplotlib.pyplot as plt ... for data visualization
%matplotlib inline ... allows for the automatic rendering of Matplotlib plots directly in the notebook rather than in a separate window.
Data Visualization in Tableau Public

# Loading the data
df = pd.read_csv ("AviationData.csv", encoding="ISO-8859-1")

US_state_code = pd.read_csv("USState_Codes.csv")


# Merging the datasets
df6 = df5.merge(US_state_code, on = "Abbreviation")

# Cleaning Data
cleaned_df = df6
cleaned_df.to_csv('cleaned_data.csv', index = False)


# Vivian-Muiruri-Phase-1
# Vivian-Muiruri-Phase-1
