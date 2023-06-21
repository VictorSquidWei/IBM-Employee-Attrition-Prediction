# **IBM HR Analytics Attrition Dataset Analysis**

This repository contains code and analysis for the IBM HR Analytics Employee Attrition & Performance Dataset. 

## **Dataset**

- The dataset used in this project is `WA_Fn-UseC_-HR-Employee-Attrition.csv`
- It contains various features, including employee demographics, work-related factors, attrition indicators, and compensation details.
- The target variable is 'Attrition', indicating employee attrition (Yes/No).

## **Files**

- `IBMHRProject.ipynb`: Jupyter Notebook containing the code and analysis for the project.
- `WA_Fn-UseC_-HR-Employee-Attrition.csv`: Dataset file used in the analysis.

## **Addressing Class Imbalance**

Two methods were implemented to address the class imbalance:

- Undersampling of Majority Class: The majority class (No Employee Attrition) was undersampled to match the number of instances in the minority class (Employee Attrition).
- Class Weights: Higher weights were assigned to the minority class during model training.

## **Model Performance**

The project evaluated the performance of the decision tree classifiers under three different training approaches:

    Undersampling of Majority Class:
        Accuracy: 0.6020
        Precision: 0.24 (Class 0), 0.92 (Class 1)
        Recall: 0.71 (Class 0), 0.58 (Class 1)
        F1-Score: 0.35 (Class 0), 0.71 (Class 1)
        ROC AUC: 0.6467

    Class Weights:
        Accuracy: 0.7687
        Precision: 0.29 (Class 0), 0.88 (Class 1)
        Recall: 0.36 (Class 0), 0.84 (Class 1)
        F1-Score: 0.32 (Class 0), 0.86 (Class 1)
        ROC AUC: 0.5995

    Original Model (No Modification for Class Imbalance):
        Accuracy: 0.8027
        Precision: 0.37 (Class 0), 0.89 (Class 1)
        Recall: 0.42 (Class 0), 0.87 (Class 1)
        F1-Score: 0.40 (Class 0), 0.88 (Class 1)
        ROC AUC: 0.6469


## **Conclusion**

The analysis explored employee attrition prediction using the IBM HR Dataset. Class imbalance was addressed through undersampling of the majority class and assigning class weights. The performance evaluation revealed that the original model achieved the highest accuracy (0.8027). However, further improvements can be made to balance the precision and recall for both classes. Additional feature engineering or an ensemble models might enhance the model's performance.
