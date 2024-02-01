## Overview

This repository contains a machine learning model for duplicate question detection. The model utilizes Tf-IDF vectorizers and advanced feature engineering, including Fuzzy-Wuzzy string matching, to determine whether two given questions are duplicates. The model has been trained on a dataset consisting of Quora duplicate question pairs.

## Dataset

The dataset used for training contains over 400,000 question pairs from Quora, and the model has been trained on 50,000 data points. Despite the limited training data and computational resources, the model achieves an accuracy of 78%. This highlights the effectiveness of the implemented techniques in capturing the semantic similarity between questions.

## Features and Techniques

- **Tf-IDF Vectorizers**: Used for transforming text data into numerical vectors, capturing the importance of terms in the documents.

- **Fuzzy-Wuzzy String Matching**: Applied for advanced feature engineering, allowing the model to capture semantic similarity even in cases where exact word matches may not occur.

- **Algorithms Used**: Random Forest, XGBoost, Logistic Regression, and Naive Bayes have been employed to build and evaluate the model.

- **Hyperparameter Tuning**: Techniques such as GridSearch and cross-validation have been employed to find the optimal hyperparameters for each algorithm, ensuring better model performance.

## Model Evaluation

The model has been evaluated on various metrics, including accuracy, precision, recall, and F1-score. The achieved accuracy of 78% is noteworthy, considering the limited dataset size and computational resources.

## Results

### Effect of Custom engineered features

- Simple Features
![image](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/02c7bb67-f869-438b-8308-2b6067ed76b9)

- Fuzzy-Wuzzy Features
![image](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/02145a4f-2fc5-4a1d-a9f6-785ad91c29e0)


### Models Performance

#### Random Forest
![Random Forest Results](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/228c8a2d-d918-4b67-92db-9bde77c93e7f)

#### Naive Bayes
![Naive Bayes Results](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/be03035b-2d30-42e8-97f2-51300bc787dc)

#### Logistic Regression
![Logistic Regression Results](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/c65041be-e438-4e41-9769-23552882b4fb)

#### XG-Boost
![XG-Boost Results](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/bb300701-e881-4273-ace8-53388b7922d7)

### Results on Test Set
![Results on Testing](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/27c966d4-b147-4a2e-928d-c41a23293a73)

## Update

### New Deep Learning Model - LSTM Networks

I have implemented a new model using deep learning techniques, specifically utilizing Long Short-Term Memory (LSTM) networks. This model achieves an improved accuracy of 77% over all the data. The LSTM's ability to capture sequential dependencies and long-term patterns enhances the model's performance in understanding the semantic similarity between questions.

#### Dataset

The new model has been trained on the same dataset, which contains over 400,000 question pairs from Quora. The training data for the LSTM model includes 50,000 data points.

#### Features and Techniques

- **LSTM Networks**: Utilized for deep learning, providing the model with the ability to understand sequential patterns and dependencies in the data.

#### Model Evaluation

The LSTM model has been evaluated on various metrics, including accuracy, precision, recall, and F1-score. The achieved accuracy of 77% is noteworthy, considering the limited dataset size and computational resources.

#### Results
- ```Loss```
  
![image](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/9c327e80-be64-4340-9774-abe20a142171)

- ```Accuracy```

![image](https://github.com/xAn-x/Duplicate-Question-Pairs/assets/115899138/70ddb7e2-8603-44f1-8e9e-3fae509d17ee)


For more details check the deep-learning Notebook

Feel free to experiment with different parameters, algorithms, or feature engineering techniques to enhance the model's performance.

Happy coding!
