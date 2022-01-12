# Time-Series Forecasting using Deep Learning in Predictive Maintenance

![An Engineer Doing Maintenance Works](https://images.pexels.com/photos/2760243/pexels-photo-2760243.jpeg?crop=entropy&cs=srgb&dl=pexels-kateryna-babaieva-2760243.jpg)

## Introduction
Predictive maintenance aims to predict whether a machine will fail and needs to be repaired given data produced by various sensors placed in the machine while it is running. 
There are multiple commonly used sensors, such as temperature, voltage, and pressure sensor. The readings produced by these sensors are then sent to a database and then used in further analysis to determine several important requirements to guarantee the machine's performance, such as Mean Time Before Failure (MTBF) and Mean Time To Repair (MTTR). In terms of time-series forecasting, one possible approach is to predict the value of a certain sensor several hours in advance. The predicted values can then be compared with a predetermined threshold based on domain knowledge or be fed into another machine learning algorithm to determine the probability of the machine breaking down. 

## Dataset
The dataset is obtained from [Kaggle](https://www.kaggle.com/arnabbiswas1/microsoft-azure-predictive-maintenance), which contains five .csv files describing different events (error, failure, and maintenance) and the sensor data for each machine. 

## Approach
In this repository, a simple deep learning model based on LSTM will be used to predict the value of the chosen feature (e.g. readings from pressure sensor). Further, a failure event from the record will be chosen to check whether the model can correctly predict the chosen sensor readings in the event of failure. 
