# Laptop Price Prediction

This project develops a machine learning model to predict laptop prices based on various features such as company, product type, operating system, CPU, GPU, memory, screen resolution, weight, etc.

## Dataset

The dataset used in this project can be obtained from Kaggle. It is available at the following link: [Laptop Price Dataset on Kaggle](https://www.kaggle.com/code/nehahatti/laptop-price-prediction)


This dataset includes information about laptops including features and their corresponding prices.

## Data Preprocessing

1. **Dataset Loading**: The dataset is loaded into a pandas DataFrame.

2. **Feature Engineering**: 
    - Unnecessary columns are dropped.
    - Categorical variables are one-hot encoded.
    - Some binary variables are converted to numerical values.
    
3. **Visualization**: 
    - Relationships between features are visualized with heatmaps.
    - Feature correlations are examined for feature selection, and features with low correlations are dropped.

## Model Development

1. **Dataset Splitting**: The dataset is split into training and test sets to evaluate the model's performance.

2. **Model Creation and Training**: 
    - A Random Forest regressor is created and initially trained with default parameters.

3. **Hyperparameter Optimization**: 
    - Hyperparameter optimization is performed using GridSearchCV to find the best parameters for the Random Forest regressor.

4. **Model Evaluation**: 
    - A new model is created with the best parameters found during hyperparameter optimization, and the model's performance is evaluated on the test set.


## Requirements

- Python 3.x
- pandas
- scikit-learn
- seaborn
- matplotlib

