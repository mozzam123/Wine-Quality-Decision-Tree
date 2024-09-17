# Wine Quality Decision Tree Prediction

This project demonstrates how to build a machine learning model using a Decision Tree Classifier to predict wine quality based on various physicochemical properties of wine. The focus is on predicting wine quality based on attributes like acidity, sugar content, alcohol level, and others.

## Project Overview

The project follows these key steps:

1. **Data Preparation**:
   - The Wine Quality dataset is used for this project. The dataset consists of multiple features like acidity, sugar content, pH level, alcohol content, etc., with the target variable being the wine's quality.
   - Features (`X`) were separated from the target variable (`y`), which is the wine quality rating.

2. **Data Splitting**:
   - The dataset is split into training and testing sets using an 80:20 ratio, ensuring that the model is trained on one part and tested on another for unbiased performance evaluation.

3. **Model Building**:
   - A **Decision Tree Classifier** was employed to build the predictive model for wine quality. The model was trained on the training set using the `fit` method of the `DecisionTreeClassifier` class.

4. **Model Evaluation**:
   - The model's predictions were tested using the testing set, and its accuracy was computed.
   - A cross-validation strategy (with 5 folds) was applied to assess the stability and generalizability of the model across different subsets of the data.

5. **Performance Metrics**:
   - **Accuracy**: The model's accuracy was measured on the test set to evaluate its performance.
   - **Cross-Validation Accuracy**: Cross-validation was used to ensure that the model performs consistently across different data splits.

## Model Results

- **Test Set Accuracy**: The accuracy of the Decision Tree Classifier was computed using the `accuracy_score` method. 
- **Cross-Validation Accuracy**: Cross-validation accuracy was calculated using the `cross_val_score` method, providing a more generalized performance evaluation.

## Dependencies

The project requires the following Python libraries:

- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical operations.
- **scikit-learn**: For building and evaluating machine learning models.
- **matplotlib** & **seaborn**: For visualizing data and model performance.

You can install these libraries using the following command:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
