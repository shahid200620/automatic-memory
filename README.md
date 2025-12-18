# 🧠 Binary Classification using Deep Neural Network (TensorFlow/Keras)

## 📌 Project Overview
This project demonstrates the complete end-to-end workflow of building a **Deep Neural Network (DNN)** for a **binary classification problem** using **TensorFlow and Keras**.  
It covers data preprocessing, exploratory data analysis (EDA), model design, training with callbacks, evaluation using multiple metrics, and result visualization.

The objective is to develop a **robust, well-documented, and evaluatable deep learning solution** following best practices.

---

## 📂 Dataset Description
- Total Samples: **267**
- Input Features: **44 numerical features**
- Target Variable: **Binary (0 / 1)**  
- Note: The dataset did not contain explicit column headers.  
  The **last column was treated as the target variable**.

---

## 🔍 Exploratory Data Analysis (EDA)
The EDA process included:
- Feature distribution analysis
- Correlation heatmap
- Feature vs target relationship analysis

Key observations:
- Features required scaling due to different ranges
- No extreme multicollinearity was observed
- The dataset was suitable for binary classification using a neural network

---

## 🏗️ Model Architecture
The neural network was built using the **Sequential API** in Keras.

**Architecture Details:**
- Input Layer: 44 features
- Hidden Layer 1: 64 neurons (ReLU)
- Hidden Layer 2: 32 neurons (ReLU)
- Hidden Layer 3: 16 neurons (ReLU)
- Output Layer: 1 neuron (Sigmoid)

**Loss Function:** Binary Crossentropy  
**Optimizer:** Adam  
**Metric:** Accuracy  

---

## ⚙️ Training Strategy
- Data Split:
  - 60% Training
  - 20% Validation
  - 20% Test
- Feature Scaling: `StandardScaler`
- Callbacks Used:
  - **EarlyStopping** (prevents overfitting)
  - **ModelCheckpoint** (saves best model based on validation loss)

---

## 📊 Model Evaluation
The model was evaluated on a **held-out test set** using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Additionally:
- ROC Curve plotted
- Training & Validation loss curves visualized
- Training & Validation accuracy curves visualized

The model achieved **strong generalization performance**, meeting the expected evaluation criteria.

---

## 📁 Project Structure
