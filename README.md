# Time Series Classification

---

## Project Description

This project involves classifying human activities based on time series data collected from a Wireless Sensor Network. The dataset used in this project is the AReM data, which contains multiple time series for different activities. The project focuses on feature extraction, binary and multiclass classification using various machine learning techniques.

## Key Features

### 1. Feature Creation/Extraction
- **Data Source**: The AReM dataset contains time series data for seven types of human activities.
- **Feature Extraction**: Time-domain features such as minimum, maximum, mean, median, standard deviation, first quartile, and third quartile are extracted for all time series in each instance.
- **Standard Deviation Estimation**: Standard deviation for each feature is estimated, and a 90% bootstrap confidence interval is built for the standard deviation of each feature.

### 2. Binary Classification
- **Logistic Regression**: Binary classification is performed to distinguish between bending and other activities using logistic regression.
- **Time Series Segmentation**: Time series data is segmented into smaller parts to analyze the impact on classification performance.
- **Recursive Feature Elimination**: Features are selected using recursive feature elimination to improve model performance.
- **Model Evaluation**: Confusion matrices, ROC curves, and AUC scores are used to evaluate the classifier's performance on training and test data.

### 3. Multiclass Classification
- **L1-penalized Logistic Regression**: Multinomial regression model using L1-penalty is implemented to classify all activities.
- **Naive Bayes Classifier**: Both Gaussian and Multinomial priors are used in Naive Bayes classification to compare results.
- **Model Comparison**: The performance of logistic regression and Naive Bayes classifiers is compared to determine the better method for multiclass classification.

