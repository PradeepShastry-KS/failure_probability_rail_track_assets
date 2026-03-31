# Data-Driven Failure Probability of Rail Track Assets



## Overview

This project focuses on predicting the probability of failure in rail track assets using machine learning.
The objective is to support predictive maintenance and risk based decision-making by identifying high risk track segments using historical condition and defect data.


## Data

The analysis uses two primary datasets:

- Rail wear data  
- Geometric defects data  

Data preprocessing included:

- Cleaning and standardising features  
- Handling missing values  
- Merging datasets on track location  
- Feature engineering based on wear thresholds and defect severity  

## Methodology

- Data preprocessing and feature engineering  
- Train-test split and feature scaling  
- Handling class imbalance using SMOTE  

### Models Used
- Logistic Regression   
- XGBoost   

## Evaluation Metrics
- Accuracy  
- ROC-AUC  
- F1-score  
- Precision-Recall AUC  

## Results
### Logistic Regression
- Test Accuracy: 0.9805  
- ROC-AUC: 0.9805  
- PR-AUC: 0.9371  
### XGBoost
- ROC-AUC: 0.9983  
- PR-AUC: 0.9930  
- F1-score (failure class): 0.95  

## Key Findings
- XGBoost significantly outperformed Logistic Regression, particularly in detecting failure cases  
- Rail wear and geometric defects are strong predictors of failure  
- High risk segments are strongly associated with curved track sections  

## Practical Application
The predicted failure probabilities can be integrated into a risk-based framework (e.g., FMEA) by mapping probabilities to occurrence scores.

This enables:

- Prioritisation of high risk track segments  
- Improved maintenance planning  
- Reduction in unexpected failures and delays  

## Project Structure


```text
Probability\_of\_failure\_for\_Rail\_track\_assets/

├── Notebook/

│ └── Failure\_Probability\_Model\_RW\_GD.ipynb

├── Report/

│ └── Probability\_of\_Failure\_for\_Rail\_Track\_Assets\_Report.pdf

├── requirements.txt

└── README.md
```

## Setup:

Install Dependencies:
```bash

pip install -r requirements.txt
```

## How to Run

* Navigate to the ```Notebook folder```
* Open Notebook: 
```Failure\_Probability\_Model\_RW\_GD.ipynb```
* Run: 
```Failure\_Probability\_Model\_RW\_GD.ipynb```



