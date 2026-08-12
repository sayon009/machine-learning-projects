# Spam Email Detection

## Overview

An end-to-end machine learning project for classifying emails as spam or non-spam using natural language processing and supervised machine learning.

The project covers data ingestion, text preprocessing, feature transformation, model training, model evaluation, and deployment through a Flask application.

## Dataset

The project uses a labeled email dataset containing examples of spam and non-spam messages.

The text data is transformed into numerical features before being provided to the machine learning model.

## Machine Learning Workflow

The project follows the following workflow:

1. Data ingestion
2. Data preprocessing
3. Text feature extraction
4. Model training
5. Model evaluation
6. Prediction pipeline
7. Flask-based deployment

## Text Processing

Email text is processed and transformed into numerical features using a feature extraction pipeline before being passed to the trained machine learning model.

The trained feature transformation object is stored in:

```text
data/models/v1/feature.pkl
Model

The trained machine learning model is stored in:

data/models/v1/model.pkl

The prediction pipeline loads the trained model and feature transformation components to classify new email messages.

Technologies
Python
Pandas
NumPy
Scikit-learn
Natural Language Processing
Flask
Project Structure
Spam-Email-Detection/
│
├── data/
│   ├── dataset/
│   │   └── dataset.csv
│   └── models/
│       └── v1/
│           ├── feature.pkl
│           └── model.pkl
│
├── Notebook Experiments/
│   └── Spam Email Detection.ipynb
│
├── src/
│   ├── components/
│   ├── config/
│   ├── pipeline/
│   └── utils/
│
├── app.py
├── pyproject.toml
├── requirements.txt
├── README.md
└── LICENSE
Installation

Clone the repository:

git clone https://github.com/sayon009/machine-learning-projects.git

Navigate to the project:

cd machine-learning-projects/Spam-Email-Detection

Install the dependencies:

pip install -r requirements.txt
Running the Application

Start the Flask application:

python app.py

The application can then be accessed through the local Flask server.

Running the Notebook

Open:

Notebook Experiments/Spam Email Detection.ipynb

The notebook contains the data analysis, preprocessing, feature transformation, model training, and evaluation workflow.

Note

This project is maintained as part of a machine learning learning and portfolio collection. The implementation is based on an existing open-source project and is being studied and extended for educational purposes.

License

See the LICENSE file for license information.


