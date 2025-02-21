# Handwritten Digit Recognition using CNN  

This project trains a Convolutional Neural Network (CNN) using the MNIST dataset to recognize handwritten digits. It also allows users to capture an image from a webcam, preprocess it, and predict the digit using the trained model.  

## Table of Contents  
- [Features](#features)  
- [Requirements](#requirements)  
- [Dataset](#dataset)  
- [Model Architecture](#model-architecture)  
- [Training](#training)  
- [Testing and Evaluation](#testing-and-evaluation)  
- [Webcam Image Capture (Google Colab)](#webcam-image-capture-google-colab)  
- [Prediction](#prediction)  
- [Results](#results)
- [Sample Digit Images](#sample-digit-images) 
- [Acknowledgments](#acknowledgments) 

## Features  
- Loads and preprocesses the MNIST dataset  
- Builds and trains a CNN model using TensorFlow/Keras  
- Captures an image from a webcam (Google Colab)  
- Preprocesses the captured image for prediction  
- Predicts the digit using the trained CNN model  

## Requirements  
This project requires TensorFlow, NumPy, Matplotlib, OpenCV, and PIL (Pillow) for image processing.  

## Dataset  
The model is trained using the MNIST dataset, which consists of 60,000 training images and 10,000 test images of handwritten digits (0-9).  

## Model Architecture  
The CNN model consists of:  
- Convolutional layer with 32 filters of size 3x3 and ReLU activation  
- MaxPooling layer with pool size 2x2  
- Convolutional layer with 64 filters of size 3x3 and ReLU activation  
- MaxPooling layer with pool size 2x2  
- Flatten layer to convert data into a 1D vector  
- Dense layer with 128 neurons and ReLU activation  
- Output Dense layer with 10 neurons and Softmax activation for classification  

## Training  
The model is trained for five epochs using the Adam optimizer and sparse categorical cross-entropy loss function.  

## Testing and Evaluation  
The trained model is evaluated on the test dataset to measure accuracy and loss.  

## Webcam Image Capture (Google Colab)  
The project includes a function to capture an image using a webcam in Google Colab. The captured image is then processed and classified using the trained model.  

## Prediction  
After preprocessing the user-provided image, the model predicts the digit with a probability distribution across all possible digits. The highest probability determines the final predicted digit.  

## Results  
After training, the model achieves high accuracy on the MNIST test dataset. The webcam image is also correctly classified after preprocessing.
![accuaracy](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnistAccuracy.png) 

## Sample Digit Images  
Below are sample images of digits (0-9) from the MNIST dataset:  


| Digit 0  | Digit 1  | Digit 2  |
|----------|----------|----------|
| ![0](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist0.png) | ![1](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist1.png) | ![2](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist2.png) |
| ![00](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist00.png) | ![11](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist11.png) | ![22](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist22.png) |

| Digit 3  | Digit 4  | Digit 5  |
|----------|----------|----------|
| ![3](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist3.png) | ![4](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist4.png) | ![5](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist5.png) |   
| ![33](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist33.png) | ![44](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist44.png) | ![55](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist55.png) |   

| Digit 6  | Digit 7  | Digit 8  |
|----------|----------|----------|
| ![6](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist6.png) | ![7](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist7.png) | ![8](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist8.png) |   
| ![66](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist66.png) | ![77](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist77.png) | ![88](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist88.png) |   

| Digit 9  |          |
|----------|----------|
| ![9](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist9.png) | ![99](https://github.com/DilshanaRanawake/DeepDigits-MNIST-CNN/blob/main/Screenshots/mnist99.png) |


## Acknowledgments  
- TensorFlow/Keras for deep learning  
- OpenCV for image processing  
- Google Colab for execution and webcam access  
