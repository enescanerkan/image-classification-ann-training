# Fish Classification Using ANN

This project is focused on classifying different fish species using Artificial Neural Networks (ANN). The model is trained on images of 18 different fish species and aims to accurately identify the species from the input image.

## KAGGLE LINK:
https://www.kaggle.com/code/enescanerkan1/fish-classification


## Dataset

- **Dataset**: A Large Scale Fish Dataset (18 classes, 18,000 images)
- **Classes**: Horse Mackerel, Red Sea Bream, Gilt-Head Bream, Shrimp, Striped Red Mullet, Trout, Sea Bass, Black Sea Sprat, and others.
- **Format**: Images in `.png` format.

## Data Augmentation

To enhance the model's performance and reduce overfitting, data augmentation techniques have been applied to the training and validation images. The following transformations have been utilized:

Image Transformations:
Images are rotated 90 degrees to the right and left. These transformations help the model understand images from different angles.

## Applied Transformations
Rotation to the Right: Images are rotated 90 degrees to the right, creating new files.
Rotation to the Left: Images are rotated 90 degrees to the left, creating new files.
These data augmentation processes help the model generalize better by exposing it to a wider variety of image conditions.

## Model Architecture

- **Model Type**: ANN (Artificial Neural Network)
- **Input**: 28x28x3 images (color images resized to 28x28 pixels)
- **Hidden Layers**:
  - Dense (512 units) with ReLU activation and Dropout (0.3)
  - Dense (256 units) with ReLU activation and Dropout (0.3)
  - Dense (128 units) with ReLU activation and Dropout (0.3)
- **Output Layer**: 18 classes (using softmax activation)
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Metrics**: Accuracy

## How to Run the Project

### 1. Clone the Repository
To run the project locally, clone the repository using:

```bash
git clone https://github.com/enescanerkan/ANN_Training.git

