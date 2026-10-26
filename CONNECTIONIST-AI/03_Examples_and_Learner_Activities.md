# Connectionist AI: Examples and Learner Activities


## 1. Learning Objectives

After completing this section, learners should be able to explain how a basic neural network makes predictions, describe how it learns from examples, and identify some of its limitations.

## 2. Worked Example: How Does a Neural Network Make a Prediction?

Imagine a model that classifies messages as **spam** or **not spam**.

The model receives information about a message, such as whether it contains suspicious links or certain words. A neural network processes these inputs and produces a prediction.

```text
 Message features
 (words, links, etc.)
         |
         v
   Input layer
         |
         v
   Hidden layer
         |
         v
   Output layer
         |
         v
  Spam / Not spam
```

This is a simplified representation of a neural network.

The hidden layer helps the model learn patterns from the input. The output layer produces the prediction. During training, the model uses labelled examples to adjust its **weights and biases** — numerical parameters that influence its predictions.

For example, if the model predicts “spam” for a message labelled “not spam,” the training process can adjust its parameters to reduce the error. Repeating this process across many examples can improve its predictions, although it does not guarantee perfect accuracy.

## 3. Learner Activities

Try answering these questions before checking the suggested answers.

### Activity A: Understanding a Prediction

A neural network predicts that a message is spam, but the correct label is “not spam.”

1. What does this tell us about the prediction?
2. What can the model adjust during training?
3. Does one incorrect prediction mean the model is useless?

### Activity B: Understanding Training

A student trains a neural network using hundreds of labelled pictures of cats and dogs.

1. What information does the model receive during training?
2. Why does it need many examples?
3. How could the student check whether the model has learned to classify pictures correctly?

## 4. Answers and Explanations

**Activity A**

1. The prediction does not match the correct label.
2. The training process can update the model's weights and biases to reduce the loss.
3. No. A single mistake does not determine overall performance. The model should be evaluated on a suitable collection of examples, including pictures or messages it has not seen during training.

**Activity B**

1. It receives pictures represented as data, together with their correct labels.
2. Multiple examples help the model learn patterns rather than rely on one specific picture.
3. The student can test the model on separate labelled pictures that were not used for training and compare its predictions with the correct labels.

## 5. Key Takeaways

- Neural networks learn patterns from examples.
- Inputs pass through connected computational units to produce predictions.
- Training adjusts parameters such as weights and biases.
- More training examples do not automatically guarantee better results.
- Testing on unseen data helps us evaluate whether a model can generalize beyond its training examples.

## 6. Resources and References

1. **Google for Developers — Neural Networks**  
   https://developers.google.com/machine-learning/crash-course/neural-networks  
   Introduces neural network components, including nodes, hidden layers, activation functions, and the training process. <Cite refs={["turn266450search2"]}/>

2. **Google for Developers — Machine Learning Crash Course**  
   https://developers.google.com/machine-learning/crash-course/  
   Provides beginner-oriented lessons, visual explanations, and interactive learning activities about machine learning. <Cite refs={["turn266450search0"]}/>

3. **Goodfellow, I., Bengio, Y., and Courville, A. — Deep Learning**  
   https://www.deeplearningbook.org/  
   A more detailed reference for readers who want to explore neural networks and deep learning further. Some chapters require mathematical background. <Cite refs={["turn266450search7"]}/>
