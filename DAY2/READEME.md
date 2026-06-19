# Fashion MNIST Image Classification using Deep Learning (CNN)

## Project Overview

This project focuses on building a Convolutional Neural Network (CNN) to classify clothing images from the Fashion-MNIST dataset. The goal is to train a deep learning model that can automatically recognize different fashion products such as T-shirts, shoes, bags, dresses, and more.

Fashion-MNIST is a popular benchmark dataset in computer vision and is often considered a more challenging replacement for the classic MNIST handwritten digits dataset.

---

## Dataset Information

The dataset contains grayscale images of fashion products.

* Training Images: 60,000
* Test Images: 10,000
* Image Size: 28 × 28 pixels
* Number of Classes: 10

### Classes

| Label | Category    |
| ----- | ----------- |
| 0     | T-Shirt/Top |
| 1     | Trouser     |
| 2     | Pullover    |
| 3     | Dress       |
| 4     | Coat        |
| 5     | Sandal      |
| 6     | Shirt       |
| 7     | Sneaker     |
| 8     | Bag         |
| 9     | Ankle Boot  |

---

## Project Workflow

### 1. Data Loading

* Loaded Fashion-MNIST CSV files
* Explored dataset structure
* Checked dimensions and labels

### 2. Data Preprocessing

* Separated features and target labels
* Normalized pixel values from 0–255 to 0–1
* Reshaped images into CNN-compatible format `(28, 28, 1)`

### 3. Exploratory Data Analysis

* Visualized sample images
* Examined class distribution
* Verified dataset balance

### 4. Data Augmentation

Applied image augmentation techniques to improve model generalization:

* Rotation
* Zoom
* Width shifting
* Height shifting

### 5. Model Development

Built a deep Convolutional Neural Network using:

* Convolution Layers
* Batch Normalization
* Max Pooling
* Dropout Regularization
* Fully Connected Dense Layers
* Softmax Output Layer

### 6. Training Strategy

Used several techniques to improve performance:

* Early Stopping
* Learning Rate Reduction
* Model Checkpointing
* Validation Monitoring

### 7. Model Evaluation

Evaluated the model using:

* Validation Accuracy
* Confusion Matrix
* Classification Report
* Training & Validation Curves

### 8. Model Saving

Saved the best-performing model for future deployment and inference.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* TensorFlow
* Keras

---

## Model Architecture

Input Image (28×28×1)

↓

Conv2D (32 Filters)

↓

Batch Normalization

↓

Conv2D (32 Filters)

↓

Batch Normalization

↓

Max Pooling

↓

Dropout

↓

Conv2D (64 Filters)

↓

Batch Normalization

↓

Conv2D (64 Filters)

↓

Batch Normalization

↓

Max Pooling

↓

Dropout

↓

Conv2D (128 Filters)

↓

Batch Normalization

↓

Max Pooling

↓

Dropout

↓

Flatten

↓

Dense (256)

↓

Dropout

↓

Dense (10)

↓

Softmax

---

## Results

The model achieved strong classification performance on the Fashion-MNIST dataset.

Expected validation accuracy:

**93% – 96%**

The model performed particularly well on:

* Trouser
* Bag
* Sneaker
* Ankle Boot

Some confusion was observed between visually similar categories such as:

* Shirt and T-Shirt
* Coat and Pullover

---

## Key Learning Outcomes

Through this project I learned:

* Image preprocessing techniques
* CNN architecture design
* Data augmentation strategies
* Batch normalization and dropout
* Deep learning model evaluation
* Hyperparameter optimization
* Model saving and loading
* Practical computer vision workflows

---

## Future Improvements

Potential improvements for future work:

* ResNet Architecture
* Transfer Learning
* Vision Transformers (ViT)
* Hyperparameter Tuning
* TensorBoard Integration
* FastAPI Deployment
* Docker Containerization
* Cloud Deployment (AWS/Azure/GCP)

---

## How to Run

1. Clone the repository

```bash
git clone <repository-url>
```

2. Install required libraries

```bash
pip install -r requirements.txt
```

3. Run the notebook or Python script

```bash
python train.py
```

4. The trained model will be saved automatically after training.

---

## Author

Argha Sarkar

This project was developed as part of my Deep Learning and Computer Vision learning journey to strengthen practical skills in image classification and modern neural network architectures.
