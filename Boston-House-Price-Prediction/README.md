# Boston House Price Prediction

## Overview

An end-to-end machine learning project for predicting housing prices using the Boston Housing dataset.

The project covers data preprocessing, exploratory data analysis, model training, hyperparameter tuning, evaluation, and deployment through a Flask web application.

## Dataset

The Boston Housing dataset contains 506 instances and 13 numerical input features describing different characteristics of houses and their surrounding areas.

### Features

1. `CRIM` - Per capita crime rate by town
2. `ZN` - Proportion of residential land zoned for large lots
3. `INDUS` - Proportion of non-retail business acres per town
4. `CHAS` - Charles River dummy variable
5. `NOX` - Nitric oxide concentration
6. `RM` - Average number of rooms per dwelling
7. `AGE` - Proportion of owner-occupied units built prior to 1940
8. `DIS` - Weighted distance to Boston employment centers
9. `RAD` - Index of accessibility to radial highways
10. `TAX` - Property tax rate
11. `PTRATIO` - Pupil-teacher ratio by town
12. `B` - Feature derived from the proportion of Black residents by town
13. `LSTAT` - Percentage of lower-status population

### Target

`MEDV` - Median value of owner-occupied homes in thousands of dollars.

## Machine Learning Workflow

The project follows the following workflow:

1. Data loading
2. Exploratory Data Analysis
3. Feature and target separation
4. Feature standardization
5. Train-test split
6. Model training
7. Hyperparameter tuning
8. Model evaluation
9. Model deployment

## Data Preprocessing

The dataset is separated into input features (`X`) and target values (`y`).

The input features are standardized using `StandardScaler` from Scikit-learn.

The dataset is then divided into training and testing sets using an 80:20 split.

## Model Training

The project uses `CatBoostRegressor` for housing price prediction.

Hyperparameter tuning is performed using `RandomizedSearchCV` with 5-fold cross-validation to identify a suitable set of model parameters.

### Algorithm

- CatBoostRegressor

### Evaluation

The trained model is evaluated on the test dataset using the R-squared (`R²`) metric.

## Deployment

The trained model is deployed through a Flask web application.

The application loads:

- `housepred.pkl` - trained prediction model
- `scaler.pkl` - feature scaler

Users can provide the required house features through the web interface, after which the application returns the predicted house price.

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- CatBoost
- Flask
- Gunicorn

## Project Structure

```text
Boston-House-Price-Prediction/
│
├── templates/
│   ├── home.html
│   └── house.ico
│
├── Boston House Price Prediction.ipynb
├── app.py
├── housepred.pkl
├── scaler.pkl
├── requirements.txt
├── README.md
└── LICENSE
Installation

Clone the repository:

git clone https://github.com/sayon009/machine-learning-projects.git

Navigate to the project:

cd machine-learning-projects/Boston-House-Price-Prediction

Install the dependencies:

pip install -r requirements.txt
Running the Application

Start the Flask application:

python app.py

The application can then be accessed through the local Flask server.

Running the Notebook

Open:

Boston House Price Prediction.ipynb

Run the notebook to explore the dataset, perform preprocessing, train the model, and evaluate its performance.

Note

This project is maintained as part of a machine learning learning and portfolio collection. The implementation is based on an existing open-source project and is being studied and extended for educational purposes.

License

This project is distributed under the GNU General Public License v3.0. See the LICENSE file for details.


