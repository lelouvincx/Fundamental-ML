# Mini-Project for Fundamentals of Machine Learning Course

![background](./materials/ai_wp.jpg)

This repository contains the code and data for a mini-project on facial expression recognition using machine learning algorithms.

This is a mini-project for the Fundamentals of Machine Learning course at the VNU-HCM University of Science. The project is designed to practice the machine learning concepts we've learned in the course, including data preprocessing, exploratory data analysis (EDA), and classification tasks.

## 📑 Project Policy
- Team: group should consist of 3-4 students.

    |No.| Student Name    | Student ID |
    | --------| -------- | ------- |
    |1| Dinh Minh Chinh | 21280007 |
    |2| Pham Nhat Hao | 21280066 |
    |3| Le Tran Bao Ngoc | 21280036 |

- The submission deadline is strict: **11:59 PM** on **June 22nd, 2024**. Commits pushed after this deadline will not be considered.

## 📦 Project Structure

The repository is organized into the following directories:

- **/data**: This directory contains the facial expression dataset. You'll need to download the dataset and place it here before running the notebooks. (Download link provided below)
- **/notebooks**: This directory contains the Jupyter notebook ```EDA.ipynb```. This notebook guides you through exploratory data analysis (EDA) and classification tasks.

## ⚙️ Usage

This project is designed to be completed in the following steps:

1. **Fork the Project**: Click on the ```Fork``` button on the top right corner of this repository, this will create a copy of the repository in your own GitHub account. Complete the table at the top by entering your team member names.

