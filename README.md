# README

## Project Overview

This project focuses on implementing and evaluating an artificial neural network (ANN) regressor for a dataset containing single input-output pairs. The goal is to learn the ANN's weights using the backpropagation algorithm and analyze the effects of network complexity on model performance. The dataset is provided in two text files: "train1.txt" for training and "test1.txt" for testing.

## Dataset Description

The dataset consists of:
- **Training Set (train1.txt):** Contains 60 examples.
- **Test Set (test1.txt):** Contains 41 examples.
  
Each line in these files represents an example, where the first number is the input and the second number is the output.

## Implementation

The project involves implementing two types of ANN regressors:
1. **Linear Regression (No Hidden Layer):** Serves as a baseline model.
2. **ANN with Single Hidden Layer:** Evaluated with 2, 4, 8, 16, and 32 hidden units.

### Steps:
1. **Data Preparation:** Load training and test data from text files.
2. **Model Training:** Train the models on the training data.
3. **Model Evaluation:** Test the models on unseen data from the test set.
4. **Visualization:** Plot the dataset to analyze model predictions and understand learned patterns.

### Configuration:
- **Learning Rate:** Try different learning rates.
- **Initial Weights:** Experiment with different ranges of initial weights.
- **Epochs:** Use 10,000 epochs for optimal performance.

## Analysis

### Plotting:
For each ANN configuration, plot the training data predictions and visualize curves for uniformly selected input points based on each hidden unit's outputs. Provide a single plot for each ANN.

### Loss Table:
Prepare a table reporting the training and test set losses. For each network, report:
- **Training Loss:** Averaged over the training set instances and its standard deviation.
- **Test Loss:** Averaged over the test set instances and its standard deviation.

### Observations:
1. **Complexity and Performance:** Increasing hidden units generally improves model performance on training data.
2. **Overfitting Risk:** Higher complexity models might overfit, leading to higher test loss despite lower training loss.
3. **Underfitting Risk:** Models with too few hidden units may underfit, failing to capture data patterns.
4. **Optimal Configuration:** The best results were obtained with 32 hidden units, a learning rate of 0.001, normalized inputs, and 10,000 epochs.
5. **Visualization Insight:** Plotting helps in understanding how well the model generalizes from training to test data.

## Conclusion

This project demonstrates the implementation and evaluation of ANN regressors on a simple dataset. By exploring different network complexities, learning rates, and initial weight ranges, we identify the optimal configuration for achieving the best performance. The results underscore the importance of balancing model complexity to avoid underfitting and overfitting, thereby ensuring robust performance on both training and unseen test data.

Contributions and feedback are welcome to further enhance the functionality and usability of the ANN models explored in this project. Thank you for your interest and support!
