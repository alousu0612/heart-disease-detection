## Heart Disease Detection based on heart-disease-uci data

### Data

 + https://www.kaggle.com/ronitf/heart-disease-uci
 
### Context

This database contains 76 attributes, but all published experiments refer to using a subset of 14 of them. In particular, the Cleveland database is the only one that has been used by ML researchers to
this date. The "goal" field refers to the presence of heart disease in the patient. It is integer valued from 0 (no presence) to 4.

### Content

Attribute Information:

+ age
+ sex
+ chest pain type (4 values)
+ resting blood pressure
+ serum cholestoral in mg/dl
+ fasting blood sugar > 120 mg/dl
+ resting electrocardiographic results (values 0,1,2)
+ maximum heart rate achieved
+ exercise induced angina
+ oldpeak = ST depression induced by exercise relative to rest
+ the slope of the peak exercise ST segment
+ number of major vessels (0-3) colored by flourosopy
+ thallium defect

The names and social security numbers of the patients were recently removed from the database, replaced with dummy values. One file has been "processed", that one containing the Cleveland database. All four unprocessed files also exist in this directory.

### Errors

+ cp: chest pain type
 
 -- Value 0: asymptomatic 
 
 -- Value 1: atypical angina 
 
 -- Value 2: non-anginal pain 
 
 -- Value 3: typical angina

restecg: resting electrocardiographic results -- Value 0: showing probable or definite left ventricular hypertrophy by Estes' criteria -- Value 1: normal -- Value 2: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)

slope: the slope of the peak exercise ST segment 0: downsloping; 1: flat; 2: upsloping

thal: 1 = fixed defect; 2 = normal; 7 = reversable defect

target (maybe THE most important feature): 0 = disease, 1 = no disease

A few more things to consider: data #93, 139, 164, 165 and 252 have ca=4 which is incorrect. In the original Cleveland dataset they are NaNs (so they should be removed) data #49 and 282 have thal = 0, also incorrect. They are also NaNs in the original dataset.

