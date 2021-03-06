# Project: Digit Recognition with modified LeNet-5
Apply computer vision fundamentals with the famous MNIST data
Competition website: https://www.kaggle.com/c/digit-recognizer

## Overview
### Description
MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

The project implementation follows LeNet-5 from "Gradient-based learning applied to document recognition" by Y-Lecun with several modifications, and achieved maximum of 99.6% with digit recognition.

### Goal
The goal is to take an image of a handwritten single digit, and determine what that digit is.
For every in the test set, predict the correct label.

### Metric
This project is evaluated on the categorization accuracy of your predictions (the percentage of images you get correct).

## Data
The data files train.csv and test.csv contain gray-scale images of hand-drawn digits, from zero through nine.

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

The training data set, (train.csv), has 785 columns. The first column, called "label", is the digit that was drawn by the user. The rest of the columns contain the pixel-values of the associated image.

Each pixel column in the training set has a name like pixelx, where x is an integer between 0 and 783, inclusive. To locate this pixel on the image, suppose that we have decomposed x as x = i * 28 + j, where i and j are integers between 0 and 27, inclusive. Then pixelx is located on row i and column j of a 28 x 28 matrix, (indexing by zero).

The test data set, (test.csv), is the same as the training set, except that it does not contain the "label" column.
