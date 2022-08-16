# Splitting Data

## Intro

Learning objectives:
* Split a training set into a smaller training set and a validation set.
* Analyze deltas between training set and validation set results.
* Test the trained model with a test set to determine whether your trained model is overfitting.
* Detect and fix a common training problem.

## Usage

### Running code cells
You must run code cells in order. In other words, you may only run a code cell once all the code cells preceding it have already been run.

To run a code cell:

1. Place the cursor anywhere inside the [ ] area at the top left of a code cell. The area inside the [ ] will display an arrow.
2. Click the arrow.
Alternatively, you may invoke Runtime->Run all. Note, though, that some of the code cells will fail because not all the coding is complete.

### Why did you see an error?
If a code cell returns an error when you run it, consider two common problems:

1. You didn't run all of the code cells preceding the current code cell.
2. If the code cell is labeled as a Task, then you haven't written the necessary code.

### Use the right version of TensorFlow
The following hidden code cell ensures that the Colab will run on TensorFlow 2.X, which is the most recent version of TensorFlow:
```python 
%tensorflow_version 2.x
```

## Definition

### 0. Data set
* The training set is in california_housing_train.csv.
  * `train_df`, which contains the training set.
  * `test_df`, which contains the test set.
* The test set is in california_housing_test.csv.

### 1. Build and train a model function
* ```build_model```, which defines the model's topography.
* ```train_model```, which will ultimately train the model, outputting not only the loss value for the training set but also the loss value for the validation set.

### 2. Plotting function
* ```plot_the_loss_curve```, function plots loss vs. epochs for both the training set and the validation set.

## Document
Google LLC 2020