2. **Download the Dataset**: Download the facial expression dataset from the following [link](https://mega.nz/file/foM2wDaa#GPGyspdUB2WV-fATL-ZvYj3i4FqgbVKyct413gxg3rE) and place it in the **/data** directory:

3. **Complete the Tasks**: Open the ```notebooks/EDA.ipynb``` notebook in your Jupyter Notebook environment. The notebook is designed to guide you through various tasks, including:
    
    1. Prerequisite
    2. Principle Component Analysis
    3. Image Classification
    4. Evaluating Classification Performance 

    Make sure to run all the code cells in the ```EDA.ipynb``` notebook and ensure they produce output before committing and pushing your changes.

5. **Commit and Push Your Changes**: Once you've completed the tasks outlined in the notebook, commit your changes to your local repository and push them to your forked repository on GitHub.


Feel free to modify and extend the notebook to explore further aspects of the data and experiment with different algorithms. Good luck.

## Dataset Description

The data consists of 48x48 pixel grayscale images of faces. The faces have been automatically registered so that the face is more or less centered and occupies about the same amount of space in each image. The task is to categorize each face based on the emotion shown in the facial expression in to one of seven categories:

0. Angry
Example:
![](./images/example_angry.png)

1. Disgust
Example:
![](./images/example_disgust.png)

2. Fear
Example:
![](./images/example_fear.png)

3. Happy
Example:
![](./images/example_happy.png)

4. Sad
Example:
![](./images/example_sad.png)

5. Surprise
Example:
![](./images/example_surprise.png)

6. Neutral
Example:
![](./images/example_neutral.png)

## Training Phase

To compare the performance of the models trained on the original data versus the transformed data, let's analyze and contrast their evaluation metrics: accuracy, precision, recall, and F1-score.

### Performance on Original Data:
- **Logistic Regression**:
  - Accuracy: 0.4304
  - Precision: 0.4034
  - Recall: 0.4304
  - F1-Score: 0.3995
- **KNN**:
  - Accuracy: 0.4490
  - Precision: 0.4368
  - Recall: 0.4490
  - F1-Score: 0.4344
- **Random Forest**:
  - Accuracy: 0.4390
  - Precision: 0.4402
  - Recall: 0.4390
  - F1-Score: 0.4190
- **MLP**:
  - Accuracy: 0.4569
  - Precision: 0.4528
  - Recall: 0.4569
  - F1-Score: 0.4412

### Performance on Transformed Data:
- **Logistic Regression**:
  - Accuracy: 0.3928
  - Precision: 0.3753
  - Recall: 0.3928
  - F1-Score: 0.3521
- **KNN**:
  - Accuracy: 0.4492
  - Precision: 0.4360
  - Recall: 0.4492
  - F1-Score: 0.4346
- **Random Forest**:
  - Accuracy: 0.4292
  - Precision: 0.4336
  - Recall: 0.4292
  - F1-Score: 0.4083
- **MLP**:
  - Accuracy: 0.2916
  - Precision: 0.3326
  - Recall: 0.2916
  - F1-Score: 0.1890

### Comparison:

#### Logistic Regression:

- **Original Data**: Better performance across all metrics compared to transformed data.
  - Accuracy: 0.4304 vs. 0.3928
  - Precision: 0.4034 vs. 0.3753
  - Recall: 0.4304 vs. 0.3928
  - F1-Score: 0.3995 vs. 0.3521

#### KNN:

- **Transformed Data**: Slightly better performance in accuracy and F1-score, but very close in all metrics.
  - Accuracy: 0.4492 vs. 0.4490
  - Precision: 0.4360 vs. 0.4368
  - Recall: 0.4492 vs. 0.4490
  - F1-Score: 0.4346 vs. 0.4344

#### Random Forest:

- **Original Data**: Better performance across all metrics compared to transformed data.
  - Accuracy: 0.4390 vs. 0.4292
  - Precision: 0.4402 vs. 0.4336
  - Recall: 0.4390 vs. 0.4292
  - F1-Score: 0.4190 vs. 0.4083

#### MLP:

- **Original Data**: Significantly better performance across all metrics compared to transformed data.
  - Accuracy: 0.4569 vs. 0.2916
  - Precision: 0.4528 vs. 0.3326
  - Recall: 0.4569 vs. 0.2916
  - F1-Score: 0.4412 vs. 0.1890

### Summary:

- **Logistic Regression and Random Forest** models perform better with the original data across all metrics.
- **KNN** shows almost identical performance on both datasets, with a slight edge in accuracy and F1-score on transformed data.
- **MLP** performs significantly better on the original data.

### Best Model Overall:

- **MLP** trained on original data achieves the highest accuracy (0.4569), precision (0.4528), recall (0.4569), and F1-score (0.4412).

In conclusion, the MLP model trained on the original data performs best overall, and models generally perform better on the original data compared to the transformed data.

## Evaluation Phase

To compare the performance of the classification models (Logistic Regression, KNN, Random Forest, and MLP), let's analyze their evaluation metrics: accuracy, precision, recall, and F1-score.

### Accuracy

- **Logistic Regression**: 0.39
- **KNN**: 0.45
- **Random Forest**: 0.43
- **MLP**: 0.29

### Macro Average Precision:

- **Logistic Regression**: 0.33
- **KNN**: 0.43
- **Random Forest**: 0.51
- **MLP**: 0.26

### Macro Average Recall:

- **Logistic Regression**: 0.30
- **KNN**: 0.42
- **Random Forest**: 0.37
- **MLP**: 0.21

### Macro Average F1-score:

- **Logistic Regression**: 0.28
- **KNN**: 0.42
- **Random Forest**: 0.39
- **MLP**: 0.13

### Weighted Average Precision:

- **Logistic Regression**: 0.38
- **KNN**: 0.44
- **Random Forest**: 0.43
- **MLP**: 0.33

### Weighted Average Recall:

- **Logistic Regression**: 0.39
- **KNN**: 0.45
- **Random Forest**: 0.43
- **MLP**: 0.29

### Weighted Average F1-score:

- **Logistic Regression**: 0.35
- **KNN**: 0.43
- **Random Forest**: 0.41
- **MLP**: 0.19

### Analysis:

- **Accuracy**: KNN has the highest accuracy (0.45), indicating it correctly classifies the most samples overall.
- **Macro Average Precision**: Random Forest has the highest precision (0.51), suggesting it is better at minimizing false positives across all classes.
- **Macro Average Recall**: KNN has the highest recall (0.42), showing it captures true positives well across all classes.
- **Macro Average F1-score**: KNN has the highest F1-score (0.42), indicating the best balance between precision and recall for all classes.
- **Weighted Average Precision, Recall, and F1-score**: KNN consistently has the highest values across these metrics, reinforcing its superior performance.

## Conclusion:

Based on the evaluation metrics, **KNN (K-Nearest Neighbors)** performs the best overall. It has the highest accuracy, recall, and F1-score. This indicates that KNN balances true positives and false positives effectively, making it the most reliable model among the four tested for this specific dataset. Random Forest has the highest precision but lower recall and F1-score, indicating it is more conservative but misses more true positives. MLP has the lowest performance across all metrics, suggesting it is not suitable for this dataset.