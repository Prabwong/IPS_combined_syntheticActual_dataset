# IPS_combined_syntheticActual_dataset

This repository is part of an Indoor Positioning System (IPS) project that aims to improve location prediction accuracy using a combination of actual data and synthetic data. The dataset combines real-world RSSI (Received Signal Strength Indicator) values and synthetically generated data using Machine Learning (ML) and Generative Adversarial Networks (GANs).

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset Structure](#dataset-structure)
- [Usage](#usage)
- [Synthetic Data Generation](#synthetic-data-generation)
- [Model Training](#model-training)
- [Evaluation Metrics](#evaluation-metrics)
- [Prerequisites](#prerequisites)
- [How to Run](#how-to-run)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

Indoor Positioning Systems rely heavily on fingerprinting techniques using RSSI values. However, collecting actual RSSI data is time-consuming and expensive. This project addresses the challenge by generating **synthetic data** that complements actual data to reduce data collection time while maintaining prediction accuracy.

Key goals:
- Combine **actual data** and **synthetic data** in various ratios (e.g., 90:10, 80:20).
- Train models to predict user positions (x, y, and floor).
- Evaluate model performance based on combined datasets.

---

## Dataset Structure

The repository includes:
- **Actual Data**: Real-world RSSI data collected from multiple access points (APs).
- **Synthetic Data**: Data generated using machine learning and GAN techniques.

The datasets are combined in ratios such as:
- **90:10**: 90% actual data, 10% synthetic data.
- **80:20**: 80% actual data, 20% synthetic data.

---

## Usage

This repository can be used for:
- Training and evaluating indoor positioning models.
- Testing the impact of synthetic data on model performance.
- Experimenting with different data ratios and model configurations.

---

## Synthetic Data Generation

Synthetic data is generated using:
1. **Machine Learning Models**: To interpolate and generate new data points based on actual RSSI values.
2. **Generative Adversarial Networks (GANs)**: To create realistic RSSI distributions mimicking actual data.

---

## Model Training

The repository supports training the following types of models:
1. **Floor Prediction**: Classification models to predict the floor.
2. **Coordinate Prediction**: Regression models to predict (x, y) coordinates.

Supported models include:
- Linear Models
- Decision Trees
- Random Forests
- Gradient Boosting
- K-Nearest Neighbors

---

## Evaluation Metrics

The following metrics are used for evaluation:
### Floor Prediction:
- Mean Absolute Error (MAE)
- Training Time
- Prediction Time
- Memory Usage

### Coordinate Prediction:
- Mean Distance Error
- Training Time
- Prediction Time
- Memory Usage

---

## Prerequisites

- Python 3.8+
- Required libraries: `scikit-learn`, `tensorflow`, `numpy`, `pandas`, etc.
- A basic understanding of IPS concepts.

---