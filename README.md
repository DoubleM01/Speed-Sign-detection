# Speed-Sign-detection

This repository hosts a deep learning project aimed at detecting and classifying speed limit signs from images. Leveraging TensorFlow and Keras, the project trains a Convolutional Neural Network (CNN) to recognize different speed limits, making it useful for applications such as autonomous vehicles and traffic monitoring systems.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Model Architecture](#model-architecture)
- [Result samples](#result-samples)

## Introduction

The Speed Sign Detection project involves building a CNN model to classify speed limit signs from images. The project processes a dataset of speed sign images, trains a model, evaluates its performance, and makes predictions on new images. The model can distinguish between various speed limits and provide real-time feedback for applications like autonomous driving.

## Installation

To set up this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/DoubleM01/speed-sign-detection.git
   cd speed-sign-detection
   ```
2. **Install the required dependencies**
     ```bash
     pip install -r requirements.txt
     ```
3. **Prepare the Dataset:**
   
     By following this [link](archive/dataset.md)

## Model Architecture
The CNN model used for speed sign detection is composed of the following layers:

### Input Layer:

* Input shape: (128, 128, 3) (128x128 RGB images)
### Convolutional Layer 1:

* Filters: 32
* Kernel size: (3, 3)
* Activation: ReLU
* MaxPooling: (2, 2)
* Dropout: 0.25
### Convolutional Layer 2:

* Filters: 64
* Kernel size: (3, 3)
* Activation: ReLU
* MaxPooling: (2, 2)
* Dropout: 0.25
### Flatten Layer:

* Flattens the input from previous layers into a single vector.
### Dense Layer 1:

* Units: 64
* Activation: ReLU
### Output Layer:

* Units: 8 (corresponding to 8 different speed limit classes)
* Activation: Softmax (for multiclass classification)


## Result samples
![image](https://github.com/user-attachments/assets/02aa1abe-0ff1-41ce-9f69-52f3b1a2233a)
