# Creating Multi Task Models With Keras

A multi-output CNN using **Keras** to classify handwritten **digits** and their **colors** from a modified MNIST dataset. This project demonstrates **multi-task learning**, data generation, training, visualization, and model evaluation.

---

## Table of Contents

- [Overview]
- [Features]
- [Installation]
- [Usage] 
- [Dataset] 
- [Model Architecture] 
- [Visualizations] 
- [Results] 

---

## Overview

This project builds a **multi-output CNN** that predicts both **digit classes (0-9)** and **color channels (red/green)**. The network uses convolutional layers, skip connections, and two separate output heads for **simultaneous learning**. It also provides **visual insights** into training performance with loss and accuracy plots, as well as confusion matrices.

---

## Features

- Multi-output CNN for digits and colors  
- Custom data generation with colored MNIST images  
- Training with **Keras** and **TensorFlow**  
- Epoch-wise metrics logging with a custom callback  
- Visualization using **Matplotlib** and **Seaborn**  
- Confusion matrix analysis for digit classification  
- Sample predictions for qualitative evaluation  

---

## Model Architecture

- **Input:** 28x28x3 RGB image  
- **Layers:** Conv2D + MaxPooling layers  
- **Skip connections:** ResNet-style  
- **Outputs:** Flatten → Dense layers for  
  - Digit (softmax)  
  - Color (sigmoid)  
- **Loss functions:**  
  - Digit: `sparse_categorical_crossentropy`  
  - Color: `binary_crossentropy`  
- **Metrics:**  
  - Digit: `SparseCategoricalAccuracy`  
  - Color: `BinaryAccuracy`  

---

## Visualizations

- Training & validation **loss curves**  
- Digit and color **accuracy curves**  
- Confusion matrix for **digit classification**  
- Sample predictions with **color-coded correctness**  

---

## Results

- High accuracy on both **digit** and **color** classification  
- Confusion matrices indicate **precise predictions** for most digits  
- Visual inspection confirms **robust model performance** on colored MNIST samples

## 👤 Author
**Om Patil**  
Machine Learning & Data Science Enthusiast  
