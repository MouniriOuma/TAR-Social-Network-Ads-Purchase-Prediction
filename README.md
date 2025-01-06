# Social Network Ads Purchase Prediction

This project demonstrates a machine learning workflow for predicting whether a user will purchase a product based on their gender, age, and estimated salary. The dataset used is a synthetic dataset from a social network advertising campaign. The model used is logistic regression, and the workflow includes data preprocessing, feature scaling, model training, evaluation, and visualization.


## Project Overview

The goal of this project is to build a logistic regression model to predict whether a user will purchase a product based on the following features:
- **Gender**: The gender of the user (encoded as `Male = 1`, `Female = 0`).
- **Age**: The age of the user.
- **EstimatedSalary**: The estimated salary of the user.

The target variable is:
- **Purchased**: Whether the user purchased the product (`1` for purchased, `0` for not purchased).

The workflow includes:
- Loading and preprocessing the dataset.
- Encoding categorical variables.
- Splitting the data into training and testing sets.
- Scaling the features using `StandardScaler`.
- Training a logistic regression model.
- Evaluating the model's performance using accuracy, classification report, and confusion matrix.
- Visualizing the confusion matrix using a heatmap.


## Code Explanation

The code is structured as follows:

1. **Import Libraries**:
   - Libraries like `numpy`, `pandas`, `matplotlib`, and `seaborn` are imported for data manipulation and visualization.
   - Scikit-learn modules are imported for machine learning tasks.

2. **Load and Inspect the Dataset**:
   - The dataset is loaded from a CSV file (`Social_Network.csv`).
   - The dataset is inspected to ensure all required columns are present.

3. **Handle Missing Values**:
   - Rows with missing values are removed.

4. **Encode Categorical Data**:
   - The `Gender` column is encoded into numerical values (`Male = 1`, `Female = 0`).

5. **Prepare Features and Target**:
   - Features (`Gender`, `Age`, `EstimatedSalary`) and the target (`Purchased`) are extracted.

6. **Split the Data**:
   - The dataset is split into training and testing sets using `train_test_split`.

7. **Feature Scaling**:
   - Features are standardized using `StandardScaler`.

8. **Train the Model**:
   - A logistic regression model is trained on the scaled training data.

9. **Evaluate the Model**:
   - Predictions are made on the test set, and the model's accuracy and classification report are computed.

10. **Visualize Results**:
    - A confusion matrix is created and visualized using a heatmap.

