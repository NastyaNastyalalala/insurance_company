# 🚀 Car Insurance - binary classification

This repository contains research for binary classification use case.

Task: you need to understand whether the client will be interested in insurance. Thus, the insurance company can target advertising more optimally and build communication with customers, increasing conversion.

## DATA Review
| Field name | Overview |
| ------ | ------ |
| Gender | Male/Female |
| Age | Age |
| Driving_License | Availability of a driver's license |
| Region_Code | Region of residence |
| Previously_Insured | Have you used the services of an insurance company before? |
| Vehicle_Age | Vehicle age |
| Vehicle_Damage | Whether the vehicle was involved in an accident |
| Annual_Premium | Client’s annual payments  |
| Policy_Sales_Channel | Policy for the distribution of insurance services |
| Vintage | Number of days during which the client was associated with the company |
| Response | interested in insurance 1, did not respond 0 |

## Brief Overview of the Files:
### 1. requirements.txt
Before running code locally please install dependancies from requirements.txt

### 2. research/insurance_company.ipynb
Main research file

### Metrics: F-1 score

### Results:
1. EDA(distributions of some columns, correlation matrix)
2. Processing categorical features(it was necessary only for models that do not know how to process categorical features)
3. Trained different models
	- GradientBoostingClassifier(plot curves for the f1-score metric depending on the number of steps for several learning_rates and find the best parameters)
	- RandomForestClassifier(deep and non-deep trees were trained)
	- CatBoostClassifier
	- LGBMClassifier
	- KNeighborsClassifier (accelerated the model due to preliminary clustering)
4. Feature importances (for different models, different features turned out to be more important)


As a result, CatBoostClassifier model turned out to be the best for this task




