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

## Answer

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
