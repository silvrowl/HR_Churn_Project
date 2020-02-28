
# Human Resources Churn Clustering and Classifier Project

A company wants to determine what is causing employees to leave the company, and what steps are need to increase retention. They have a dataset containing almost 15000 employees, 24% of which leave over the course of one year. The employees are from across all departments and all salary levels in the company

They have provided a semi-anonymized dataset containing 606 successful and 76 not successful loans along with their information and transactions. The goal here is to produce a model that can predict whether an employee will leave the company or not and determine what can be done to keep them. 

Overview of the results: [link](/Human_Resources_Retention.pdf)

## Prerequisites

All notebooks are written in Python 3. 

The libraries that are used in this notebook are listed under the `requirements.txt` file. One can simply issue to following command to insure the proper libraries are installed:

```bash
pip3 install -r requirements.txt
```

## Description of Analysis

The analysis consisted of feature creation of interaction variables and encoding of the ordinal and categorical variables. Agglomerative Clustering was used to group the employees into 3 groups, which split them on low, medium and high risk groups. AdaBoost Classifers were build for each of the risk groups to determine the most important factors in each risk group. Finally a test case was built to show how to adjust the most important factors for an individual to change them from leaving to staying at the company.

## Figures

#### Churn Analysis

![Employee Retention](/png_files/Employee_Retention_Distribution.png)


#### Cluster Groups

![Cluster Risk](/png_files/Cluster_Risk.png)

![Group Distribution](/png_files/Group_Distribution.png)


#### Shapely Values for Low Risk Group

![RF Shaply Values](/png_files/ada_shap_low.png)

#### Shapely Values for Medium Risk Group

![RF Shaply Values](/png_files/ada_shap_medium.png)

#### Shapely Values for High Risk Group

![RF Shaply Values](/png_files/ada_shap_high.png)
