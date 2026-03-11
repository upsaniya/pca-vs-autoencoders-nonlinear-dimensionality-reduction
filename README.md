# pca-vs-autoencoders-nonlinear-dimensionality-reduction

__I. Datasets__

MNIST Dataset
(Kaggle link: https://www.kaggle.com/datasets/oddrationale/mnist-in-csv)

Handwritten digit dataset containing grayscale images of digits (0-9).

Images: 28 × 28 pixels
Features after flattening: 784

Training samples: 60,000
Test samples: 10,000

Dataset files used:
mnist_train.csv
mnist_test.csv

__II. Data Preprocessing__

Load dataset using Pandas.
Separate labels and features.
Normalize pixel values from 0–255 to 0–1.
Split into training and testing sets.

__III. Methods Implemented__
1. Principal Component Analysis (PCA)
   Steps:
   Compute covariance matrix
   Perform eigenvalue decomposition
   Select top principal components
   Project data into reduced feature space
   Reconstruct original data

3. Deep Autoencoder
   Optimizer: Adam
   Loss function: Mean Squared Error (MSE)
   Framework: TensorFlow / Keras

__IV. Evaluation Metrics__
1. Reconstruction Error
Measures how accurately the original image can be reconstructed.
Metric used: Mean Squared Error (MSE)
2. Visualization
Reconstructed images are compared visually with the original images.

__V. Outcome__

The project demonstrates that:

PCA performs well for linear data structures.
Autoencoders capture nonlinear patterns more effectively.
Deep learning methods can provide better feature representations for complex data.
