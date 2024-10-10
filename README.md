# Crop Stage Detection and Prediction

## Overview
This project implements a crop stage detection and prediction model using remote sensing data from Google Earth Engine (GEE). The main algorithm uses first and second derivative calculations to detect the phase or change in time series trend's curve.
The model utilizes various machine learning techniques, specifically LSTM (Long Short-Term Memory) networks, to analyze the satellite imagery data and predict the growth stages of crops.
This project is an fully automated approach from extracting remote sensing data from Google Earth Engine API till model training.

## Algorithm Specific hyper parameters
1. Crop cycle length
2. window length for savgol filter to remove the noise from extracted data
3. Poly order as a parameter of savgol filter

## Features
- Fetches Sentinel-2 satellite imagery data from Google Earth Engine.
- Masks clouds from the imagery for accurate analysis.
- Processes and prepares the data for modeling.
- Implements LSTM for predicting crop growth stages.

## Prerequisites
Before running the script, ensure you have the following installed:

- Python 3.x
- Required libraries (listed in `requirements.txt`)

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/pallavi17798/crop-stage-detection.git
   cd crop-stage-detection

