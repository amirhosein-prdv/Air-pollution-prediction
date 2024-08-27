## Air Pollution Prediction in Smart Cities using Deep Learning

### Overview
This repository contains the implementation of a deep learning approach for predicting air pollution, specifically PM2.5 levels, in the city of Beijing, China. The method utilizes a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks for accurate predictions.
![image](https://github.com/user-attachments/assets/cca1a26e-a5fb-4df4-87bc-0501dd430cda)

### Dataset
The dataset consists of hourly air pollution measurements from 12 monitoring sites in Beijing. Each site provides PM2.5 data along with other air pollutants.

### Preprocessing
1. **Missing Value Imputation**: Utilizing linear interpolation for filling missing values in PM2.5 data.
2. **Encoding Categorical Variables**: Converting wind direction to degrees.
3. **Normalization**: Applying Min-Max normalization to the data.

### Pearson Correlation
Calculating the Pearson correlation between PM2.5 values from the Aotizhongxin station and surrounding sites.

### Feature Selection
Creating an Excel file with selected features, including PM2.5 data from all stations, CO, PM10, and other meteorological variables.

### Supervised Dataset
Preparing the data in a supervised format for training, splitting it into 80% for training and 20% for testing.

### Training the Model
Implementing the CNN-LSTM model as described in the paper with optimal hyperparameters. Reporting RMSE, MAE, and R2 for lag periods of 1 day and 7 days.

### References
this model adopted from this paper:

`Bekkar, A., Hssina, B., Douzi, S. et al. Air-pollution prediction in smart city, deep learning approach. J Big Data 8, 161 (2021). https://doi.org/10.1186/s40537-021-00548-1`
