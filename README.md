# Shape Identifier Using Convolutional Neural Network (CNN)

A GUI-based machine learning project that allows users to **draw or upload geometric shapes**, and the system will classify the shape using a pre-trained CNN model.


## Project Overview

This project implements a deep learning model trained on a **geometric shape dataset** to classify 8 different shapes. It also provides a user-friendly **Tkinter-based GUI** for interaction.


## Shapes Supported

The model currently supports the following 8 geometric shapes:

- Circle
- Kite
- Parallelogram
- Rectangle
- Rhombus
- Square
- Trapezoid
- Triangle


## Dataset

We use the **Geometric Shapes Mathematics** dataset available on Kaggle: [Download Dataset from Kaggle](https://www.kaggle.com/datasets/reevald/geometric-shapes-mathematics?resource=download)

After downloading:
- Extract the dataset and structure it as:

```plaintext
/dataset/
├── train/
├── test/
└── val/
```


## Project Structure
```plaintext
/shape-identifier-cnn
├── dataset/ # Geometric shapes dataset
├── shape-identifier-cnn.ipynb # Training notebook
├── shapeIdentifier.py # GUI + Prediction
├── saved_model.h5 # Trained CNN model
├── class_indices.json # Class labels to index mapping
├── requirements.txt # Dependencies
└── README.md # Project documentation
```


## Tools and Technologies

| Component       | Details                          |
|-----------------|----------------------------------|
| Language        | Python 3.x                       |
| ML Framework    | TensorFlow + Keras               |
| GUI Framework   | Tkinter                          |
| Libraries       | PIL, NumPy, matplotlib, json, os |
| IDE             | Jupyter Notebook, VS Code        |


## Features

- CNN model for image classification.
- Train/Validation/Test split support.
- GUI to draw or upload shapes.
- Real-time shape prediction using the trained model.
- Dataset-driven training and predictions.


