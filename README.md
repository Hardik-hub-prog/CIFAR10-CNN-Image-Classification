# CIFAR10-CNN-Image-Classification
This project implements a Convolutional Neural Network (CNN) for image classification using the classic CIFAR-10 dataset. The model learns visual patterns from RGB images and classifies them into 10 different object categories. ReLU activation function and max pooling operation followed by fully connected output layer for multiclass classification.

he CNN architecture consists of three convolutional blocks with 32, 64, and 128 filters, respectively. Each block uses a convolutional layer, ReLU activation, and max pooling, followed by a fully connected output layer for multi-class classification.

The model achieved 75% test accuracy after training for 10 epochs using PyTorch.

🎯 Project Objectives

Understand the fundamentals of Computer Vision and CNN architecture.
Extract spatial features from images using convolutional layers.
Apply ReLU activation and max pooling.
Build a deep learning model for multi-class image classification.
Train and evaluate a CNN using PyTorch.

📊 Dataset: CIFAR-10

The CIFAR-10 dataset contains 60,000 color images distributed across 10 classes.

Dataset Property

Total Images - 60,000
Training Images -50,000
Testing Images -10,000
Image Dimensions - 32 × 32 pixels
Image Channels - 3 (RGB)
Number of Classes - 10

CIFAR-10 Classes - Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, and Truck.

Architecture Flow:

Input Image → Conv2D (32) → ReLU → MaxPool2D → Conv2D (64) → ReLU → MaxPool2D → Conv2D (128) → ReLU → MaxPool2D → Flatten → Fully Connected Layer → 10 Class Scores

Key Components

Convolutional Layers: Extract image features such as edges, textures, and shapes using learnable filters.
ReLU Activation: Introduces non-linearity into the network.
Max Pooling: Reduces spatial dimensions while retaining prominent features.
Flatten: Converts the extracted feature maps into a one-dimensional vector.
Fully Connected Layer: Maps extracted features to scores for the 10 classes.
Cross-Entropy Loss: Measures the difference between predicted class scores and the actual labels.
Adam Optimizer: Updates model parameters during training to minimize the loss.

⚙️ Model Training Configuration

Hyperparameter

Value

Deep Learning Framework - PyTorch
Loss Function - CrossEntropyLoss
Optimizer - Adam
Batch Size - 64
Number of Epochs - 10
Convolutional Layers -3
Filter Sizes - 32, 64, 128
Convolution Kernel Size - 3 × 3
Max Pooling Kernel Size - 2 × 2

The trained CNN achieved the following result:
Evaluation Metric

Result
Test Accuracy - 75%
Total Test Images - 10,000
Correct Predictions - Approximately 7,500

The model demonstrates its ability to learn useful visual features and classify images into the 10 CIFAR-10 categories.

🔄 Project Workflow

Load the CIFAR-10 dataset using Torchvision.
Preprocess the images and prepare data loaders.
Define the CNN architecture with three convolutional blocks.
Configure CrossEntropyLoss and the Adam optimizer.
Train the model for 10 epochs using batches of 64 images.
Evaluate the model on the test dataset.
Calculate and report test accuracy.


🛠️ Technologies Used

Pyhon , PyTorch ,Torchvision , NumPy, Scikit-learn

💡 Key Learnings

Understanding the architecture and working principles of CNNs.
Learning hierarchical feature extraction through convolutional layers.
Implementing ReLU activation and max pooling.
Training neural networks using CrossEntropyLoss and the Adam optimizer.
Evaluating a multi-class image classification model.
Applying deep learning concepts to a standard Computer Vision dataset.

👨‍💻 Author
Hardik Jain
Building hands-on projects in Machine Learning, Deep Learning, and Computer Vision.
