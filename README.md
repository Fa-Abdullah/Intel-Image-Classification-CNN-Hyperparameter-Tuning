# Intel-Image-Classification-CNN# Intel Image Classification – CNN with Hyperparameter Tuning

A multi-class image classification project on the Intel Image Classification dataset (6 scenes) using a Convolutional Neural Network (CNN) with advanced regularization techniques and hyperparameter tuning.

## What it does

- Classifies images into 6 categories: buildings, forest, glacier, mountain, sea, street
- Applies data augmentation (zoom, shift, fill_mode) to improve generalization
- Uses a CNN with:
  - BatchNormalization after each convolutional block
  - Dropout (0.5) for regularization
  - L2 regularization (kernel_regularizer)
  - ReduceLROnPlateau to dynamically adjust learning rate
- Includes hyperparameter tuning using Keras Tuner (Hyperband)

## Technologies

- Python
- TensorFlow / Keras
- OpenCV
- Scikit-learn
- Matplotlib / Seaborn
- Keras Tuner

## Model Architecture

The model consists of:
- 3 convolutional blocks (128 -> 64 -> 32 filters)
- BatchNormalization after each MaxPooling
- Flatten -> Dense(256) -> Dropout(0.5) -> Dense(128) -> Dropout(0.5) -> Dense(32) -> Dense(6, softmax)

## Results

After 50 epochs of training, the model achieves competitive accuracy on the test set with clear training/validation curves and a confusion matrix for detailed evaluation.

