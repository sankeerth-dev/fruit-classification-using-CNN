# 🍎 Fruit Classification using CNN

This project is a deep learning-based image classification model that identifies different types of fruits using a Convolutional Neural Network (CNN). Built using TensorFlow and Keras, the model is trained on a labeled dataset of fruit images and achieves high accuracy using standard preprocessing and data augmentation techniques.

---

## 📌 Project Overview

- 📷 **Input**: Images of fruits
- 🧠 **Model**: Convolutional Neural Network (CNN)
- 🎯 **Goal**: Classify images into 6 different fruit categories
- 💡 **Tools**: Python, TensorFlow, Keras, Matplotlib

---

## 🗂️ Dataset

- Loaded using `image_dataset_from_directory`
- Dataset split: 80% training, 10% validation, 10% testing
- Images resized to **300x300 pixels**
- Contains 6 fruit classes (e.g., apple, banana, etc.)

---

## 🏗️ Model Architecture

```text
Input → Resize & Rescale → Data Augmentation →
Conv2D → MaxPooling × 6 →
Flatten → Dense(64) → Dense(6, Softmax)
