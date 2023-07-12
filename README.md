# Deep Learning for Gastrointestinal Image Classification
This repository contains code and documentation for an image classification project that involves training deep learning models on the Kvasir dataset v2. Our main objective was to classify images from the gastrointestinal tract into eight different classes.

# Project Overview
The project explores three deep learning models: a baseline model, a modified model, and a transfer learning model, each built using the TensorFlow and Keras libraries in Python.

The dataset was split into training/validation/test sets in a 70:15:15 ratio. Data augmentation techniques were applied to increase the size and variability of the training dataset.

Three convolutional layers, each followed by a max-pooling layer, made up the baseline model. The modified model added a fourth convolutional layer and increased the number of filters in the first layer.

The transfer learning model used MobileNetV2, pre-trained on the ImageNet dataset, as the base model. The top layers of this base model were replaced with custom layers.

# Project Results
Baseline model: Achieved an accuracy of 75.75% after training for 20 epochs.

Modified model: Achieved an improved accuracy of 76.33% after training for 15 epochs.

Transfer learning model: Achieved the highest accuracy of 84.92% after training for 15 epochs.

# Getting Started
Clone the repository to your local machine.

Install the required dependencies listed in the requirements.txt file.

Download and prepare the Kvasir dataset v2.

Run the training scripts for the baseline model, the modified model, and the transfer learning model.

Please refer to the respective Python notebook files for detailed explanations and visualizations of each model.

# Acknowledgements
This project was inspired by the research conducted by Pogorelov et al., 2017 on "Deep learning and hand-crafted feature based approaches for polyp detection in medical videos".

# References
Pogorelov, K., Randel, K. R., Griwodz, C., Eskeland, S. L., de Lange, T., Johansen, D., ... & Riegler, M. (2017, April). Deep learning and hand-crafted feature based approaches for polyp detection in medical videos. In 2017 IEEE 31st International Symposium on Computer-Based Medical Systems (CBMS) (pp. 381-386). IEEE.
