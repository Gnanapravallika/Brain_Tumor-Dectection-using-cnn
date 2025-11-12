# 🧠 Brain Tumor Detection using CNN with PyTorch

## Overview

This repository contains the code for a Convolutional Neural Network (CNN) model developed with PyTorch for **Brain Tumor Detection** from MRI images. The model classifies MRI scans into two categories: **Brain Tumor (Cancer)** or **Healthy (Not Cancer)**. The project demonstrates key machine learning concepts, including data preparation, augmentation, custom CNN architecture definition, training/validation, and performance evaluation.

## 🌟 Features

* **Custom CNN Model:** A four-layer convolutional network (`CNN_TUMOR`) built from scratch using PyTorch's `nn.Module`.
* **Data Augmentation:** Techniques applied to increase the diversity of the training data, including resizing, random horizontal/vertical flips, and rotation.
* **Train/Validation Split:** The initial dataset is automatically split into training and validation sets (80/20 ratio).
* **Training & Evaluation:** Uses standard PyTorch training loop with `NLLLoss`, `Adam` optimizer, and `ReduceLROnPlateau` scheduler.
* **Performance Metrics:** Detailed evaluation using a classification report and a visual confusion matrix.

## 💾 Dataset

The project utilizes a dataset of brain MRI images organized into two classes:
* `Brain Tumor`
* `Healthy`

The dataset is loaded from the Kaggle input path: `/kaggle/input/brian-tumor-dataset/`.

**Data Distribution (After 80/20 split as seen in the notebook output):**

| Set | Total Samples |
| :--- | :--- |
| **Training** | 3680 |
| **Validation** | 920 |
| **Total** | 4600 |

## 🛠️ Technologies and Prerequisites

This project requires Python and several popular data science and machine learning libraries.

* Python (3.x recommended)
* PyTorch
* NumPy
* Pandas
* Matplotlib
* Seaborn
* `split-folders`
* `torch-summary`
* Scikit-learn (`sklearn`)

You can install the necessary PyTorch and other required packages using `pip`:

```bash
# Install required libraries
pip install torch torchvision numpy pandas matplotlib seaborn scikit-learn split-folders torch-summary# Brain_Tumor-Dectection-using-cnn


raining and Results
The model was successfully trained for 60 epochs.

The final performance of the CNN model on the Validation Set is summarized below:

Classification Report

Class,Precision,Recall,F1-Score,Support
0.0 (Brain Tumor),0.96,0.98,0.97,503
1.0 (Healthy),0.97,0.95,0.96,418
Accuracy,,,0.97,921
Macro Avg,0.97,0.96,0.96,921
Weighted Avg,0.97,0.97,0.97,921
