# Topic: Connectionist AI Fundamentals - The Single-Layer Perceptron

## Explanations
**Connectionist AI** models intelligence by simulating networks of simple, interconnected processing units (neurons). Unlike traditional rule-based algorithms that follow explicit "if-then" logic, connectionist models *learn* by adjusting the strengths of connections between units. 

To build a neural network, we rely on fundamental **Data Structures** (like vectors and matrices to hold inputs and weights) and **Algorithms** (like matrix multiplication and activation functions) to process data. 

In this lesson, we will explore the **Single-Layer Perceptron**, the foundational algorithm of connectionist AI. It takes an input data structure (a vector of features), applies an algorithm (a weighted sum and a step function), and outputs a binary decision (e.g., 1 for True, 0 for False).

## Terminology
*   **Perceptron:** The simplest artificial neuron that performs binary classification.
*   **Input Vector (\(X\)):** A data structure (array) containing the features of a single data point. E.g., \(X = [x_1, x_2]\).
*   **Weight Vector (\(W\)):** A data structure containing values that determine the importance of each input. E.g., \(W = [w_1, w_2]\).
*   **Bias (\(b\)):** A constant value added to the weighted sum to shift the decision boundary away from the origin.
*   **Dot Product:** An algorithm that multiplies corresponding elements of two vectors and sums the results: \((x_1 \times w_1) + (x_2 \times w_2)\).
*   **Activation Function:** A mathematical algorithm that decides if the neuron "fires" (outputs 1) or not (outputs 0). For a perceptron, this is a **Step Function**: output 1 if the sum \(\ge 0\), otherwise 0.

## A Worked Example or Demonstration
**Scenario:** We want to predict if a student will pass an exam (1 = Pass, 0 = Fail) based on two inputs: 
1. Hours studied (\(x_1\))
2. Hours slept (\(x_2\))

**Data Structures:**
*   Inputs for Student A: \(X = [5, 6]\) (5 hours studied, 6 hours slept)
*   Weights (learned by the network): \(W = [0.8, 0.4]\) 
*   Bias: \(b = -5.0\)

**Step-by-Step Algorithm:**

*Step 1: Calculate the Weighted Sum (Dot Product + Bias)*
\[
Z = (x_1 \times w_1) + (x_2 \times w_2) + b
\]
\[
Z = (5 \times 0.8) + (6 \times 0.4) + (-5.0)
\]
\[
Z = 4.0 + 2.4 - 5.0
\]
\[
Z = 1.4
\]

*Step 2: Apply the Activation Function (Step Function)*
The rule is: If \(Z \ge 0\), output 1. If \(Z < 0\), output 0.
Since \(Z = 1.4\), which is \(\ge 0\):
\[
Output = 1
\] 
*Prediction:* The student will pass.

## A Meaningful Visual

| Component | Type | Value in Example | Description |
| :--- | :--- | :--- | :--- |
| **Inputs (\(X\))** | Vector | `[5, 6]` | Features of the current data point |
| **Weights (\(W\))** | Vector | `[0.8, 0.4]` | Importance of each feature |
| **Bias (\(b\))** | Scalar | `-5.0` | Shifts the threshold |
| **Sum (\(Z\))** | Algorithm | `1.4` | \((X \cdot W) + b\) |
| **Output** | Step Func | `1` | Final prediction (Pass) |

```text
  x1 (5) --(w1=0.8)--> \
                        \
                         [Sum & Bias] ---> [Step Function] ---> Output (1)
                        /     (1.4)             (1.4 >= 0)
  x2 (6) --(w2=0.4)--> /
