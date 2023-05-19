# Heart Disease Classification

## Contents:
- [Problem Statement](#Problem-Statement)
- [Data Cleaning](#Data-Cleaning)
- [Data Dictionary](#Data-Dictionary)
- [Data preprocessing](#Data-Preprocessing)
- [Model Building](#Model-Building)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)


## Problem Statement
The goal of this study is to develop classification models for heart disease prediction and inference that accurately identifies individuals at risk of developing the condition. We will utilize the CDC's BRFSS 2021 dataset to do our research. We plan to optimize for balanced accuracy and recall so that the true positive rate is high, meaning those who are sick are identified as often as possible. Leveraging relevant health and demographic data, the model will assist healthcare professionals in targeting preventive measures, enhancing patient outcomes, and reducing the overall burden of heart disease on the healthcare system.


## Data Cleaning
First, we need to use domain knowledge to identify and remove any irrelevant or redundant columns from the dataset. Then, consult the Dataset Dictionary to properly handle missing values. If a missing value represents a specific category such as 'Not Sure' or 'Missing', rather than being truly missing, replace it accordingly.
...


## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**_michd**|object|2021_heart_cleaned.csv|If have heart disease or not|
|**_state**|object|2021_heart_cleaned.csv|State of U.S.|
|**_sex**|object|2021_heart_cleaned.csv|Calculated sex variable|
|**genhlth**|object|2021_heart_cleaned.csv|General Health|
|**physhlth**|float64|2021_heart_cleaned.csv|Number of Days Physical Health Not Good|
|**menthlth**|float64|2021_heart_cleaned.csv|Number of Days Mental Health Not Good|
|**addepev3**|object|2021_heart_cleaned.csv|(Ever told) you had a depressive disorder|
|**checkup1**|object|2021_heart_cleaned.csv|Length of time since last routine checkup|
|**_totinda**|object|2021_heart_cleaned.csv|Adults who reported doing physical activity or exercise during the past 30 days other than their regular job|
|**_rfhype6**|object|2021_heart_cleaned.csv|Adults who have been told they have high blood pressure by a doctor, nurse, or other health professional|
|**cholmed3**|object|2021_heart_cleaned.csv|Currently taking medicine for high cholesterol|
|**_rfchol3**|object|2021_heart_cleaned.csv|High Cholesterol Calculated Variable|
|**cvdstrk3**|object|2021_heart_cleaned.csv|Ever Diagnosed with a Stroke|
|**_asthms1**|object|2021_heart_cleaned.csv|Computed asthma status|
|**chcscncr**|object|2021_heart_cleaned.csv|(Ever told) you had skin cancer|
|**chcocncr**|object|2021_heart_cleaned.csv|(Ever told) you had any other types of cancer|
|**chccopd3**|object|2021_heart_cleaned.csv|Ever told you had C.O.P.D. emphysema or chronic bronchitis|
|**chckdny2**|object|2021_heart_cleaned.csv|Ever told you have kidney disease|
|**diabete4**|object|2021_heart_cleaned.csv|(Ever told) you had diabetes|
|**_drdxar3**|object|2021_heart_cleaned.csv|Respondents diagnosed with arthritis|
|**marital**|object|2021_heart_cleaned.csv|Marital Status|
|**children**|float64|2021_heart_cleaned.csv|Number of Children in Household|
|**_incomg1**|object|2021_heart_cleaned.csv|Computed income categories|
|**employ1**|object|2021_heart_cleaned.csv|Employment Status|
|**htm4**|float64|2021_heart_cleaned.csv|Computed Height in Meters|
|**wtkg3**|float64|2021_heart_cleaned.csv|Computed Weight in Kilograms|
|**_bmi5**|float64|2021_heart_cleaned.csv|Computed body mass index|
|**decide**|object|2021_heart_cleaned.csv|Difficulty Concentrating or Remembering|
|**diffwalk**|object|2021_heart_cleaned.csv|Difficulty Walking or Climbing Stairs|
|**diffdres**|object|2021_heart_cleaned.csv|Difficulty Dressing or Bathing|
|**_smoker3**|object|2021_heart_cleaned.csv|Four-level smoker status: Everyday smoker, Someday smoker, Former smoker, Non-smoker|
|**usenow3**|object|2021_heart_cleaned.csv|Frequency of using chewing tobacco|
|**ecignow1**|object|2021_heart_cleaned.csv|Do you now use e-cigarettes, every day, some days, or not at all|
|**_drnkwk1**|float64|2021_heart_cleaned.csv|Calculated total number of alcoholic beverages consumed per week|
|**_metstat**|object|2021_heart_cleaned.csv|Metropolitan Status|
|**_imprace**|object|2021_heart_cleaned.csv|Imputed race/ethnicity value (If no response, imputed with most common race for that region)|
|**_age80**|float64|2021_heart_cleaned.csv|Imputed Age value collapsed above 80|
|**_educag**|object|2021_heart_cleaned.csv|Level of education completed|
|**ftjuda2_**|float64|2021_heart_cleaned.csv|Computed Fruit Juice intake in times per day|
|**frutda2_**|float64|2021_heart_cleaned.csv|Computed Fruit intake in times per day|
|**grenda1_**|float64|2021_heart_cleaned.csv|Computed Dark Green Vegetable intake in times per day|
|**frnchda_**|float64|2021_heart_cleaned.csv|Computed French Fry intake in times per day|
|**potada1_**|float64|2021_heart_cleaned.csv|Computed Potato Servings per day|
|**vegeda2_**|float64|2021_heart_cleaned.csv|Computed Other Vegetable intake in times per day|


## Data Preprocessing
For the categorical columns, we applied one-hot encoding to transform them into a format for different classification models. Additionally, we utilized standard scaling to scale the data, ensuring that all features are on a similar scale. With these preprocessing steps, the dataset is now optimally prepared for building models.
...


## Model Building
...


## Conclusions and Recommendations
...
