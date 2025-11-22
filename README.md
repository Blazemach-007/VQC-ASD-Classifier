⚛️ VQC-ASD-Classifier
A project implementing a Variational Quantum Classifier (VQC) using PennyLane and PyTorch to classify Autism Spectrum Disorder (ASD) across combined child, adolescent, and adult datasets.

🎯 Project Overview
This repository contains the code for an experimental machine learning model that leverages Quantum Computing principles to tackle a binary classification problem.

Key Components:
Dataset: Combination of Autism screening datasets (Child, Adolescent, Adult).

Model: A hybrid Classical-Quantum Neural Network (CQNN) implemented with PyTorch and PennyLane.

Quantum Circuit: Uses Angle Embedding for data input and a Strongly Entangling Layer ansatz for quantum feature mapping.

Objective: Classify individuals as having ASD (YES) or not (NO).

🛠️ Requirements and Setup
To run this code, you'll need Python and the following libraries. It's recommended to use a virtual environment.
=>  pip install pennylane pennylane-lightning[gpu] torch pandas scikit-learn matplotlib seaborn

Output
The script trains the model for 70 epochs and outputs training metrics (Loss/Accuracy/LR) per epoch, followed by comprehensive test set metrics and visualizations.

Test Metrics:
The final output will include metrics calculated on the 20% test split:
    Accuracy
    Precision
    Recall
    F1 Score
    ROC-AUC Score
    Classification Report

Visualizations:
The script generates plots to visualize the model's performance and training progression:
    Training Loss vs. Epoch
    Training Accuracy vs. Epoch
    Confusion Matrix on Test Data
    ROC Curve on Test Data