# MNIST Handwritten Digit Classifier Using LeNet-5
A deep learning project implementing LeNet-5 architecture to classify handwritten digits using the MNIST dataset.

## Overview
This project builds and trains a Convolutional Neural Network (CNN) based on the LeNet-5 architecture on the MNIST dataset.

## Model Architecture
Model: "sequential_1"
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┓
┃ Layer (type)                         ┃ Output Shape                ┃         Param # ┃
┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━┩
│ conv2d_8 (Conv2D)                    │ (None, 28, 28, 6)           │             156 │
├──────────────────────────────────────┼─────────────────────────────┼─────────────────┤
│ average_pooling2d_6                  │ (None, 14, 14, 6)           │               0 │
│ (AveragePooling2D)                   │                             │                 │
├──────────────────────────────────────┼─────────────────────────────┼─────────────────┤
│ conv2d_9 (Conv2D)                    │ (None, 10, 10, 16)          │           2,416 │
├──────────────────────────────────────┼─────────────────────────────┼─────────────────┤
│ average_pooling2d_7                  │ (None, 5, 5, 16)            │               0 │
│ (AveragePooling2D)                   │                             │                 │
├──────────────────────────────────────┼─────────────────────────────┼─────────────────┤
│ conv2d_10 (Conv2D)                   │ (None, 1, 1, 120)           │          48,120 │
├──────────────────────────────────────┼─────────────────────────────┼─────────────────┤
│ flatten_2 (Flatten)                  │ (None, 120)                 │               0 │
├──────────────────────────────────────┼─────────────────────────────┼─────────────────┤
│ dense_3 (Dense)                      │ (None, 84)                  │          10,164 │
├──────────────────────────────────────┼─────────────────────────────┼─────────────────┤
│ dense_4 (Dense)                      │ (None, 10)                  │             850 │
└──────────────────────────────────────┴─────────────────────────────┴─────────────────┘
 Total params: 61,706 (241.04 KB)
 Trainable params: 61,706 (241.04 KB)
 Non-trainable params: 0 (0.00 B)
 
## Files
- **mnist_lenet5.ipynb**: Main notebook containing the code.
- **requirements.txt**: List of dependencies.

## Results
Achieved 98.6% accuracy on the test dataset.

## How to Run
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Open `leNet5_implementation.ipynb` in Jupyter Notebook or run it on [Google Colab](https://colab.research.google.com/drive/1EJNnzgvwAiCwQeJYG5-vywu1UGTMMunY?usp=sharing).

![image](https://github.com/user-attachments/assets/3fa05287-ff89-4e12-99c4-5caa3e2bc197)

