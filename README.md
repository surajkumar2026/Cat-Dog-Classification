# 🐱🐶 Cat vs Dog Classification

This project uses a **Convolutional Neural Network (CNN)** built with **TensorFlow/Keras** to classify images as cats or dogs.  
The model is trained on the **Dogs vs Cats** dataset from Kaggle.

---

## 📂 Dataset
- **Source:** [Kaggle - Dogs vs Cats](https://www.kaggle.com/datasets/salader/dogs-vs-cats)  
- Images are split into `train/` and `test/` directories with `cat/` and `dog/` subfolders.

---

## 🛠️ Tech Stack
- **Language:** Python  
- **Libraries:** TensorFlow, Keras, Matplotlib  
- **Model:** Custom CNN with BatchNormalization & Dropout

---

## 🧠 Model Summary
- **Input:** 256×256 RGB images  
- **Layers:**  
  - 3× Conv2D → BatchNormalization → MaxPooling2D  
  - Flatten → Dense(128) → Dropout → Dense(64) → Dropout  
  - Output: Dense(1, activation='sigmoid')  
- **Loss:** Binary Crossentropy  
- **Optimizer:** Adam

---

## 🚀 How It Works
1. Load dataset from directory.  
2. Normalize pixel values to `[0,1]`.  
3. Train CNN for 10 epochs with validation set.  
4. Evaluate and plot accuracy/loss curves.

---

## 📊 Expected Results
- Accuracy: ~85–90% after 10 epochs.  
- Loss & accuracy plots available in notebook.


