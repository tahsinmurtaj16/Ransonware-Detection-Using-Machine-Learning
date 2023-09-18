# Ransonware Detection Using Machine Learning
## Overview 
This project focuses on developing a machine learning solution for the detection of ransomware attacks. Ransomware is a significant cybersecurity threat that can have severe consequences for individuals and organizations. Detecting ransomware early is crucial for minimizing the damage it can cause.

In this project, we employ various machine learning techniques, including Random Forest, Support Vector Machine (SVM), and Convolutional Neural Network (CNN), to build models that can identify ransomware activity in network traffic data. We also perform feature selection, data preprocessing, and evaluation to ensure the models' effectiveness.
## Dataset
The dataset used in this project contains network traffic data, including features such as source and destination IPs, ports, packet lengths, and protocol types. The target variable is the "Label," which indicates whether the network traffic is benign or associated with specific types of ransomware.
## Methodology
### Data Preprocessing
* Label Encoding: We encode the target variable into numerical values for model training.
* Feature Selection: We identify the most relevant features for model building using correlation analysis.
* Data Splitting: The dataset is split into training and testing sets (typically 70%:30%).
* Model Training: We train machine learning models using the selected features.
## Model Types
1. Random Forest:

Parameters: We tune hyperparameters such as the number of trees and maximum depth for optimal performance.
Evaluation: We calculate metrics like accuracy, precision, recall, and F1-score.

2. Support Vector Machine (SVM):

Parameters: We experiment with different kernel functions and regularization parameters.
Evaluation: We assess model performance using standard classification metrics.

3. Convolutional Neural Network (CNN):

Architecture: We construct a CNN model suitable for tabular data.
Training: We train the model using network traffic features.
Evaluation: We measure the model's accuracy, precision, recall, and F1-score.

## Binary Classification
To simplify the problem, we perform binary classification, where "Benign" traffic is assigned to class 0, and all other types are grouped as class 1 (indicating ransomware activity).

## Results
We present the performance metrics and evaluation results for each model, allowing you to understand how well they identify ransomware attacks in network traffic data.

## Usage
You can use the provided code and models to detect ransomware activity in your network traffic data. Feel free to experiment with different datasets or further optimize the models for your specific use case.

Dependencies
Python
Scikit-Learn
TensorFlow/Keras (for CNN)
Other libraries as specified in the code

## License
```txt
MIT License

Copyright (c) 2023 tahsinMurtaj16

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE. 
   
