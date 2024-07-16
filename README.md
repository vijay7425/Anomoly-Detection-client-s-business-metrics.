# Splash Anomaly Detection
Welcome to the Splash Anomaly Detection project! This repository contains the code and resources for the Anomaly Detection task aimed at helping retailers with pricing intelligence and business monitoring.

## Project Description
In the dynamic world of retail, real-time monitoring and analysis of business metrics are crucial for detecting incidents that may impact revenue. Our primary challenge is to monitor and analyze our client's business metrics in real time to instantly detect anomalies. This project focuses on detecting anomalies in business metrics to generate alerts for our clients.

### Dataset
The dataset used for this project contains the following columns:

timestamp [float]: Provided as a Unix epoch in seconds.
value [int]: A real value measurement of some metric at the timestamp.</br>
is_anomaly [boolean]: A boolean value indicating whether the corresponding value is identified as an anomaly.</br>
predicted [float]: A real value prediction from a black-box forecasting model for that timestamp. This model is assumed to be aware of only the true data distribution.

### Anomaly Detection Task
The task involves developing a model to detect anomalies in the given dataset. The anomalies are identified based on the provided is_anomaly column, and the predictions from a black-box forecasting model are used to enhance the detection process.

### Installation
To run this project locally, follow these steps:

### Clone the repository:
```
git clone https://github.com/vijay7425/splash-anomaly-detection.git
cd splash-anomaly-detection
```
### Create and activate a virtual environment:
```
python -m venv venv
source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
```
### Install the required dependencies:
```
pip install -r requirements.txt
```
### Usage
To run the anomaly detection script, execute the following command:
```
python anomaly_detection.py
```
This script will process the dataset, train the anomaly detection model, and evaluate its performance.
