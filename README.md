# IPL Match Winner Prediction using Artificial Neural Networks

## Overview

This project focuses on predicting the outcome of IPL (Indian Premier League) cricket matches using an Artificial Neural Network (ANN). The model is trained on historical match and ball-by-ball data to learn patterns that influence match outcomes.

The objective is to build a classification model that predicts whether a team will win or lose based on match conditions and game progress.

---

## Dataset

The project uses two datasets:

* matches.csv
  Contains match-level information such as teams, venue, toss winner, and result.

* deliveries.csv
  Contains ball-by-ball data including runs scored, wickets, overs, and match events.

---

## Features Used

* Batting team
* Bowling team
* Venue
* Current score
* Balls left
* Wickets left
* Current Run Rate (CRR)
* Required Run Rate (RRR)

These features were engineered from raw data to capture match dynamics.

---

## Data Preprocessing

* Handled missing values
* Converted categorical data into numerical format
* Removed irrelevant columns (ID, names, etc.)
* Fixed datatype issues (string to numeric)
* Cleaned inconsistent rows in deliveries dataset
* Created new features like current_run, balls_left, and run rates

---

## Model Architecture

* Input Layer
* Dense Layer (ReLU)
* Dropout Layer
* Dense Layer (ReLU)
* Output Layer (Sigmoid)

---

## Training Details

* Loss Function: Binary Crossentropy
* Optimizer: Adam
* Metrics: Accuracy
* Epochs: 17
* Batch Size: 32

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## Results

* Accuracy: ~85%
* Precision: ~84%
* Recall: ~89%
* F1 Score: ~86%

The model shows strong performance with good generalization.

---

## Confusion Matrix Interpretation

* True Positives: Correct win predictions
* True Negatives: Correct loss predictions
* False Positives: Incorrect win predictions
* False Negatives: Missed win predictions

The model performs well with balanced predictions.

---

## Visualizations

* Accuracy vs Epoch graph
* Loss vs Epoch graph
* Confusion Matrix heatmap
* Correlation heatmap

---

## Key Observations

* Run rate and match progress strongly influence outcomes
* Feature engineering significantly improves performance
* Model shows minimal overfitting
* Ball-by-ball data provides deeper insights

---

## Conclusion

The ANN model successfully predicts IPL match outcomes with good accuracy. Proper preprocessing and feature engineering played a major role in improving model performance.

---

