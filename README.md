\# Binary Classification using Deep Neural Network (TensorFlow/Keras)



\## Overview

This project implements a Deep Neural Network (DNN) using TensorFlow and Keras to solve a binary classification problem. The workflow includes data preprocessing, exploratory data analysis, model training with callbacks, and rigorous evaluation.



\## Dataset

The dataset consists of 267 samples with 44 numerical features. The final column represents the binary target variable. Since the dataset did not include explicit headers, the last column was treated as the target.



\## Model Architecture

\- Sequential Neural Network

\- 3 Hidden Layers with ReLU activation (64, 32, 16 neurons)

\- Output layer with 1 neuron and Sigmoid activation

\- Binary Crossentropy loss

\- Adam optimizer



\## Training Strategy

\- Data split: 60% Training, 20% Validation, 20% Testing

\- Feature scaling using StandardScaler

\- EarlyStopping to prevent overfitting

\- ModelCheckpoint to save the best-performing model



\## Evaluation Metrics

The model was evaluated on a held-out test set using:

\- Accuracy

\- Precision

\- Recall

\- F1-score

\- ROC-AUC



The trained model achieved strong performance, demonstrating effective generalization.



\## How to Run

1\. Create and activate a virtual environment

2\. Install dependencies from `requirements.txt`

3\. Run the Jupyter Notebook `binary\_classification\_dnn.ipynb`



\## Files

\- `binary\_classification\_dnn.ipynb` — Main notebook

\- `model/best\_model.h5` — Saved model

\- `requirements.txt` — Dependencies



