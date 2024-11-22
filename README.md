# Flight Prediction
![image](https://github.com/user-attachments/assets/01af3c08-097f-4c7a-b0ad-70fe8fe547e2)
## Overview
This project aims to predict flight ticket prices based on various features such as airline, journey date, route, and stops using Linear Regression. The dataset contains flight details, including departure and arrival times, route, total stops, and additional information.

## Features in the Dataset
        Airline (object):The name of the airline providing the flight.
        Date_of_Journey (object):The date on which the journey takes place, stored as a string.
        Source (object): The starting point of the journey.
        Destination (object):The endpoint of the journey.
        Route (object):The route taken by the flight, showing stopovers (10682 non-null).
        Dep_Time (object):The departure time of the flight, stored as a string.
        Arrival_Time (object):The arrival time of the flight, stored as a string.
        Duration (object):The duration of the flight in hours and minutes, stored as a string.
        Total_Stops (object):The number of stops between the source and destination (10682 non-null).
        Additional_Info (object):Additional information about the flight (e.g., meal type, layovers).
        Price (int64):The price of the flight ticket (target variable).
## Steps Involved in the Project
    1. Data Preprocessing
        Missing Values: Handle missing values in Route and Total_Stops.
        Feature Transformation: Convert categorical columns (Airline, Source, Destination, etc.) into numerical format using OneHotEncoding or LabelEncoding.
        Date & Time Features: Extract day and month from Date_of_Journey,Extract hour and minute from Dep_Time and Arrival_Time,Convert Duration into a numeric format by separating hours and minutes.
    2. Exploratory Data Analysis
        Visualize relationships between features and the target variable (Price) to identify trends.
        Check for correlations between features to improve feature selection.
    3. Model Building
        * Use Linear Regression to predict flight ticket prices.
        * Split the dataset into training and testing sets.
        * Evaluate the model using metrics like:
            * Mean Absolute Error (MAE)
            * Mean Squared Error (MSE)
            * R² Score
