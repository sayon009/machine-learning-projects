# Heart Disease Prediction

## Overview

An end-to-end machine learning project for predicting the presence of heart disease from patient health and clinical features.

The project covers exploratory data analysis, data preprocessing, feature transformation, model training, model evaluation, and deployment through a Flask application.

## Dataset

The dataset contains 13 input features related to patient health and a target variable indicating the presence or absence of heart disease.

### Features

- Age
- Gender
- Chest Pain Type
- Resting Blood Pressure
- Serum Cholesterol
- Fasting Blood Sugar
- Resting Electrocardiographic Results
- Maximum Heart Rate Achieved
- Exercise-induced Angina
- ST Depression
- Slope of Peak Exercise ST Segment
- Number of Major Vessels
- Thalassemia

### Target

The target variable represents whether heart disease is present or absent.

## Project Workflow

1. Data ingestion
2. Exploratory Data Analysis
3. Data preprocessing
4. Feature transformation
5. Model training
6. Model evaluation
7. Prediction pipeline
8. Flask-based deployment

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Flask
- CatBoost
- XGBoost
- MLflow
- DVC

## Project Structure

```text
Heart-Disease-Prediction/
│
├── Notebook_Experiments/
│   ├── Data/
│   ├── Exploratory_Data_Analysis.ipynb
│   └── Model_training.ipynb
│
├── src/
│   └── Heart/
│       ├── components/
│       │   ├── Data_ingestion.py
│       │   ├── Data_transformation.py
│       │   ├── Model_evaluation.py
│       │   └── Model_trainer.py
│       │
│       ├── pipeline/
│       │   ├── Prediction_pipeline.py
│       │   └── Training_pipeline.py
│       │
│       └── utils/
│
├── static/
├── templates/
├── app.py
├── requirements.txt
├── setup.py
├── Dockerfile
└── README.md
Installation

Clone the repository:

git clone https://github.com/sayon009/machine-learning-projects.git

Navigate to the project:

cd machine-learning-projects/Heart-Disease-Prediction

Install the required dependencies:

pip install -r requirements.txt
Running the Application

Start the Flask application:

python app.py

The application can then be accessed through the local Flask server.

Machine Learning Pipeline

The project follows a modular machine learning pipeline consisting of:

Data ingestion
Data transformation
Model training
Model evaluation
Prediction

The training and prediction workflows are organized inside the src/Heart package.

Experiment Tracking

MLflow is included in the project for experiment tracking and model-related experimentation.

Sensitive credentials and tracking passwords are intentionally not stored in this repository.

Deployment

The project includes a Flask web application and a Dockerfile for containerized deployment.

Note

This project is maintained as part of a machine learning learning and portfolio collection. The implementation is based on an existing open-source project and is being studied and extended for educational purposes.

License

This project is distributed under the MIT License. See the LICENSE file for details.