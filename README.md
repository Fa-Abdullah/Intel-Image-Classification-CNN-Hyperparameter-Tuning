# Intel-Image-Classification-CNN-Hyperparameter-Tuning

---

## Overview

This project focuses on classifying images into 6 categories using Convolutional Neural Networks (CNN). The dataset used is the Intel Image Classification dataset from Kaggle, which contains natural and urban scene images.

---

## Classes

| Index | Class       |
|-------|-------------|
| 0     | Buildings   |
| 1     | Forest      |
| 2     | Glacier     |
| 3     | Mountain    |
| 4     | Sea         |
| 5     | Street      |

---

## Technologies Used

- Python 
- TensorFlow / Keras
- OpenCV
- NumPy / Pandas
- Matplotlib / Seaborn
- Scikit-learn
- KaggleHub (for dataset download)

---

## Model Architecture

The model is built using CNN and includes:

- Conv2D layers with ReLU Activation
- MaxPooling2D layers
- Flatten layer
- Dense layers with Dropout to reduce overfitting
- BatchNormalization for better training
- Optimizer: Adam
- Loss Function: CategoricalCrossentropy

---

## Data Augmentation

Used to improve model performance and avoid overfitting:

ImageDataGenerator(
    rescale=1.0/255,
    zoom_range=0.3,
    width_shift_range=0.30,
    height_shift_range=0.30,
    fill_mode='nearest'
)

---

## Expected Results

- Training Accuracy: ~90%+
- Test Accuracy: ~85%+
- Confusion Matrix and Classification Report will be displayed for detailed performance evaluation per class.

---

## References

- Intel Image Classification Dataset on Kaggle: https://www.kaggle.com/datasets/puneet6060/intel-image-classification
- TensorFlow Documentation: https://www.tensorflow.org/

---

## Author

Fatma Abdullah

