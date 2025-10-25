# 🐾 Dog vs. Cat CNN Classifier

A custom Convolutional Neural Network (CNN) built with TensorFlow/Keras to classify images of dogs and cats.



---

## 📖 Table of Contents
* [Project Goal](#project-goal)
* [Model Architecture](#model-architecture)
* [Results](#results)
* [Installation](#installation)
* [How to Use](#how-to-use)

---

## 🎯 Project Goal
The goal of this project was to build and train a custom CNN from scratch to achieve high accuracy on the "Dogs vs. Cats" dataset.

---

## 🔧 Model Architecture

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┓
┃ Layer (type)                    ┃ Output Shape           ┃       Param # ┃
┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━┩
│ conv2d (Conv2D)                 │ (None, 148, 148, 32)   │           896 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ max_pooling2d (MaxPooling2D)    │ (None, 74, 74, 32)     │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ conv2d_1 (Conv2D)               │ (None, 72, 72, 64)     │        18,496 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ max_pooling2d_1 (MaxPooling2D)  │ (None, 36, 36, 64)     │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ conv2d_2 (Conv2D)               │ (None, 34, 34, 128)    │        73,856 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ max_pooling2d_2 (MaxPooling2D)  │ (None, 17, 17, 128)    │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ flatten (Flatten)               │ (None, 36992)          │             0 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dense (Dense)                   │ (None, 512)            │    18,940,416 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dense_1 (Dense)                 │ (None, 1)              │           513 │
└─────────────────────────────────┴────────────────────────┴───────────────┘

## 📊 Results
The model was trained for 10 epochs and achieved:
* 
* **Validation Accuracy:** 83%

Here is the training and validation loss/accuracy over time:


---

## ⚙️ Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/dog-cat-cnn.git](https://github.com/YOUR_USERNAME/dog-cat-cnn.git)
    cd dog-cat-cnn
    ```

2.  **(Recommended) Create a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Install Git LFS** (to download the model file):
    ```bash
    git lfs install
    git lfs pull
    ```
---

## 🚀 How to Use

### 1. Dataset
This project uses the Kaggle "Dogs vs. Cats" dataset.
1.  Download the dataset using !kaggle datasets download -d biaiscience/dogs-vs-cats.
2.  Unzip the `train.zip` and `test.zip` files.



```
Prediction: Dog (92.4% confidence)
```
