# Handwritten Digit Recognition with PyTorch

**Project Overview**

This project aims to build a neural network model using PyTorch to accurately recognize handwritten digits from the MNIST dataset. The model employs a simple architecture consisting of four linear layers with ReLU activation functions.

**Dataset**

The MNIST dataset, a widely used benchmark for image classification tasks, is utilized. It comprises a training set of 60,000 images and a testing set of 10,000 images, each representing a handwritten digit from 0 to 9.

**Model Architecture**

The neural network architecture is as follows:

1. **Input Layer:** Receives 784-dimensional input (28x28 pixel images flattened).
2. **Hidden Layers:**
   - **Hidden Layer 1:** 256 neurons with ReLU activation.
   - **Hidden Layer 2:** 128 neurons with ReLU activation.
   - **Hidden Layer 3:** 64 neurons with ReLU activation.
   - **Hidden Layer 4:** 32 neurons with ReLU activation.
4. **Output Layer:** 10 neurons (one for each digit class) with softmax activation for probability distribution.

**Training Process**

1. **Data Preprocessing:**
   - Normalize pixel values to the range [0, 1].
   - Convert images to PyTorch tensors.
2. **Model Initialization:**
   - Define the model architecture using PyTorch's `nn.Linear` and `nn.ReLU` modules.
3. **Loss Function and Optimizer:**
   - **Loss Function:** Cross-entropy loss to measure the difference between predicted and actual probabilities.
   - **Optimizer:** Adaptive Moment Estimation(Adam) to update model parameters.
4. **Training Loop:**
   - Iterate over the training dataset in batches.
   - Forward pass: Compute the model's predictions.
   - Backward pass: Calculate the loss and gradients.
   - Update model parameters using the optimizer.
5. **Evaluation:**
   - Evaluate the model's performance on the test dataset using accuracy metrics.

**Getting Started**

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/Severus25/handwritten-digit-recognition](https://github.com/Severus25/handwritten-digit-recognition)
   ```
2. **Install the requirements:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Jupyter Notebook!**
