## Overview



## Problem



## Datasets
### MIMIC-IV

### eICU

### Outcomes
  - 60-Day Readmission or In-Hospital Death
  - 48-Hour Readmission or In-Hospital Death (with observability requirement)

### Features
  - Latest value
  - Change over stay



## Modeling



## Results
Table 1: Results from training and predicting outcomes using the MIMIC-IV dataset on two different outcomes: (1) ICU readmission or in-hospital death within 60 days of ICU discharge, and (2) ICU readmission or in-hospital death within 48 hours of ICU discharge among patients remaining in the hospital (i.e. discharged from the ICU to the floor or other stepdown unit). 

| Model               |  Outcome 1: 60 Days (AUC) | Outcome 2: 48 Hours (AUC)|
| :---------------    | :---------------          | :---------------     |
| Logistic Regression | 67.8                      | 84.0 |
| Decision Tree       | 66.0                      | 83.9 |
| XGBoost             | 73.1                      | 91.8 |

Table 2: Results from training and predicting outcomes using the eICU dataset on outcome 2: ICU readmission or in-hospital death within 48 hours of ICU discharge among patients remaining in the hospital (i.e. discharged from the ICU to the floor or other stepdown unit). 

| Model               |  Outcome 2: 48 Hours (AUC)|
| :--------------     | :---------------          | 
| Logistic Regression | 87.7 |
| Decision Tree       | 87.2 |
| XGBoost             | 94.4 |

Table 3: Results from training using the MIMIC dataset and predicting outcomes using the eICU dataset on outcome 2: ICU readmission or in-hospital death within 48 hours of ICU discharge among patients remaining in the hospital (i.e. discharged from the ICU to the floor or other stepdown unit). 

| Model               |  Outcome 2: 48 Hours (AUC)|
| :--------------     | :---------------          | 
| Logistic Regression | 77.6 |
| Decision Tree       | 80.5 |
| XGBoost             | 85.0 |

### Interpretability
Figure 1: Coefficient weights from the logistic regression model trained on MIMIC data to predict the 48-hour outcome.
![Logistic Regression - MIMIC - 48-hour Outcome](logreg.png)

Figure 2: Decision tree plot showing top three levels of tree trained on MIMIC data to predict the 48-hour outcome.
![Decision Tree - MIMIC - 48-hour Outcome](dec_tree.png)

Figure 3: Summary of Shapley values for the XGBoost model trained on MIMIC data to predict the 48-hour outcome.
![XGBoost - MIMIC - 48-hour Outcome](shap.png)

## Discussion

## Supporting Slides
Note: the slide deck is only accessible to those logged in to Google with a UC Berkeley account.

<https://docs.google.com/presentation/d/1zNuIRwdBwT33wzVQZBsBXjrRoxMhzQjeOeQEm_L4jbY/edit>

## Citations
1. Johnson, A., Bulgarelli, L., Pollard, T., Horng, S., Celi, L. A., & Mark, R. (2021). MIMIC-IV (version 1.0). PhysioNet. https://doi.org/10.13026/s6n6-xd98.
2. Pollard, T., Johnson, A., Raffa, J., Celi, L. A., Badawi, O., & Mark, R. (2019). eICU Collaborative Research Database (version 2.0). PhysioNet. https://doi.org/10.13026/C2WM1R.

## About Us
This website is the final deliverable for our capstone project as part of the course W210: Synthetic Capstone in the UC Berkeley Master of Information and Data Science (MIDS) program. We took the course in the spring term of 2022 with Puya Vahabi and Alberto Todeschini. More information about us is below.

Dahler Battle

![Dahler](dahler.jpeg)

<https://www.linkedin.com/in/dahlerbattle/>
<https://github.com/dahlerbattle>


Mohamed Gesalla

![Mohamed](mohamed.jpg)

<https://www.linkedin.com/in/mohamed-gesalla/>
<https://github.com/mgesalla>


Natasha Flowers
![Natasha](nflowers.jpg)

<https://www.linkedin.com/in/natasha-a-flowers/>
<https://github.com/natasha-flowers>






