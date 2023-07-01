# **IBM HR Analytics Attrition Dataset Analysis**

This repository contains code and analysis for the IBM HR Analytics Employee Attrition & Performance Dataset. 

## **Dataset**

- The dataset used in this project is `WA_Fn-UseC_-HR-Employee-Attrition.csv`
- It contains various features, including employee demographics, work-related factors, attrition indicators, and compensation details.
- The target variable is 'Attrition', indicating employee attrition (Yes/No).

## **Files**

- `IBMHRProject.ipynb`: Jupyter Notebook containing the code and analysis for the project.
- `WA_Fn-UseC_-HR-Employee-Attrition.csv`: Dataset file used in the analysis.

## **Models and Results**
Several models have been implemented and evaluated in this project. Here are the results of the model performances:

    Decision Tree Classifier (Baseline)
        Accuracy: 75.51%
        Precision (0): 23%
        Precision (1): 87%
        Recall (0): 28%
        Recall (1): 84%

    Class Weights
        Accuracy: 75.17%
        Precision (0): 22%
        Precision (1): 87%
        Recall (0): 28%
        Recall (1): 83%

    Balancing the Dataset
        Accuracy: 54.42%
        Precision (0): 16%
        Precision (1): 87%
        Recall (0): 51%
        Recall (1): 55%

    Bagging (with Grid Search)
        Accuracy: 85.37%
        Precision (0): 50%
        Precision (1): 87%
        Recall (0): 19%
        Recall (1): 97%

    Random Forest (with Grid Search)
        Accuracy: 86.05%
        Precision (0): 55%
        Precision (1): 89%
        Recall (0): 28%
        Recall (1): 96%

    Gradient Boosting (with Grid Search)
        Accuracy: 87.76%
        Precision (0): 71%
        Precision (1): 89%
        Recall (0): 28%
        Recall (1): 98%

## **Performance Evaluation**
The performance of the models is assessed based on accuracy, precision, recall, and F1-score. The classification reports and confusion matrices provide a comprehensive understanding of model performance for both 0s (no employee attrition) and 1s (employee attrition present). Additionally, ROC AUC is computed to evaluate the models' ability to discriminate between the two classes.

## **Usage**
To run the Jupyter Notebook file `IBMHRProject.ipynb`, it is recommended to use Google Colab due to resource-intensive computations involved in ensemble methods. Make sure to have the dataset file WA_Fn-UseC_-HR-Employee-Attrition.csv available in a working directory.

## **Conclusion**
In this project, we explored different machine learning techniques to predict employee attrition. The ensemble methods, such as Bagging, Random Forest, and Gradient Boosting, showed improved performance compared to the baseline decision tree model. By leveraging these techniques, we achieved higher accuracy and better prediction capabilities.

The results highlight the importance of considering class imbalance and utilizing ensemble methods to tackle this challenge. The Random Forest and Gradient Boosting models outperformed other approaches, demonstrating their ability to handle complex relationships within the dataset.

This project provides insights into employee attrition factors and offers predictive models that can assist HR departments in understanding and managing attrition risks. Further improvements and optimizations can be explored to enhance the models' performance and cater to specific organizational needs.

Please refer to the Jupyter Notebook file for a detailed implementation of the models, including data preprocessing, model training, hyperparameter tuning, and performance evaluation.
