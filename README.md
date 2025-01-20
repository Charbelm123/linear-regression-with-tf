# Auto MPG Linear Regression

This project implements various regression models to predict car fuel efficiency (MPG - Miles Per Gallon) based on different features like horsepower, weight, cylinders etc. using the classic Auto MPG dataset.

## Dataset

The Auto MPG dataset contains information about various cars including:
- MPG (Miles Per Gallon)
- Cylinders
- Displacement
- Horsepower 
- Weight
- Acceleration
- Model Year
- Origin
- Car Name

## Models Implemented

The project implements several regression models with increasing complexity:
1. Single Feature Linear Regression (using horsepower)
2. Multi-Feature Linear Regression (using all features)
3. Deep Neural Network with single feature
4. Deep Neural Network with all features

## Requirements

The project requires the following Python packages:
tensorflow
numpy  
pandas
matplotlib
seaborn

Project Structure
auto-mpg/
├── auto-mpg.data        # Main dataset file
├── auto-mpg.data-original # Original dataset backup
├── auto-mpg.names       # Dataset description
├── linear_regression.ipynb # Main Jupyter notebook
└── requirements.txt     # Project dependencies

Usage
1-Install the requirements:
  pip install -r requirements.txt
2-Open and run the Jupyter notebook:
  jupyter notebook linear_regression.ipynb

Model Architecture
The DNN model architecture consists of:

Input normalization layer
Two dense layers with 128 units and ReLU activation
L1 regularization (0.001) on dense layers
Output layer with single unit (MPG prediction)
The model is trained using:

Adam optimizer
Mean Absolute Error loss function
100 epochs
20% validation split


