# Iris Classification with Machine Learning

## Table of Contents
- [Project Overview](#Project-Overview)
- [Dataset](#Dataset)
- [Algorithms](#Algorithms)
- [Results](#Results)
  * [Outcome](#Outcome)
  * [Accuracy Table](#Accuracy-Table)
  * [Confusion Matrix](#Confusion-Matrix)
  * [Classification Report](#Classification-Report)
- [Steps](#Steps)
- [Credit](#Credit)

## Project Overview
Evaluated 6 different machine learning algorithms and implemented the method with the highest accuracy to predict iris classifications. 

## Dataset
Utilized a variation of the classic iris data set (https://archive.ics.uci.edu/ml/datasets/Iris) that would be split into a training set and a cross-validation set (80/20).

## Algorithms
- Logistic Regression (LR)
- Linear Discriminant Analysis (LDA)
- K-Nearest Neighbors (KNN)
- Classification and Regression Trees (CART)
- Gaussian Naive Bayes (NB)
- Support Vector Machines (SVM)

## Results

### Outcome
SVM was the selected algorithm with the highest accuracy at 98.33% and the lowest standard deviation of 3.33%. When applied to the cross-validation set, the accuracy was 96.67%. The outcome is satisfactory as I am 96% confidence that the algorithm will correctly classify the iris. Next steps would be to measure bias and variance using learning curves to determine potential optimizations.

### Accuracy Table
| Algo | Accuracy | STD |
| :---: | :---: | :---: |
| LR | 0.941667 | (0.065085) |
| LDA | 0.975000 | (0.038188) |
| KNN | 0.958333 | (0.041667) |
| CART | 0.941667 | (0.038188) |
| NB | 0.950000 | (0.055277) |
| `SVM` | `0.983333` | `(0.033333)` |

### Confusion Matrix

| | Iris-setosa | Iris-versicolor | Iris-virginica |
| :---: | :---: | :---: | :---: |
| Iris-setosa | 11 | 0 | 0 |
| Iris-versicolor | 0 | 12 | 1 |
| Iris-virginica | 0 | 0 | 6 |

 ### Classification Report
| Class | Precision | Recall | F1-Score | Support |
| :---: | :---: | :---: | :---: | :---: |
| Iris-setosa | 1.00 | 1.00 | 1.00 | 11 |
| Iris-versicolor | 1.00 | 0.92 | 0.96 | 13 |
| Iris-virginica | 0.86 | 1.00 | 0.92 | 6 |

## Steps
1. Import libraries
2. Load and review data set
3. Visualize data set
4. Evaluate and compare algorithms
5. Make predictions
6. Evaluate predictions

## Credit
To Jason Brownlee @ https://machinelearningmastery.com/ for the project