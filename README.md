Working Procedure
This section describes the complete workflow for the Iris Flower Classification project using Random Forest:

1. Data Acquisition
Download the Iris dataset from the UCI Machine Learning Repository.
Save the dataset as Iris.csv in your project directory.

2. Data Loading and Preprocessing
Load Data: The script reads the Iris.csv using pandas.
Column Cleanup: If the "Id" column is present, it is dropped as it is not relevant for prediction.
Label Encoding: The Species column (which contains string labels: Setosa, Versicolor, Virginica) is converted into numerical labels using LabelEncoder from scikit-learn. This step is necessary for the machine learning model to process categorical data.

3. Feature Selection and Splitting
Feature Matrix (X): All columns except Species are treated as input features.
Target Vector (y): The encoded Species column is the target.
Train-Test Split: The dataset is divided into training (80%) and testing (20%) sets using train_test_split, ensuring the model is evaluated on unseen data.

4. Model Building and Training
Model Selection: A RandomForestClassifier is initialized with 100 trees (n_estimators=100) and a fixed random seed for reproducibility.
Training: The classifier is fitted to the training data using the .fit() method.

5. Prediction
The trained model predicts the species for the test data using the .predict() method.

6. Model Evaluation
Accuracy Score: The script prints the percentage of correct predictions on the test set.
Classification Report: Detailed metrics including precision, recall, and f1-score for each class are displayed.
Actual vs. Predicted Display: For each test instance, the actual and predicted values are printed, allowing you to see where the model performed well or made mistakes.

7. Result Analysis
Analyze the accuracy and classification report to assess model performance.
Inspect the actual vs. predicted output to understand any misclassifications and gain insights into model behavior.

In summary:
The project covers the full machine learning cycle: data acquisition, preprocessing, feature selection, model training, prediction, evaluation, and result analysis, providing a hands-on introduction to supervised classification with Python and scikit-learn.
