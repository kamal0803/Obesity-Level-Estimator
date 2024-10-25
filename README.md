# Estimation of Obesity Levels Based on Eating Habits and Physical Condition

Developed machine learning models to estimate the obesity levels of humans based on eating habits and physical condition.

## Data
For each individual, below are the features -

- `Gender` - individual's gender (binary: 'Male' or 'Female')
- `Age` - individuals's age (numeric: from 14 to 61)
- `Height` - individual's height (numeric: 1.45 to 1.98)
- `Weight` - individual's height (numeric: 39 to 173)
- `family_history_with_overweight` - Has a family member suffered or suffers from overweight? (binary: 'yes' or 'no')
- `FAVC` - Do you eat high caloric food frequently? (binary: 'yes' or 'no')
- `FCVC` - Do you usually eat vegetables in your meals? (numeric: 1 to 3)
- `NCP` - How many main meals do you have daily? (numeric: 1 to 4)
- `CAEC` - Do you eat any food between meals? (categorical: 'no', 'Sometimes', 'Always', 'Frequently')
- `SMOKE` - Do you smoke? (binary: 'yes' or 'no')
- `CH2O` - How much water do you drink daily? (numeric: 1 to 3)
- `SCC` - Do you monitor the calories you eat daily? (binary: 'yes' or 'no')
- `FAF` - How often do you have physical activity? (numeric: 0 to 3)
- `TUE` - How much time do you use technological devices such as cell phone, videogames, television, computer and others? (numeric: 0 to 2)
- `CALC` - How often do you drink alcohol? (categorical: 'no', 'Sometimes')
- `MTRANS` - Which transportation do you usually use? (categorical: 'Walking', 'Public_Transportation', 'Motorbike', 'Bike', 'Automobile')
- `NObeyesdad` - Obesity level (categorical: 'Insufficient_Weight', 'Normal_Weight', 'Overweight_Level_I', 'Overweight_Level_II', 'Obesity_Type_I', 'Obesity_Type_II', 'Obesity_Type_III')

## Approach
Various factors such as eating habits, physical conditions, alcohol consumption, smoking, water intake were correlated with obesity levels in terms of visuals, which helped to drill down to the factors contributing to obesity. To build a model to estimate obesity levels, various pre-processing steps were done using OrdinalEncoder & OneHotEncoder, and duplicates were removed too. **Random Forest Classifier**, **Decision Tree Classifier** and **XGBoost Classifier** were used.

Out of 2111 data points, 80% was considered for training & remaining 20% for testing.

## Results & Conclusion
The XGBoost Classifier & Random Forest Classifier performed the best in terms of testing accuracy of about 85% and training accuracy of 97%.

## Acknowledgements

Data for building the model was taken from below - 
https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition
