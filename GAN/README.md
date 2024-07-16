# GAN Assignment

This folder contains the assignment on implementing a Generative Adversarial Network (GAN) to generate images from the CIFAR-10 dataset. The objective is to explore the effect of various noise distributions on image generation and to study the modifications made to the generator and discriminator networks.

## Files

- **gan-assignment-devesh-final.ipynb:** Jupyter Notebook with the complete code and analysis.
- **GAN_Presentation.pptx:** PowerPoint presentation summarizing the findings.

## Problem Definition

The CIFAR-10 dataset consists of 60000 32x32 color images in 10 classes, with 6000 images per class. The objective is to implement a GAN to generate images for one class from the CIFAR-10 dataset and explore the effect of the noise vector on image generation.

## Approach and Learnings

### Model Architecture

- **Generator:**
  - Conv2D Transpose layers for upsampling.
  - Dropout layers to prevent overfitting.

- **Discriminator:**
  - Convolutional Layers for feature extraction.
  - Strided convolutions to reduce dimensionality.
  - Dropout layers to prevent overfitting.
  - ZeroPadding to maintain feature dimensions during convolution.

### Training Process

- **Adversarial Training:** The generator and discriminator are trained in an adversarial manner, with the generator aiming to create realistic images and the discriminator aiming to distinguish real from fake images.
- **Minimax Game:** The training process is framed as a minimax game where the generator minimizes and the discriminator maximizes the loss.

### Noise Vector Distributions

- **Normal Distribution:** Generates balanced and naturally varied images.
- **Uniform Distribution:** Produces a wide variety of features, enhancing latent space exploration.
- **Truncated Normal Distribution:** Limits extremes, focusing on more consistent image features.
- **Logistic Distribution:** Introduces pronounced feature variations with heavier tails.
- **Laplace Distribution:** Promotes central feature emphasis with a sharp peak and heavy tails.

### Results

- **Model Performance Metrics:** 
  - Visual inspection of generated images.
  - Effect of different noise vector distributions.
- **Visualization of Results:** 
  - Confusion Matrix
  - Improvement over baseline model: Visualization of generated images for different distributions.
  - Accuracy & Loss Graphs: Show the training and validation accuracy/loss over epochs.

## Instructions

1. Open the Jupyter Notebook `gan-assignment-devesh-final.ipynb` to view and run the code.
2. Review the PowerPoint presentation `GAN_Presentation.pptx` for a summary of the assignment.

## Additional Resources

- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
- [Keras Documentation](https://keras.io/)

