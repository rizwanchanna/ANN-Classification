# ANN Classification for Customer Churn Prediction
This project focuses on building an Artificial Neural Network (ANN) to predict customer churn based on a variety of input features. The application is built using TensorFlow and Keras, and includes preprocessing pipelines, model training, hyperparameter tuning, and a basic prediction interface.

# Project Structure
- app.py: Main application script for running predictions using the trained model.
- Churn_Modelling.csv: Dataset used for training the classification model. It includes features such as customer demographics, account balance, and product usage.
- experiments.ipynb, hyperparametertuningann.ipynb, prediction.ipynb, salaryregression.ipynb: Jupyter notebooks used for various stages of model development, including experimentation, parameter tuning, and testing.
- model.h5: Trained ANN model saved in HDF5 format.
- label_encoder_gender.pkl, onehot_encoder_geo.pkl, scaler.pkl: Pickled preprocessing objects used for transforming input features (gender encoding, geographic encoding, and feature scaling).
- requirements.txt: List of Python dependencies needed to run the project.

# Getting Started
Clone the Repository
git clone https://github.com/rizwanchanna/ANN-Classification
cd annclassification/annclassification

Install Dependencies
It is recommended to use a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt

Run the Application
Make sure all necessary .pkl files and the model.h5 are in place, then run:

python app.py
Dataset
The dataset Churn_Modelling.csv contains records of bank customers, including their geographic information, credit score, balance, estimated salary, and a label indicating whether they exited the bank. The goal of the model is to predict this churn label.

# Model Details
The ANN is built using Keras and trained on preprocessed data. Feature encoding includes:
- One-hot encoding for geographic data
- Label encoding for gender
- Standard scaling for numerical features

Hyperparameter tuning was conducted and documented in hyperparametertuningann.ipynb.

# Usage
After launching the app or using the prediction.ipynb notebook, you can input new customer data and receive a prediction on whether they are likely to churn.
