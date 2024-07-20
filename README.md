# Anomaly_Detector

## Overview
This project implements an anomaly detection model using the Gaussian (normal) distribution to identify anomalies in a dataset. The model assumes that normal data points follow a Gaussian distribution and identifies anomalies based on their deviation from this expected distribution. Anomalies are considered as points that lie at the tails of the Gaussian distribution.

## Features
### Model:

- **Anomaly Detection** : Utilizes the Gaussian distribution to model the data. By estimating the mean and variance of the data, the model defines what constitutes "normal" behavior.
- **Probability Calculation** : Computes the probability density function (PDF) for each data point. Points with low probability values are considered potential anomalies.
### Thresholding:

- **Classification** : Defines a threshold for the probability values. Data points with probability below this threshold are classified as anomalies.
- **Customization** : Allows for the threshold to be adjusted based on the desired sensitivity of the anomaly detection. A lower threshold results in fewer anomalies being detected, while a higher threshold increases sensitivity.

### Evaluation:

   **Metrics** : Evaluates the model's performance using precision, recall, and F1-score.
- **Precision** : Measures the accuracy of the anomalies detected (i.e., the proportion of true anomalies among the detected anomalies).
- **Recall** : Measures the model's ability to detect all actual anomalies (i.e., the proportion of actual anomalies that were correctly detected).
- **F1-score** : Provides a balanced measure of the model's performance by combining precision and recall.

### Visualization:

- **Distribution Plotting** : Visualizes the Gaussian distribution of the data, showing the mean and variance.
- **Anomaly Highlighting** : Highlights detected anomalies on the distribution plot, making it easy to see how far these points deviate from the normal distribution.
- **Interactive Elements** : May include interactive elements (e.g., sliders) to adjust the threshold and see the impact on anomaly detection in real-time.
