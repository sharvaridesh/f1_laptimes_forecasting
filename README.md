## **F1 Forecasting Model**

### **Overview**
This project focuses on forecasting lap times in Formula 1 races using machine learning techniques. The model is built upon historical race data, including lap times, pit stops, qualifying results, and race outcomes.

### **Libraries Used**
os
datetime
requests
joblib
pandas
numpy
matplotlib
seaborn
warnings
scikit-learn
xgboost

### **Data Import**
The project utilizes multiple CSV files containing F1 data. The following datasets are loaded for analysis:
lap_times.csv
pit_stops.csv
qualifying.csv
races.csv
results.csv
sprint_results.csv
status.csv
Make sure to change the dir_path to point to the directory where these files are stored.

### **Data Preprocessing**

The preprocessing steps include:
* Handling missing values.
* Converting lap times to a standardized format.
* Aggregating data to extract insights such as total time per driver per race and best positions.
* Merging dataframes to create a comprehensive dataset for analysis.

### **Exploratory Data Analysis**
Visualizations are generated to understand the relationships between variables, including:

* Histograms of lap distributions.
* Correlation heatmaps to identify potential influences on lap times.

### **Model Training**
The model uses the XGBoost algorithm to predict lap times. The training and testing datasets are split by year, with the model trained on data from 2014 to 2022 and tested on data from 2023.

### **Key Metrics**
The performance of the model is evaluated using:

* Root Mean Squared Error (RMSE)
* Mean Absolute Error (MAE)
* Visualizations of actual vs. predicted lap times are also included.

### **Model Saving**
The trained model is saved to a file using joblib for future predictions.

### **Usage**
To use the model for predictions:

* Load the model using joblib.
* Prepare new input data in the same format as the training data.
* Use the predict method of the model.

### **Conclusion**
This project provides a comprehensive framework for predicting lap times in Formula 1 races. The insights gained from the data can be leveraged for strategic decision-making in racing.

