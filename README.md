# Scene Image Classification using Deep Learning

## Overview

This project develops deep learning-based image classification models to classify natural and urban scene images into six categories:

* Buildings
* Forest
* Glacier
* Mountain
* Sea
* Street

The project explores and compares multiple convolutional neural network (CNN) architectures, including a custom CNN model, EfficientNet, and ResNet, to evaluate their effectiveness in multi-class scene image classification.

---

# Objectives

* Perform exploratory data analysis (EDA) on scene image datasets.
* Apply image preprocessing and augmentation techniques.
* Train and evaluate multiple deep learning models.
* Compare model performance across architectures.
* Visualize model evaluation results and predictions.

---

# Dataset

Dataset used:

**Intel Image Classification Dataset**

The dataset contains natural scene images categorized into six classes:

* Buildings
* Forest
* Glacier
* Mountain
* Sea
* Street

Dataset source:
[https://www.kaggle.com/datasets/puneet6060/intel-image-classification](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)

---

# Tools Used

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* PIL

---

# Project Workflow

## 1. Data Loading and Exploratory Data Analysis

* Loaded training and testing image datasets.
* Converted image directories into structured DataFrames.
* Visualized sample images from each class.
* Analyzed image resolution distributions.
* Examined class balance and dataset characteristics.

## 2. Data Preprocessing

Different preprocessing pipelines were applied for each model architecture.

Techniques include:

* Image resizing
* Normalization
* Validation split generation
* Data augmentation

## 3. Model Training

Three deep learning architectures were implemented:

### Custom CNN (CNN2D)

A custom convolutional neural network designed for baseline image classification performance.

### EfficientNet

Transfer learning implementation using EfficientNet architecture for improved classification performance and efficiency.

### ResNet

Transfer learning implementation using ResNet architecture to evaluate deeper residual learning performance.

---

# Model Evaluation

Each model was evaluated using:

* Test Accuracy
* Test Loss
* Classification Metrics
* Prediction Visualization

The project compares model performance to determine the most effective architecture for scene image classification.

---

# Repository Structure

```text
scene-image-classification/
│
├── README.md
├── scene-image-classification-project.ipynb
├── models/
│   └── best_model.keras
├── results/
│   ├── confusion_matrix.png
│   ├── training_curve.png
│   └── sample_predictions.png
└── requirements.txt
```

---

# How to Run

## Clone Repository

```bash
git clone https://github.com/your-username/scene-image-classification.git
cd scene-image-classification
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run Notebook

Open the notebook using Jupyter Notebook or Google Colab:

```bash
jupyter notebook
```

---

# Results

The models successfully learned to classify scene images across six categories.

EfficientNet and ResNet architectures demonstrated stronger classification performance compared to the baseline CNN model due to transfer learning and deeper feature extraction capability.

---
