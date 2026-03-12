# Cat vs Dog Image Classification using HOG and CNN Features

## Project Overview

This project performs **image classification of cats and dogs** using two different feature extraction approaches and compares their performance.

The goal is to evaluate which feature extraction technique provides better classification accuracy when combined with a **Support Vector Machine (SVM)** classifier.

## Methods Used

Two different approaches were implemented:

### 1. HOG + SVM

* Images are resized to **128 × 128**
* **Histogram of Oriented Gradients (HOG)** features are extracted
* Features are normalized using **StandardScaler**
* A **Support Vector Machine (SVM)** classifier is trained on the extracted features

### 2. CNN Feature Extraction + SVM

* Images are resized to **224 × 224**
* Features are extracted using a **pretrained ResNet18 CNN model**
* The final classification layer is removed to use the network as a **feature extractor**
* Extracted deep features are used to train an **SVM classifier**

## Libraries and Tools

The following libraries were used in this project:

* Python
* OpenCV
* NumPy
* Pandas
* Scikit-learn
* PyTorch
* Torchvision
* Matplotlib
* Seaborn
* scikit-image (HOG)

## Dataset Structure

The dataset directory contains two folders:

dataset/
│
├── cats/
└── dogs/

Each folder contains images belonging to its respective class.

## Evaluation

Both models were evaluated using:

* Train-test split (80/20)
* Accuracy score
* Classification report
* Confusion matrix
* ROC curve

## Results

The **CNN-based feature extraction using ResNet18** produced higher classification accuracy compared to the **HOG feature extraction method**.

This shows that **deep learning features capture more complex image patterns than traditional hand-crafted features.**



Ali Ahmed
