## Credit Card Fraud Detection
## Problem Statement
high rate of false positives in their current system, which leads to unnecessary inconvenience for customers and additional workload for the fraud investigation team. 

## Project Overview
 implement a more accurate and efficient fraud detection model that can reduce false positives without compromising on the detection of actual fraud cases.

 ## Business Understanding
 A credit card company looking to improve its fraud detection system

## Components

* **Jupyter Notebook**
The [Jupyter Notebook](https://github.com/obystephen/dsc-phase-3-project-v2-3/blob/main/student.ipynb) is our key deliverable and contains details of our approach and methodology, data cleaning, exploratory data analysis and model building and validation.

I recommend using [nbviewer](https://nbviewer.jupyter.org/) to view the Jupyter Notebook.

* **Presentation**
The [presentation](https://) gives a high-level overview of our approach, findings and recommendations for non-technical stakeholders. It is aimed to be between 5 and 10 minutes long.

* **Data**

The dataset can be found in the file *"kc_house_data.csv"* in the Data folder, in this repository. It was originally provided in the following [repository](https://github.com/obystephen/dsc-phase-3-project-v2-3/blob/main/data/creditcard.csv). 

## Technologies/ Packages

* Python version: 3.6.9
* Matplotlib version: 3.1.3
* Seaborn version: 0.9.0
* Pandas version: 0.25.1
* Numpy version: 1.16.5
* Statsmodels version: 0.10.1
* Scikit-learn version: 0.21.2  

## To get started

1. Clone this repository - [guidance](https://help.github.com/articles/cloning-a-repository/).
2. Dataset can be found in the file "kc_house_data.csv".
3. Check requirements in Technologies section above and download libraries if necessary.

## Data Wrangling
Here we will work on data cleaning, handling missing values, data transformation, handling duplicates, data reshaping and other processes to ensure that we have a clean, structured, and suitable format for analysis and modeling

## Exploratory Data Analysis (EDA)
Here we will explore the different features of the dataset to gain a better understanding of the data. We will use data vizualization to uncover trends and patterns. We will use Feature Engineering to create new features from existing ones and perform One-Hot Encoding on categorical variables that we will require for analysis.

## Data Preprocessing
Here we determine our predictor and target variables. 
We split the data to train and test data.
Finally we scale our data.

## Modelling
We begin our modelling with a baseline model followed by an intermediate model and cap it off with a hyperparameter tuned complex model. The models will be evaluated based on their precision, accuracy, recall and F1 score. The modwel with the best metrics will be chosen for use and deployment.

# Model Results
### **Linear Regression Model**
##### Confusion Matrix:
[[56852     9]
 [   37    64]]
##### Accuracy:
 99.91924440855307
##### F1:
 0.7356321839080459
##### Precision:
 0.8767123287671232
##### Recall:
 0.6336633663366337

 ### **Random Forest**
##### Confusion Matrix:
 [[56854     7]
 [   22    79]]
##### Accuracy:
 99.94908886626172
##### F1:
 0.8449197860962566
##### Precision:
 0.9186046511627907
##### Recall:
 0.7821782178217822

 ### **Hyper Parameter Tuned Random Forest Model**
 ##### Confusion Matrix:
 
##### Accuracy:
 0.999420666409185
##### F1:
 0.8216216216216216
##### Precision:
 0.9047619047619048
##### Recall:
 0.7524752475247525
##### AUC:
 0.94

**RESULTS**
Using hyperparameter tuning, we positively impacted model performance. Suggesting that the tuning process and increased model complexity have resulted in a model that is better at distinguishing between legitimate and fraudulent transactions.
A higher F1 score indicates a better balance between precision and recall. This is desirable in fraud detection because it implies that the model is effective at both identifying fraudulent transactions and minimizing false positives. The complexity of the model, coupled with hyperparameter tuning, allows it to capture subtle patterns and relationships in the data, improving its discriminatory power.

## Conclusion
In conclusion, developing a robust credit card fraud detection model involves navigating through various challenges inherent to the dynamic and complex nature of financial transactions. The imbalanced distribution of fraudulent and legitimate transactions, the evolving tactics of fraudsters, and the need for interpretability and compliance present significant hurdles.

