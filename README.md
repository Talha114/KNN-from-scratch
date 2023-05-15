# Using KNN Algorithm to predict if a person will have diabetes or not (KNN from scratch)

This project implements the K-Nearest Neighbors algorithm to predict if a person will have diabetes or not. The dataset used is the Pima Indians Diabetes Database from the UCI Machine Learning Repository.

## Libraries Used

- NumPy: For performing numerical operations.
- Pandas: For data manipulation and analysis.
- scikit-learn: For machine learning tasks such as train-test splitting, standardization, and KNN classification.
- Seaborn: For creating visualizations.
- Matplotlib: For creating plots and charts.

## Loading the Dataset

The dataset used in this project is 'diabetes.csv'. It contains 768 rows and 9 columns. The columns are as follows:

- Pregnancies: Number of times pregnant
- Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
- BloodPressure: Diastolic blood pressure (mm Hg)
- SkinThickness: Triceps skin fold thickness (mm)
- Insulin: 2-Hour serum insulin (mu U/ml)
- BMI: Body mass index (weight in kg/(height in m)^2)
- DiabetesPedigreeFunction: Diabetes pedigree function
- Age: Age (years)
- Outcome: Class variable (0 or 1)

## KNN Algorithm

The K-Nearest Neighbors algorithm is a supervised machine learning algorithm that can be used for classification and regression. It works by finding the K nearest data points in the training set to a test data point and assigning a label based on the most common label among those K points.

### Euclidean Distance

The Euclidean distance is used to measure the distance between two points in n-dimensional space. In this project, the Euclidean distance is used to find the distance between the test data point and each training data point.

### Implementation

The KNN algorithm is implemented from scratch in this project. The `euclidean_dist` function calculates the Euclidean distance between two data points. The `KNN` function uses this distance calculation to find the K nearest neighbors to a test data point. It then assigns a label to the test data point based on the most common label among those K neighbors.

### Results

The KNN algorithm is run for K values of 2, 9, 18, 21, and 23. The accuracy of the algorithm is calculated for each value of K using the F1 score and confusion matrix. The results are plotted using a line chart.

## Conclusion

In this project, we implemented the K-Nearest Neighbors algorithm from scratch to predict if a person will have diabetes or not. We achieved good accuracy results using the F1 score and confusion matrix. The KNN algorithm is a simple yet effective algorithm that can be used for classification tasks.
