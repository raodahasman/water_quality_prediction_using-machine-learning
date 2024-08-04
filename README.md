![alt text](https://github.com/raodahasman/water_quality_prediction_using-machine-learning/blob/main/deployment/water.jpg?raw=true)
# Water Quality Analysis Using Machine Learning

## Tools

[<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />](https://pandas.pydata.org/)
[<img src="https://img.shields.io/badge/Seaborn-388E3C?style=for-the-badge&logo=seaborn&logoColor=white" alt="Seaborn" />](https://seaborn.pydata.org/)
[<img src="https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="Numpy" />](https://numpy.org/)
[<img src="https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib" />](https://matplotlib.org/)
[<img src="https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white" alt="SciPy" />](https://www.scipy.org/)
[<img src="https://img.shields.io/badge/Scikit%20learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-learn" />](https://scikit-learn.org/)
[<img src="https://img.shields.io/badge/XGBoost-016E54?style=for-the-badge&logo=xgboost&logoColor=white" alt="XGBoost" />](https://xgboost.ai/)

---

## Data Source

Kaggle: [Water Quality](https://www.kaggle.com/datasets/mssmartypants/water-quality).

## Introduction
Water is a valuable asset, and its availability affects many aspects of daily life, including agriculture, industry, and household needs. However, poor water quality can have detrimental effects, particularly by threatening public health and causing various diseases. By creating a project to predict whether water is safe or not, prevention measures can be taken to protect public health.
Objective: This project is created to enhance the model's ability to predict whether water is classified as safe or not, so that water can be used/ utilized according to the needs of the community.

## Conclusion
### Based on EDA:
In this exploration, it was found that the dataset consists of features containing information about the concentration of chemicals in the water. A simple check was also performed regarding the distribution of several features and their correlation with other features, and it was found that some features are not normally distributed. Since the dataset is imbalanced, meaning the distribution of classes (target) is not equal, with minority and majority classes present, the model may potentially be biased.

### Based on Model Evaluation:
- KNN: has a recall value of 0.355, indicating the model has limitations in identifying samples of water that are actually unsafe.
- SVM: has a recall value of 0.5, indicating the model has limitations in identifying samples of water that are actually unsafe.
- Decision Tree: has a high recall value of 0.8, indicating the model is effective in identifying water that is actually unsafe.
- Random Forest: has a recall value of 0.65. The performance of this model is quite good, although slightly below the performance of the Decision Tree model.
- XGBoost: has a recall value of 78.3%. This indicates that the XGBoost model also performs well in identifying water that is actually unsafe.

Based on model evaluation, modeling using the Decision Tree algorithm is the best model, with the ability to identify water that is actually unsafe at 80% and the model's accuracy in predicting whether water is safe or not at 95%.

The prediction results using the Decision Tree model provide valuable information for decision-making regarding water quality, thereby aiding in efforts to protect public health and safety.

## Model Development
- It is recommended to use optimal C parameter tuning.
- Because the data is imbalanced, perform techniques to balance the data, such as SMOTE.

## Deployment Model
hugging face : https://huggingface.co/spaces/raodahasman/Water_quality_prediction
