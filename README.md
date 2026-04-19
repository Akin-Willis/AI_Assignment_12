## Overview
This project trains a simple feedforward neural network (ANN) using TensorFlow/Keras to classify images from **Fashion-MNIST** into **10 clothing categories**. The notebook includes data preprocessing, model building (Flatten + Dense layers), training, evaluation, and confusion matrix visualization.

## Dataset
Uses `tf.keras.datasets.fashion_mnist` (grayscale images, 28×28 pixels). Class labels:
T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot.

## How to Run (Google Colab)
1. Open the notebook in Google Colab.
2. Run cells in order (the dataset is downloaded automatically by Keras).
3. Train the model and view:
   - training/validation performance
   - test accuracy and macro metrics
   - confusion matrix

## Outputs
- Test Accuracy (~0.88 in the current run)
- Macro Precision, Recall, F1-score
- Confusion Matrix plot
- Model training history (loss/accuracy trends)

## Notes
The key preprocessing steps are:
- normalize images to 0–1
- one-hot encode labels
The ANN uses softmax + categorical crossentropy for multi-class classification.
