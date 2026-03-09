# Deep-Learning-for-Skin-Lesion-Classification-using-the-HAM10000-Dataset
Deep learning model for classifying seven types of skin lesions using the HAM10000 dermoscopy dataset with a custom CNN built in PyTorch.
Skin Lesion Classification using Deep Learning (HAM10000)

This project implements a convolutional neural network in PyTorch to classify dermoscopy images into seven different skin lesion categories using the HAM10000 dermatology dataset.

The goal is to explore how deep learning models learn patterns in medical images while addressing real challenges such as class imbalance, dataset variability, and model evaluation.

Dataset

HAM10000 skin lesion dataset (~10,000 dermoscopy images)

Classes detected:

Melanocytic Nevi

Melanoma

Benign Keratosis

Basal Cell Carcinoma

Actinic Keratosis

Vascular Lesions

Dermatofibroma

Model

Custom CNN architecture with:

Convolution blocks + Batch Normalization

ReLU activation

Max Pooling

Global Average Pooling

Fully connected classification head

Training Techniques

Data augmentation (rotation, flips, color jitter)

Class weighted cross entropy to handle dataset imbalance

Cosine annealing learning rate scheduler

Results

Best validation accuracy: 61.6%

Evaluation includes:

Confusion matrix

Training vs validation accuracy curves

Classification report

Technologies

Python
PyTorch
Torchvision
HuggingFace Datasets
NumPy
Pandas
Matplotlib
Seaborn
OpenCV
