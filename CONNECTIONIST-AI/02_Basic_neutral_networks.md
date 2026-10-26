# Basic Neural Network and How Neural Network Learns

**Group Project – Algorithms, Data Structures & Connectionist AI**

---

## 1. Introduction

A neural network is a computational model inspired by the structure and function of biological brains. It consists of many simple processing units called neurons that are connected together by weighted links. By adjusting the strength of these connections, the network can learn patterns from data and make useful predictions.

Neural networks belong to the field of Connectionist AI. Unlike traditional rule-based systems, connectionist models learn directly from examples instead of following hand-written rules.

This document explains the basic structure of a neural network and the complete process by which a neural network learns.

---

## 2. Basic Building Blocks

### 2.1 Neuron (Node)

A neuron is the fundamental unit of a neural network. It receives one or more input values, multiplies each input by a weight, adds a bias, and then applies an activation function to produce an output.

The basic computation inside a neuron is:

**z = (w₁ × x₁) + (w₂ × x₂) + … + (wₙ × xₙ) + b**  
**a = f(z)**

Where:
- x = inputs
- w = weights
- b = bias
- f = activation function
- a = output of the neuron

### 2.2 Weight

A weight is a numerical value that determines how important a particular input is to a neuron.  
- A large positive weight means the input strongly increases the neuron’s activation.  
- A large negative weight means the input strongly decreases the neuron’s activation.  
- A weight close to zero means the input has almost no influence.

During learning, the network continuously changes the weights so that the final predictions become more accurate.

### 2.3 Bias

A bias is an extra parameter added to the weighted sum. It allows a neuron to activate even when all of its inputs are zero. The bias shifts the activation threshold of the neuron and gives the model more flexibility.

### 2.4 Activation Function

An activation function introduces non-linearity into the network. Without activation functions, stacking many layers would still result in only a linear model.

Common activation functions:

- **Sigmoid**: outputs a value between 0 and 1 (useful for probabilities)
- **Tanh**: outputs a value between -1 and 1
- **ReLU**: outputs the input if it is positive, otherwise outputs zero

The sigmoid function is often used in educational examples because its derivative is simple.

---

## 3. Structure of a Neural Network

A basic neural network is organized into layers:

### 3.1 Input Layer
The input layer receives the raw data. It does not perform any calculation; it only holds the feature values and passes them to the next layer.

### 3.2 Hidden Layer(s)
Hidden layers sit between the input layer and the output layer. They create internal representations of the data. Even one hidden layer greatly increases the power of the network.

### 3.3 Output Layer
The output layer produces the final prediction of the network.  
- For binary classification it usually has one neuron.  
- For multi-class classification it has one neuron per class.

Networks with one or more hidden layers are called Multi-Layer Perceptrons (MLPs).

---

## 4. How a Neural Network Learns

Learning means adjusting the weights and biases so that the network’s predictions become closer to the correct answers. The learning process consists of four repeated steps.

### 4.1 Forward Propagation

In forward propagation the input data is passed through every layer of the network:

1. Each neuron computes the weighted sum of its inputs plus the bias.
2. The activation function is applied.
3. The result is sent to the next layer.
4. The final layer produces the prediction.

Forward propagation only generates a prediction; it does not change any weights.

### 4.2 Loss Function

After the prediction is made, a loss function measures how wrong the prediction is.  
A common loss function for binary classification is Binary Cross-Entropy.

The goal of training is to make the loss as small as possible.

### 4.3 Backpropagation

Backpropagation is the algorithm that calculates how much each weight and each bias contributed to the final error. It works by sending the error signal backwards from the output layer to the earlier layers using the chain rule of calculus.

For every weight the algorithm computes a gradient (a number that shows the direction and size of the needed change).

### 4.4 Gradient Descent

Once the gradients are known, Gradient Descent updates the parameters:

**new weight = old weight − learning_rate × gradient**

The learning rate is a small positive number that controls the size of each update.  
This process is repeated for many epochs (complete passes through the training data).

---

## 5. Complete Learning Cycle

The network learns by repeating the following cycle thousands of times:

1. Forward Propagation → produce a prediction  
2. Calculate the Loss → measure the error  
3. Backpropagation → calculate the gradient of every weight and bias  
4. Gradient Descent → update the weights and biases  

After many cycles the loss becomes very small and the network has learned the pattern in the data.

---

## 6. Why Hidden Layers Are Necessary

A network with only an input layer and an output layer can only solve linearly separable problems. Many important problems (such as the XOR function) are not linearly separable.

When a hidden layer is added, the network can create new internal features. These new features make the problem linearly separable in the transformed space. This is why hidden layers are essential for solving complex tasks.

---

## 7. Summary

A basic neural network learns through the continuous adjustment of weights and biases.  

- Forward propagation generates predictions.  
- The loss function measures the error.  
- Backpropagation calculates how each parameter should change.  
- Gradient descent actually changes the parameters.  

By repeating this process, the network gradually improves its performance and discovers useful patterns in the data. This mechanism is the foundation of modern Connectionist AI and deep learning.

---

**End of Document**
