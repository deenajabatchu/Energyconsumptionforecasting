# Energy Consumption Prediction using Machine Learning
## Time Series Forecasting (LSTM)

This research was done as part of a research seminar course at LAB University of Applied Science (fall 2022).
The report was written using the thesis template of LAB University.

### Abstract

The purpose of this research was to predict energy consumption using the data of Finland's transmission system operator. 
The objective of this project was to test if a machine learning model can yield good enough results in a complex forecasting problem, 
exploring machine learning techniques and developing a data-driven model for forecasting energy.
The data contained 6-year hourly electrical consumption in Finland, and it is a univariate time series, as it is seasonal. 
We used a long-short term memory (LSTM) model to train the data.
The model was evaluated using root mean squared error (RMSE) to be directly comparable to energy readings in the data.
The result shows that electricity consumption can be predicted using machine learning algorithms so we can use the results to deploy renewable energy, 
plan for high/low load days, and reduce wastage from polluting on reserve standby generation.

### Model Implementation
The data was imported from Finland's transmission system operator as a CSV file and then exported to a GitHub repository. 
There was a total number of 52965 observations and 5 variables in this dataset and no missing values were found. 
The minimum load volume is 5341 MWh, and the maximum load volume is 15105 MWh along with an average volume of 9488.750519 MWh. 
The data is univariate time series, where there is a need for one column to present time and another one to present energy consumption. 
For predicting day consumption, data were down-sampled using resample function. 
This function changed the data from hourly frequency to daily frequency.
Training the LSTM model was done using the training set and the validation dataset for testing the results through the training process. 
The learning algorithm worked through the entire training dataset 60 times (Epoch), and the model weights were updated after each batch where the batch size is 20.


📊 Energy Consumption Forecasting and Visualization for Smart Homes
📌 Overview

This project focuses on analyzing historical electricity consumption data and predicting future energy demand using machine learning and deep learning techniques. The goal is to support efficient energy planning in smart homes and smart grid systems.

🎯 Problem Statement

Electricity consumption varies based on time, season, and user behavior. Without accurate forecasting, it leads to energy wastage or shortages.
This project aims to build a system that can predict future electricity consumption using historical data.

💡 Proposed Solution
Data preprocessing and feature engineering
Implementation of Random Forest and LSTM models
Performance comparison using evaluation metrics
Visualization of consumption patterns and predictions
🛠️ Technologies Used
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
TensorFlow / Keras
Power BI (for dashboards)
📂 Dataset
Source: Finland Electricity Consumption Dataset
Total records: ~52,965
Features:
Timestamp
Consumption (MWh)
⚙️ Workflow
Data Collection
Data Preprocessing
Feature Engineering (Month, Day, Lag features)
Data Splitting (Train/Test)
Model Training (Random Forest & LSTM)
Model Evaluation (MSE, RMSE, R²)
Visualization
Future Forecasting
🤖 Models Used
🌳 Random Forest
Handles nonlinear relationships
Fast and stable
🧠 LSTM
Handles time-series data
Captures temporal dependencies
Provides better accuracy
📏 Evaluation Metrics
MSE (Mean Squared Error)
RMSE (Root Mean Squared Error)
R² Score
📊 Results
Random Forest → R² ≈ 0.91
LSTM → RMSE ≈ 0.08
LSTM performed better due to its ability to capture time-based patterns
📈 Result Graphs
🔹 Actual vs Predicted

🔹 Electricity Consumption Over Time

🔹 Year-wise Consumption

🔹 Consumption vs Month (Box Plot)

🔹 Consumption vs Hour (Box Plot)

🔮 Future Scope
Real-time data integration
Weather-based prediction
Hybrid models for higher accuracy
📎 Project Structure
📁 Energy-Forecasting
 ┣ 📁 data
 ┣ 📁 notebooks
 ┣ 📁 images
 ┣ 📄 README.md
 ┣ 📄 requirements.txt
🤝 Acknowledgement

We would like to thank our guide and team members for their support and valuable suggestions throughout the project.

📬 Contact

For any queries or collaboration:
Deenaja Batchu
