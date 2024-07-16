# CNN Assignment

This folder contains the assignment on classifying CIFAR-10 images using a Convolutional Neural Network (CNN). The objective is to study the effect on the model's performance by varying the following modeling aspects:

1. Batch Normalization
2. Dropout
3. Number of convolution and pooling layers
4. Activation functions

## Files

- **Assignment_CNN.ipynb:** Jupyter Notebook with the complete code and analysis.
- **CNN_Presentation.pptx:** PowerPoint presentation summarizing the findings.

## Problem Definition

The CIFAR-10 dataset consists of 60000 32x32 color images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images. The objective is to develop a CNN model to classify these images into one of the 10 categories:

1. Airplane
2. Automobile
3. Bird
4. Cat
5. Deer
6. Dog
7. Frog
8. Horse
9. Ship
10. Truck

## Approach and Learnings

### Model Architecture

- **Initial Baseline:** 3 layers (Convolution, Flatten, Dense)
- Iteratively added:
  - Pooling Layer
  - Batch Normalization
  - More Convolution Layers
  - More Pooling Layers
  - Dropout Layers

### Model Training & Optimization

- **Epochs and Batch Size:** Tested 5, 10, 15, 20 epochs and batch sizes of 32 and 64.
- **Convolution and Pooling Layers:** Increased depth and number of filters, tested MaxPooling, AveragePooling, and GlobalAveragePooling.
- **Dropout Layer & Batch Normalization:** Introduced for regularization and faster training.
- **Activation Functions & Optimizers:** Experimented with ReLU, LeakyReLU, Adam, and SGD optimizers with different learning rates.
- **Early Stopping:** Implemented to prevent overfitting.

### Results

- **Model Performance Metrics:** Achieved 80% accuracy on the test set.
- **Confusion Matrix:** Visualized to identify strengths and weaknesses in classification.
- **Accuracy & Loss Graphs:** Showed training and validation accuracy/loss over epochs.

## Instructions

1. Open the Jupyter Notebook `Assignment_CNN.ipynb` to view and run the code.
2. Review the PowerPoint presentation `CNN_Presentation.pptx` for a summary of the assignment.

## Additional Resources

- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
- [Keras Documentation](https://keras.io/)

