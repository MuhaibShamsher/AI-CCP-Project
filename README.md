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

After downloading: Extract the dataset and structure it as:
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

## How to Run the Project

### Step 1: Clone or Download the Project

```bash
git clone https://github.com/MuhaibShamsher/AI-CCP-Project.git
cd AI-CCP-Project
```

### Step 2: Setup Environment (Anaconda Recommended)

- **Create Environment:**
  ```bash
  conda create -n shape-cnn-env python=3.9
  ```

- **Activate Environment:**
  ```bash
  conda activate shape-cnn-env
  ```

- **Install Dependencies:**
  ```bash
  pip install tensorflow scikit-learn Pillow notebook
  ```

- **Navigate to Your Project Directory:**
  ```bash
  cd "C:\Users\Muhaib Shamsher\OneDrive\Desktop\AI-CCP-Project"
  ```

### Step 3: (Optional) Train the Model

- **Launch Jupyter Notebook:**
  ```bash
  jupyter notebook
  ```

- **In the Jupyter interface, open the file: shape-identifier-cnn.ipynb**

- **Run all the cells to start training the CNN model**

  The training process will generate and save the following files in your project directory:
  - saved_model.h5 — The trained CNN model.
  - class_indices.json — A JSON file mapping shape labels to numerical indices.


### Step 4: Run the GUI
```bash
python shapeIdentifier.py
```

Use the canvas to draw shapes or click Upload to select an image. Click Predict Shape to get results.


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


