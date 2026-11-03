# Basic Neural Networks and How They Learn

**Group Project – Algorithms, Data Structures & Connectionist AI**

---

## 1. Introduction

A neural network is a computational model loosely inspired by the way biological brains process information. It consists of connected processing units called **neurons**. These neurons work together to identify patterns in data and produce predictions.

Neural networks belong to the field of Connectionist AI. Unlike traditional rule-based systems, which follow rules written by humans, neural networks learn patterns by using examples and adjusting their internal values.

This document introduces the basic structure of a neural network and explains how it learns.

---

## 2. Basic Building Blocks

### 2.1 Neuron (Node)

A neuron is one of the basic processing units in a neural network. It receives input values, multiplies each input by a weight, adds a bias, and applies an activation function to calculate an output.

The basic calculation is:

**z = (w₁ × x₁) + (w₂ × x₂) + … + (wₙ × xₙ) + b**

**a = f(z)**

Where:

- **x** = input values
- **w** = weights that determine the influence of each input
- **b** = bias, an additional value used in the calculation
- **f** = activation function
- **z** = weighted sum of the inputs plus the bias
- **a** = final output of the neuron

In simple terms, a neuron combines information from its inputs and produces a result for the next part of the network.

### 2.2 Weight

A weight is a numerical value that determines how strongly an input influences a neuron.

- A larger positive or negative weight generally means a stronger influence.
- A weight close to zero means the input has less influence.
- The direction of the influence also depends on the input value and the other parts of the calculation.

During training, the network adjusts its weights to improve its predictions.

### 2.3 Bias

A bias is an additional value added to the weighted sum of a neuron's inputs. It gives the neuron more flexibility by shifting the value passed to the activation function.

This means the neuron does not rely only on its input values when producing an output.

### 2.4 Activation Function

An activation function determines the output of a neuron after the weighted sum and bias have been calculated.

It introduces **non-linearity**, which allows a neural network to learn more complex patterns. Without non-linear activation functions, a network made of multiple layers would still behave like a linear model.

Common activation functions include:

- **Sigmoid:** Produces an output between 0 and 1. It is often used in the output layer of binary classification networks. However, its output is not automatically a reliable probability.
- **Tanh:** Produces an output between -1 and 1.
- **ReLU (Rectified Linear Unit):** Returns the input if it is positive and returns zero otherwise.

---

## 3. Structure of a Neural Network

A basic feedforward neural network is organized into layers. Information moves from the input layer towards the output layer.

### 3.1 Input Layer

The input layer receives the data and passes its values to the next layer.

For example, in a system that recognizes handwritten numbers, the input could be the pixel values of an image.

### 3.2 Hidden Layer(s)

Hidden layers are located between the input and output layers. They process information and help the network identify patterns and relationships in the data.

A network can have one or more hidden layers. More layers can help a network learn more complex patterns, although adding layers does not always improve its performance.

### 3.3 Output Layer

The output layer produces the network's final result or prediction.

- **Binary classification:** Often uses one output neuron to predict between two categories.
- **Multi-class classification:** Commonly uses one output neuron for each possible category.

For example, a network that recognizes handwritten digits from 0 to 9 may have ten output neurons, one for each digit.

A basic feedforward network with input, hidden, and output layers is commonly called a **Multi-Layer Perceptron (MLP)**.

---

## 4. How a Neural Network Learns

Learning means adjusting the network's weights and biases so that its predictions become closer to the correct answers.

The process involves four main steps that are repeated during training.

### 4.1 Forward Propagation

Forward propagation is the process of passing input data through the network to produce a prediction.

The steps are:

1. The input data enters the input layer.
2. Each neuron calculates the weighted sum of its inputs and adds its bias.
3. An activation function is applied.
4. The result passes to the next layer.
5. The output layer produces the final prediction.

Forward propagation produces a prediction but does not update the network's weights or biases.

### 4.2 Loss Function

A loss function measures how different the network's prediction is from the correct answer.

- A **lower loss** generally means the prediction is closer to the correct answer.
- A **higher loss** means the prediction is further from the correct answer.

For example, Binary Cross-Entropy is a loss function commonly used for binary classification. At a beginner level, it is enough to understand that a loss function measures prediction error.

The goal of training is to reduce the loss.

### 4.3 Backpropagation

Backpropagation is a process that calculates how the network's weights and biases affect the loss.

It works backwards from the output layer towards the earlier layers. This helps the network determine how its internal values should be adjusted to reduce prediction errors.

Backpropagation calculates values called **gradients**. A gradient indicates how a small change in a weight or bias would affect the loss.

### 4.4 Gradient Descent

Gradient Descent is an optimization method that uses the gradients calculated during backpropagation to update the network's weights and biases.

A simplified weight update formula is:

**New weight = Old weight − (Learning rate × Gradient)**

Where:

- **Learning rate** = controls the size of each adjustment.
- **Gradient** = indicates how changing the weight affects the loss.

A learning rate that is too large may cause the network to make unstable updates, while one that is too small may make learning very slow.

The network repeats these updates during training to reduce its loss.

---

## 5. The Complete Learning Cycle

A neural network learns by repeating the following process:

1. **Forward Propagation:** Produce a prediction from the input data.
2. **Calculate the Loss:** Measure the difference between the prediction and the correct answer.
3. **Backpropagation:** Calculate gradients to understand how the weights and biases affect the loss.
4. **Gradient Descent:** Use the gradients to update the weights and biases.

One complete pass through the training dataset is called an **epoch**. Training usually involves multiple epochs.

The aim is to reduce the loss and improve the network's predictions over repeated training steps. However, training does not guarantee that the loss will become zero or that every prediction will be correct.

---

## 6. Why Hidden Layers and Activation Functions Matter

A network without hidden layers and non-linear activation functions can only learn simple linear relationships.

Some problems involve more complex patterns that cannot be separated using a straight line. The XOR problem is a common example.

Hidden layers allow the network to create and combine internal representations of the input data. Non-linear activation functions help these layers learn more complex relationships.

However, not every task requires hidden layers. The structure of a network depends on the problem it is designed to solve.

---

## 7. Summary

A neural network learns by adjusting its weights and biases through repeated training.

- **Neurons** process input values and produce outputs.
- **Weights and biases** influence the calculations within the network.
- **Activation functions** help the network learn complex patterns.
- **Forward propagation** produces predictions.
- **Loss functions** measure prediction errors.
- **Backpropagation** calculates gradients.
- **Gradient descent** updates the network's parameters.

By repeating this learning process, a neural network can improve its predictions and identify useful patterns in data. This process is one of the foundations of Connectionist AI and deep learning.

---

**End of Document******
