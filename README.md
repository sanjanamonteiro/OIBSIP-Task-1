Working Procedure

# Iris Flower Classification using Random Forest

## Objective

This project demonstrates how to classify Iris flower species using the Random Forest algorithm. The goal is to accurately predict the species (`Iris-setosa`, `Iris-versicolor`, `Iris-virginica`) based on flower measurements.

## Steps Performed

1. **Data Loading & Exploration**
   - The Iris dataset is loaded into a pandas DataFrame.
   - Initial exploration includes viewing the first few rows, checking data types, statistical summary, and class distribution.
   - Data visualization is performed using seaborn's pairplot to understand feature relationships.
   - The presence of missing values is checked.

2. **Preprocessing**
   - The `Id` column (if present) is dropped, as it does not contribute to classification.
   - Species labels are encoded from string names to integers using `LabelEncoder`.

3. **Feature and Target Selection**
   - Features (`X`) consist of the four flower measurements: sepal length, sepal width, petal length, and petal width.
   - The target (`y`) is the encoded species.

4. **Data Splitting**
   - The dataset is split into training and testing sets (80/20 split) to evaluate model performance.

5. **Model Training**
   - A `RandomForestClassifier` is instantiated and trained on the training data.

6. **Evaluation**
   - The model's predictions are compared to actual values using:
     - **Accuracy Score**: Overall correctness of the model.
     - **Classification Report**: Precision, recall, and F1-score for each class.
     - **Confusion Matrix**: Visual representation of prediction errors.
   - Actual vs. predicted values for the test set are printed.

## Tools Used

- **Python**: Programming language for implementation.
- **pandas**: Data manipulation and analysis.
- **seaborn & matplotlib**: Data visualization.
- **scikit-learn**: Machine learning library for data splitting, preprocessing, model training, and evaluation.

## Outcome

- The Random Forest model achieves high accuracy in classifying the Iris species.
- Evaluation metrics (accuracy, classification report, confusion matrix) demonstrate the effectiveness of the model.
- The workflow demonstrates a standard approach to supervised classification tasks, from data exploration to model evaluation.

## Requirements

- pandas
- scikit-learn
- seaborn
- matplotlib

Install requirements with:
```bash
pip install pandas scikit-learn seaborn matplotlib
```

