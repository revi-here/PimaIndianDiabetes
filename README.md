# PimaIndianDiabetes  

<b> by Revathy Thiyagarajan  

# Introduction.  

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases.  
The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic  
measurements included in the dataset. Several constraints were placed on the selection of these instances from a larger  
database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.  

![Diabetes](images/intro.jpg 'Diabetes')  

# Goals  
1.Look for any correlation between different variables.  
2.Study the trend of the variables for different age group.  
3.Conclusion based on influence of the variables on the Outcome variable.   

*** 
## Resources  
1.Data Source  : UCI Machine Learning — Repository:https://www.kaggle.com/uciml/pima-indians-diabetes-database   
2.Data analysis : Pandas, Numpy   
3.Visualisation : Matplotlib, Pyplot, Seaborn   
  
***
# Exploratory Data Analysis.  

## 1.Visualization of the different features.  
 
![Features](images/distplot.png 'Features')  
***Conclusion***  
From the above plots, we see that there are 0 in some fields which are impossible to occur like BloodPressure, Glucose, Insulin.  
1.Insulin and SkinThickness have around 200-300 data with 0. We replace the 0 with average of the fields respectively.  
2.Glucose and BMI have way few(less than 10%) with ).So we ignore them in the data .  

## Correlation matrix  
### Correlation between different features/variables.   
![Correlation](images/heatmap.png 'Correlation')     
From the above heatmap, we don't see much correlation between the variables.  
The maximum correlation we see is only 0.5 - 0.6.   
Better correlation between Glucose, Insulin and glucose, outcome.  
This clearly shows that value of Glucose has some influence on the Outcome variable.  

## Diabetic Count across different age groups.  
![Diabetic Count](images/diabetic_count.png 'Diabetic Count')   

## Average measures across different age groups.   
![Average measures](images/average_agegroup.png 'Average measures')   
<b>BMI, BloodPressure, Glucose and all other variables except Insulin seems to be consistent with age.  
Insulin apike  is clearly visible with the age group 51-60.  
</b>

# Final Conclusion.   
<b>Based on our analysis, we see that  
 <b>1.BMI, BloodPressure, Glucose and all other variables except Insulin seems to be consistent with age.    
    2.Insulin apike is clearly visible with the age group 51-60.    
    3.Women in the age group 30-50 have higher count of diabetics.  
    4.Young women in the age 21-30 has a low percentage(less than 30%) of diabetics dignosis.  
    5.Women over the age 70 cannot be analyzed because of almost no supporting data.(only 1 available).  
    6.we don't see much correlation between the variables from the heatmap created from correlation matrix.  
    7.The maximum correlation is 0.5 - 0.6.  
    8.Better correlation between Glucose, Insulin and glucose, outcome.This clearly shows that value of Glucose has some             influence on the Outcome variable.
    </b>
