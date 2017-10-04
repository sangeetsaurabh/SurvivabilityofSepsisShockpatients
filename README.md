# Survivability of patients diagnosed with Sepsis Shock

## Goal

For the patients who have been diagnosed with Sepsis/septic shock, goal of this project is to build a machine learning model that can predict survivability within 30 days of ICU admission. 

## Background 

Sepsis and severe sepsis (sepsis accompanied by acute organ dysfunction) are leading causes of death in the United States and the most common cause of death among critically ill patients in non-coronary intensive care units (ICU). Recent data suggest the annual cost of hospital care for patients with septicemia is $14 billion in United States. Also in the United States, the incidence of severe sepsis is estimated to be 300 cases per 100000 population. Approximately half of these cases occur outside the ICU. A fourth of patients who develop severe sepsis will die during their hospitalization. Septic shock is associated with the highest mortality, approaching 50%. The cumulative burden of organ failure is the strongest predictor of death, both in terms of the number of organs failing and the degree of organ dysfunction.Therefore, sepsis and severe sepsis are important public health problems. 

Although U.S. hospitals pay out over $22.2 billion annually for sepsis treatment, the disease still causes 20-45%  of death in hospitals. By the time the physical manifestations of sepsis start to appear, it’s sometimes too late to help the patient. Somewhere, buried in the data – in the blood values, the blood-pressure values, the heart rate, the temperature – is a prediction that this patient is heading toward an overwhelming infection and is likely to die. If we could predict that very early, it will make it less likely that the patient would die.

A predictive model that determines which patients are most vulnerable can really help ICUs focus their Physicians and staff on the most vulnerable patients. Potentially, such selective treatment can reduce mortality without increasing spending. This machine learning model is being designed to predict death within 30 days of ICU admission for the patients who have been diagnosed with Sepsis/septic shock.

## Solution Approach

The solution to is to categorize patients survivability at the time of admittance. This is calculated by considering: patient’s demographic, vitals and infection information. A supervised learning model will be trained off of this information along with the calculated target value(patient survival over 30 days from admittance).

The general strategy to solve this problem is to build a machine learning model using right set of features available within MIMIC-III database.

### What's included in this project?

1. **Survivability with severe Sepsis Shock - Data Preparation.ipynb :** This is the iPython notebook that reads data from postgres Mimic-III database and preapares the data such that it could be trained for machine learning model. Output of this notebook is a CSV file (Final_sepsis_feature_list.csv) that's used as input to machine learning models.

2. **Final_sepsis_feature_list.csv:** Output of Survivability with severe Sepsis Shock - Data Preparation.ipynb.

3. **Survivability with severe Sepsis Shock - Machine Learning Models.ipynb:** : This ipython notebook has the code to build machine learning models to predict surviability of patients diagonsed with Sepsis shock.

4. **visuals.py :** Python functions to do data visulation of Machine learning model results.

5. **Proposal for Survivability of ICU Patients with Severe Sepsis Shock project.pdf :** Proposal for the Project.

6. **Analysis of ML models for survivability of Sepsis patients.pdf :** Analysis of outcome of the projects.


### Other technical requirements

1. In order to run the iPython notebook, access to MIMIC-III database will be required. Detailed information about MIMIC-III database is available at https://mimic.physionet.org/ . 
2. In order to run Survivability with severe Sepsis Shock - Data Preparation.ipynb Notebook, MIMIC-III data is required on PostgreSQL database. Once a PostgreSQL database has MIMIC-III data, Notebook will need to be updated with database and user account information. 


