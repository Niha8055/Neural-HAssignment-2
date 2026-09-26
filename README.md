# CS5720 Neural Network and Deep Learning
## Home Assignment 2

### Student Information
- **Name:** Niharika
- **Course:** CS5720 Neural Network and Deep Learning
- **Semester:** Fall 2026
- **University:** University of Central Missouri

## Assignment Overview

This repository contains the implementation of Home Assignment 2 for CS5720 Neural Network and Deep Learning. The assignment covers Recurrent Neural Networks (RNNs), LSTM models, convolution operations, edge detection, pooling, AlexNet, and ResNet architectures.

## Q1: RNN for Text Generation

Implemented a character-level LSTM-based Recurrent Neural Network for text generation using the Shakespeare text dataset.

The implementation includes:
- Loading and preprocessing the text dataset
- Character-level encoding
- Creating training sequences
- Building an LSTM model
- Training the model
- Generating text character by character
- Testing different temperature values: 0.5, 1.0, and 1.5

Temperature scaling controls the randomness of generated text. Lower temperatures produce more predictable output, while higher temperatures increase randomness and diversity.

## Q2: Sentiment Classification Using RNN

Implemented an LSTM-based sentiment classification model using the IMDB movie review dataset.

The implementation includes:
- Loading the IMDB dataset
- Padding review sequences
- Building an Embedding + LSTM model
- Training the model
- Evaluating test accuracy
- Generating a confusion matrix
- Generating a classification report with precision, recall, and F1-score

The precision-recall tradeoff is important because improving one metric can sometimes reduce the other depending on the classification threshold.

## Q3: Convolution Operations with Different Parameters

Performed convolution on the provided 5x5 input matrix using the provided 3x3 kernel.

The following configurations were tested:
- Stride = 1, Padding = VALID
- Stride = 1, Padding = SAME
- Stride = 2, Padding = VALID
- Stride = 2, Padding = SAME

The resulting feature maps were printed for comparison.

## Q4: CNN Feature Extraction with Filters and Pooling

### Sobel Edge Detection

Applied the provided Sobel-X and Sobel-Y filters to a grayscale sample image.

The following images were displayed:
- Original grayscale image
- Edge detection using Sobel-X
- Edge detection using Sobel-Y

### Pooling Operations

Created a random 4x4 matrix and applied:
- 2x2 Max Pooling
- 2x2 Average Pooling

The original matrix, max-pooled matrix, and average-pooled matrix were printed.

## Q5: Implementing and Comparing CNN Architectures

### AlexNet

Implemented a simplified AlexNet architecture containing:
- Five convolutional layers
- Three max-pooling layers
- Two fully connected layers with 4096 neurons
- Dropout layers with a rate of 0.5
- Softmax output layer with 10 classes

The model summary was generated to display the architecture and parameters.

### ResNet

Implemented a simple ResNet-like architecture using residual blocks.

Each residual block contains:
- Two 3x3 convolutional layers
- A skip connection
- Addition of the input to the convolution output

The final model contains two residual blocks followed by a Flatten layer, Dense layer with 128 neurons, and a Softmax output layer.

## Technologies Used

- Python
- Jupyter Notebook
- TensorFlow / Keras
- NumPy
- OpenCV
- Matplotlib
- Scikit-learn

## Source Code

The complete implementation for Questions 1–5 is available in:

`Neural HAssignment-2.ipynb`

## How to Run

1. Download or clone this repository.
2. Open `Neural HAssignment-2.ipynb` using Jupyter Notebook.
3. Install the required Python libraries if necessary.
4. Run the notebook cells sequentially from top to bottom.
5. Review the generated outputs, plots, evaluation results, and model summaries.
