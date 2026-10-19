# New York City Taxi Fare Prediction

## Overview

This project uses an artificial neural network (ANN) to predict the fare amount of a New York City taxi trip. The model learns from trip details such as pickup and dropoff locations, pickup time, and passenger count.

The goal is to use these features to estimate the trip fare for records where the fare is unknown.

## Dataset

The dataset comes from the [New York City Taxi Fare Prediction competition on Kaggle](https://www.kaggle.com/competitions/new-york-city-taxi-fare-prediction).

It contains:

- `data.csv` — trip information and the known fare, used to train and evaluate the model.

### Data fields

| Field | Description |
|---|---|
| `key` | Unique identifier for each trip. Used to match predictions to test rows. |
| `pickup_datetime` | Date and time the trip started. |
| `pickup_longitude` | Longitude of the pickup location. |
| `pickup_latitude` | Latitude of the pickup location. |
| `dropoff_longitude` | Longitude of the dropoff location. |
| `dropoff_latitude` | Latitude of the dropoff location. |
| `passenger_count` | Number of passengers. |
| `fare_amount` | Trip fare in dollars; this is the value the model predicts. |

## Project Workflow

1. Load and inspect the training data.
2. Clean the data and handle missing or invalid values.
3. Prepare useful model inputs from the trip details.
4. Split the training data into training and validation sets.
5. Train an ANN to predict `fare_amount`.
6. Evaluate predictions using a regression metric such as root mean squared error (RMSE).
7. Generate fare predictions for the test data and save them in the required submission format.

## Model

The project uses a feed-forward artificial neural network for regression. It takes processed trip features as input and produces an estimated fare amount.

The model’s performance depends on data preparation, feature selection, and training settings. No performance score is stated here; add your measured validation or competition result after running the model.

## Tools

- Python
- pandas
- NumPy
- scikit-learn
- PyTorch


## Acknowledgements

Dataset provided through Kaggle’s [New York City Taxi Fare Prediction](https://www.kaggle.com/competitions/new-york-city-taxi-fare-prediction) competition, hosted in partnership with Google Cloud and Coursera.
