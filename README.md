Human Activity Recognition with CNN-LSTM and Gradio
Overview
This project implements a Human Activity Recognition (HAR) system using a hybrid deep learning model (CNN-LSTM) and an interactive Gradio web interface. The system processes time-series sensor data (e.g., accelerometer, gyroscope) to classify activities like walking, sitting, and running. It supports real-time predictions, batch processing, and data exploration.

Features
Hybrid CNN-LSTM Model:
Combines CNN for local feature extraction and LSTM for modeling temporal dependencies.

Comprehensive Preprocessing:
Data cleaning, missing value imputation, feature scaling, and segmentation into overlapping windows.

Interactive Gradio Interface:

Real-time and batch predictions

Visualization of prediction confidence and history

Exploratory data analysis (EDA) tools

Getting Started
Prerequisites
Python 3.7+

Recommended: virtual environment

Install Required Libraries

pip install gradio pandas numpy scikit-learn tensorflow matplotlib pillow

Dataset
Place your CSV files:

train_har.csv

test.csv

Each file should include sensor readings and an Activity label.

Running the App
Ensure dataset files are in place.

Run the application:

python HAR_system.py
The Gradio web interface will open in your browser.

Usage
Predict Activity:

Predict on test samples or upload your own CSV for batch predictions.

View prediction history and confidence.

EDA Tabs:

Explore activity distribution, feature statistics, confusion matrix, and per-class accuracy.

Project Structure
text
├── train_har.csv
├── test.csv
├── HAR_system.py
└── README.md
Methodology
Data preprocessing: numeric conversion, imputation, scaling, windowing

Model: 1D CNN layers, LSTM layer, dense layers with dropout

Evaluation: accuracy, confusion matrix, per-class accuracy

This project is for educational and research purposes.
