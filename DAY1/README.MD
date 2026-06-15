# Handwritten Digit Recognition using CNN (MNIST)

## Project Overview

This project is a Deep Learning-based Handwritten Digit Recognition System developed using Convolutional Neural Networks (CNNs) and TensorFlow/Keras.

The model is trained on the MNIST dataset from the Kaggle Digit Recognizer competition and is capable of identifying handwritten digits from 0 to 9 with high accuracy.

The objective of this project is to demonstrate the complete Deep Learning workflow, including data preprocessing, exploratory data analysis, model development, training, evaluation, prediction, and Kaggle submission generation.

---

## Problem Statement

Handwritten digit recognition is one of the most fundamental Computer Vision problems.

Given a grayscale image of a handwritten digit, the model must correctly classify it into one of the ten classes:

* 0
* 1
* 2
* 3
* 4
* 5
* 6
* 7
* 8
* 9

---

## Business Applications

Handwritten digit recognition is widely used in:

* Bank cheque processing
* Postal code recognition
* Automated form processing
* Educational examination systems
* Healthcare record digitization
* Logistics and package tracking
* Government document processing

---

## Dataset Information

Dataset Source:

Kaggle Digit Recognizer Competition

Dataset consists of:

### Training Dataset

* 42,000 images
* 785 columns
* 784 pixel features
* 1 target column (label)

### Test Dataset

* 28,000 images
* 784 pixel features

### Image Properties

* Grayscale images
* Resolution: 28 × 28 pixels
* Total pixels per image: 784

---

## Technologies Used

### Programming Language

* Python

### Libraries

* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* TensorFlow
* Keras

---

## Project Workflow

### 1. Data Loading

* Import training data
* Import test data

### 2. Data Understanding

* Dataset shape analysis
* Feature inspection
* Label analysis

### 3. Data Cleaning

* Missing value detection
* Duplicate record inspection

### 4. Data Visualization

* Sample digit visualization
* Class distribution analysis

### 5. Data Preprocessing

* Feature-target separation
* Pixel normalization
* Image reshaping
* One-hot encoding

### 6. Data Augmentation

Applied:

* Rotation
* Width shift
* Height shift
* Zoom

Purpose:

* Reduce overfitting
* Improve generalization

### 7. CNN Model Development

Architecture:

Conv2D → MaxPooling

Conv2D → MaxPooling

Flatten

Dense Layer

Dropout

Output Layer (Softmax)

### 8. Model Training

* Optimizer: Adam
* Loss Function: Categorical Crossentropy
* Metric: Accuracy

### 9. Model Evaluation

* Validation Accuracy
* Training Accuracy
* Loss Analysis

### 10. Prediction

* Generate predictions on unseen test data
* Create Kaggle submission file

---

## CNN Architecture

Input Shape:

28 × 28 × 1

Layer Structure:

```text
Input Layer
↓
Conv2D (32 Filters)
↓
MaxPooling2D
↓
Conv2D (64 Filters)
↓
MaxPooling2D
↓
Flatten
↓
Dense (128 Neurons)
↓
Dropout (0.5)
↓
Dense (10 Neurons, Softmax)
```

---

## Why CNN?

Traditional Machine Learning models require manual feature extraction.

CNN automatically learns:

* Edges
* Curves
* Shapes
* Patterns
* Digit structures

This makes CNN highly effective for image classification tasks.

---

## Model Performance

Typical Results:

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 92–94%   |
| Random Forest       | 95–97%   |
| CNN                 | 98–99%   |

---

## Project Structure

```text
Digit-Recognizer/
│
├── train.csv
├── test.csv
├── digit_recognizer.ipynb
├── submission.csv
├── digit_recognizer_model.h5
├── README.md
│
└── images/
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/digit-recognizer.git
```

Move into project directory:

```bash
cd digit-recognizer
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Open Jupyter Notebook:

```bash
jupyter notebook
```

Run:

```bash
digit_recognizer.ipynb
```

---

## Future Improvements

Possible enhancements:

* Batch Normalization
* Early Stopping
* Learning Rate Scheduling
* Hyperparameter Tuning
* LeNet Architecture
* ResNet Architecture
* Vision Transformers (ViT)
* FastAPI Deployment
* Docker Containerization
* Cloud Deployment

---

## Learning Outcomes

Through this project, I learned:

* Deep Learning fundamentals
* Convolutional Neural Networks
* Image preprocessing
* Data augmentation
* Model evaluation
* Kaggle competition workflow
* TensorFlow/Keras implementation
* Computer Vision fundamentals

---

## Author

Argha Sarkar

MBA (Analytics & Data Science)

Data Science | Machine Learning | Deep Learning | Business Analytics | Computer Vision

---

## License

This project is intended for educational, research, and portfolio purposes.

