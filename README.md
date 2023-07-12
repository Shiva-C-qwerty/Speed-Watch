# SpeedWatch: Automated Overspeed Detection and Analysis

This repository contains code for a Speed Detection system using computer vision techniques. The system detects and tracks vehicles in a video stream, calculates their speeds, and identifies overspeeding vehicles. It also includes an analysis of the speed data and prediction of traffic flow rates.

## Contents

- `Speed Detection.py`: Python script for detecting and tracking vehicles, calculating speeds, and identifying overspeeding vehicles.
- `Speed Analysis.py`: Python script for analyzing speed data, fitting GARCH and ARIMA models, and predicting traffic flow rates.
- `files/`: Directory containing the required files for the speed detection system (Haar cascade classifier XML file and test video file).
- `overspeeding/`: Directory to store images of overspeeding vehicles.
- `overspeeding.csv`: CSV file containing information about the overspeeding vehicles detected.

## Prerequisites

- Python 3.x
- OpenCV
- dlib
- pandas
- numpy
- matplotlib
- arch
- statsmodels
- sklearn
- seaborn

## Usage

1. Ensure that the necessary dependencies are installed.
2. Place the Haar cascade classifier XML file in the `files/` directory.
3. Place the video file for testing in the `files/` directory.
4. Run the `Speed Detection.py` script to detect and track vehicles, calculate speeds, and identify overspeeding vehicles. The script will display the video stream with bounding boxes around the detected vehicles.
5. After the script finishes, the overspeeding vehicles' images and information will be stored in the `overspeeding/` directory and `overspeeding.csv` file, respectively.
6. Run the `Speed Analysis.py` script to analyze the speed data, fit GARCH and ARIMA models, and predict traffic flow rates. The script will generate visualizations and print relevant statistics.

## Results

The `Speed Detection.py` script will display the video stream with bounding boxes around the detected vehicles. It will print the vehicle IDs, speeds, and whether they are overspeeding. The overspeeding vehicles' images will be saved in the `overspeeding/cars/` directory, and the information will be stored in the `overspeeding.csv` file.

The `Speed Analysis.py` script will generate visualizations of the speed data, including a plot of speed over time and volatility plot from the GARCH model. It will print the summary of the GARCH model, as well as statistics such as mean absolute error (MAE), mean squared error (MSE), root mean squared error (RMSE), and mean absolute percentage error (MAPE). Additionally, it will predict traffic flow rates using ARIMA and machine learning models (Linear Regression, Gradient Boosting Regressor, and Random Forest Regressor).

Please refer to the detailed documentation in the repository for more information on configuration options, API integration, and customization.
