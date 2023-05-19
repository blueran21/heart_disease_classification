# Heart Disease Classification

## Contents:
- [Problem Statement](#Problem-Statement)
- [Data Cleaning](#Data-Cleaning)
- [Data Dictionary](#Data-Dictionary)
- [Data preprocessing](#Data-Preprocessing)
- [Model Building](#Model-Building)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)


## Problem Statement
The goal of this study is to develop classification models for heart disease prediction and inference that accurately identifies individuals at risk of developing the condition. We will utilize the CDC's BRFSS 2021 dataset to do our research. We plan to optimize for balanced accuracy and choose the model with high recall so that means those who are sick are identified as often as possible. Leveraging relevant health and demographic data, the model will assist healthcare professionals in targeting preventive measures, enhancing patient outcomes, and reducing the overall burden of heart disease on the healthcare system.


## Data Cleaning
First, we need to use domain knowledge to identify and remove any irrelevant or redundant columns from the dataset. We also eliminate columns that have an excess of missing data. Observations without a target label are discarded, as are rows with a high count of missing values. Next, we reference the Dataset Dictionary to handle missing values appropriately. Our data is represented by numbers, which means we need to convert some column values to their corresponding category names, following the code book. For categorical variables, if a missing value is actually indicating a distinct category such as 'Not Sure' or 'Not Asked', rather than being truly missing, we replace it accordingly and mark truly missing values as 'missing'. Similarly, for numerical variables, we label and assign values based on the code book's guidelines, and impute any remaining missing values with the median.


## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**_michd**|object|cleaning_data_phase2.csv|If have heart disease or not|
|**_state**|object|cleaning_data_phase2.csv|State of U.S.|
|**_sex**|object|cleaning_data_phase2.csv|Calculated sex variable|
|**genhlth**|object|cleaning_data_phase2.csv|General Health|
|**physhlth**|float64|cleaning_data_phase2.csv|Number of Days Physical Health Not Good|
|**menthlth**|float64|cleaning_data_phase2.csv|Number of Days Mental Health Not Good|
|**addepev3**|object|cleaning_data_phase2.csv|(Ever told) you had a depressive disorder|
|**checkup1**|object|cleaning_data_phase2.csv|Length of time since last routine checkup|
|**_totinda**|object|cleaning_data_phase2.csv|Adults who reported doing physical activity or exercise during the past 30 days other than their regular job|
|**_rfhype6**|object|cleaning_data_phase2.csv|Adults who have been told they have high blood pressure by a doctor, nurse, or other health professional|
|**cholmed3**|object|cleaning_data_phase2.csv|Currently taking medicine for high cholesterol|
|**_rfchol3**|object|cleaning_data_phase2.csv|High Cholesterol Calculated Variable|
|**cvdstrk3**|object|cleaning_data_phase2.csv|Ever Diagnosed with a Stroke|
|**_asthms1**|object|cleaning_data_phase2.csv|Computed asthma status|
|**chcscncr**|object|cleaning_data_phase2.csv|(Ever told) you had skin cancer|
|**chcocncr**|object|cleaning_data_phase2.csv|(Ever told) you had any other types of cancer|
|**chccopd3**|object|cleaning_data_phase2.csv|Ever told you had C.O.P.D. emphysema or chronic bronchitis|
|**chckdny2**|object|cleaning_data_phase2.csv|Ever told you have kidney disease|
|**diabete4**|object|cleaning_data_phase2.csv|(Ever told) you had diabetes|
|**_drdxar3**|object|cleaning_data_phase2.csv|Respondents diagnosed with arthritis|
|**marital**|object|cleaning_data_phase2.csv|Marital Status|
|**children**|float64|cleaning_data_phase2.csv|Number of Children in Household|
|**_incomg1**|object|cleaning_data_phase2.csv|Computed income categories|
|**employ1**|object|cleaning_data_phase2.csv|Employment Status|
|**htm4**|float64|cleaning_data_phase2.csv|Computed Height in Meters|
|**wtkg3**|float64|cleaning_data_phase2.csv|Computed Weight in Kilograms|
|**_bmi5**|float64|cleaning_data_phase2.csv|Computed body mass index|
|**decide**|object|cleaning_data_phase2.csv|Difficulty Concentrating or Remembering|
|**diffwalk**|object|cleaning_data_phase2.csv|Difficulty Walking or Climbing Stairs|
|**diffdres**|object|cleaning_data_phase2.csv|Difficulty Dressing or Bathing|
|**_smoker3**|object|cleaning_data_phase2.csv|Four-level smoker status: Everyday smoker, Someday smoker, Former smoker, Non-smoker|
|**usenow3**|object|cleaning_data_phase2.csv|Frequency of using chewing tobacco|
|**ecignow1**|object|cleaning_data_phase2.csv|Do you now use e-cigarettes, every day, some days, or not at all|
|**_drnkwk1**|float64|cleaning_data_phase2.csv|Calculated total number of alcoholic beverages consumed per week|
|**_metstat**|object|cleaning_data_phase2.csv|Metropolitan Status|
|**_imprace**|object|cleaning_data_phase2.csv|Imputed race/ethnicity value (If no response, imputed with most common race for that region)|
|**_age80**|float64|cleaning_data_phase2.csv|Imputed Age value collapsed above 80|
|**_educag**|object|cleaning_data_phase2.csv|Level of education completed|
|**ftjuda2_**|float64|cleaning_data_phase2.csv|Computed Fruit Juice intake in times per day|
|**frutda2_**|float64|cleaning_data_phase2.csv|Computed Fruit intake in times per day|
|**grenda1_**|float64|cleaning_data_phase2.csv|Computed Dark Green Vegetable intake in times per day|
|**frnchda_**|float64|cleaning_data_phase2.csv|Computed French Fry intake in times per day|
|**potada1_**|float64|cleaning_data_phase2.csv|Computed Potato Servings per day|
|**vegeda2_**|float64|cleaning_data_phase2.csv|Computed Other Vegetable intake in times per day|


## Data Preprocessing
For the categorical columns, we applied one-hot encoding to transform them into a format for different classification models. Additionally, we utilized standard scaling to scale the whole data, ensuring that all features are on a similar scale. With these preprocessing steps, the dataset is now optimally prepared for building models.


## Model Building
...


## Conclusions and Recommendations
...
