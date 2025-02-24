<div align='center'>
  <h1 align='center'>Heart Diseases Analysis and Classification</h1>
</div>
<br>

## About this Project
This project aims to study and classify a widely known dataset in data science community: the [UCI Heart Diseases](https://archive.ics.uci.edu/dataset/45/heart+disease) dataset. It is used as a tool to develop key Machine Learning techniques while trying to classify the dataset and develop an analysis.

### Problem Overview
According to WHO (World Health Organization), approximately 32% of deaths worldwide are caused by heart diseases by 2019. Therefore, developing a machine learn based classification algorithm can lead to much faster identification of said diseases, possibly enabling better treatment.

### Goals
- Identifying features that indicate a disease
- Finding correlation between health indicators and heart diseases

## Contributors
- [João P. B. Silva](https://github.com/buzzo-cancri)
- [Victor H. T. Amaral](https://github.com/AmaralVh)

## Dataset Information
The [dataset](https://archive.ics.uci.edu/dataset/45/heart+disease) used includes:
- Patient age
- Cholesterol level present in blood
- Maximum heartbeat levels after stress
- Maximum heartbeat levels while resting
- Amount of blood vessels obstructed (identified through fluoroscopy)

The dataset consists of scattered data from multiple sources, with a significant presence of null values (mostly __ca__ feature). Therefore, two analysis are made simultaneously: one considering no null values, one without the feature __ca__.

## Models Utilized
The classification models utilized were:
- K-Nearest Neighbors
- Decision Tree Classifier
- Support Vector Machine - Linear
- Support Vector Machine - Polynomial Kernel (Degree 3)
- Multi-Layered Perceptron

## Results
The results from the classification are separated into two tables, considering the two analysis made.

First, the classification without __ca__ feature:

| Model | Accuracy | Recall | Precision | F1-Score |
|-------|----------|--------|-----------|----------|
| KNN | 0,80 | 0,80 | 0,83 | 0,81 |
| DT | 0,77 | 0,77 | 0,80 | 0,78 |
| SVM (Linear) | 0,81 | 0,81 | 0,84 | 0,82 |
| SVM (Poly3) | 0,81 | 0,79 | 0,85 | 0,82 |
| MLP | 0,77 | 0,78 | 0,79 | 0,78 |

Second, the classification with no null values:

| Model | Accuracy | Recall | Precision | F1-Score |
|-------|----------|--------|-----------|----------|
| KNN | 0,80 | 0,80 | 0,78 | 0,79 |
| DT | 0,80 | 0,76 | 0,80 | 0,77 |
| SVM (Linear) | 0,83 | 0,79 | 0,83 | 0,81 |
| SVM (Poly3) | 0,84 | 0,76 | 0,87 | 0,81 |
| MLP | 0,74 | 0,73 | 0,74 | 0,70 |

## Dependencies
- Pandas: Data manipulation and analysis
- NumPy: Mathematical and array operations
- Seaborn: Data visualization
- Scikit-learn: Machine Learning models and preprocessing
- Imbalanced Learn: Preprocessing

## Acknowledgements
This project was developed under the supervision of Prof. Roseli Aparecida Francelin Romero at the Institute of Mathematical and Computer Sciences (ICMC) - University of São Paulo.
