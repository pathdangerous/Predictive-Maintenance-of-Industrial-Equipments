# Predictive Maintenance with XGBoost

## Overview

This repository contains a Python script that demonstrates predictive maintenance using the XGBoost machine learning algorithm. Predictive maintenance is a critical practice in various industries to anticipate when equipment or machinery may require maintenance or servicing, reducing downtime and improving operational efficiency. The script uses a dataset (sample provided) containing sensor readings and equipment details to predict whether maintenance is required for specific equipment.

## Dataset

The dataset, 'Predictive Maintenance.csv', contains the following columns:

- **Equipment**: The type of equipment (e.g., CNC Machine, Robot, Stamping Machine, Conveyor Belt).
- **Timestamp**: The date and time when the sensor readings were recorded.
- **Temperature**: Temperature reading in degrees Celsius.
- **Vibration**: Vibration reading (measurement units vary).
- **Usage_Hours**: Number of hours the equipment has been in use.
- **Lubrication_Status**: The status of lubrication (e.g., Good, Low, Empty).
- **Motor_Current**: Current consumption of the equipment's motor.
- **Pressure**: Pressure reading (measurement units vary).
- **Humidity**: Humidity level (measurement units vary).
- **Conveyor_Speed**: Speed of the conveyor (if applicable).
- **Maintenance_Required**: The target variable indicating whether maintenance is required (Yes/No).

Please ensure that your dataset matches the format and columns described above. You can replace the sample data with your own dataset.

## Requirements

Before using the code, make sure you have the following requirements installed:

- Python (>= 3.6)
- Required Python packages (install them using `pip install`):
  - pandas
  - numpy
  - sklearn (scikit-learn)
  - xgboost
  - seaborn (for data visualization)

## Usage

1. **Data Preparation:**
   - Ensure your dataset matches the format described above and is saved as 'Predictive Maintenance.csv'.

2. **Data Preprocessing:**
   - The script performs data preprocessing, including label encoding for categorical variables like 'Equipment' and 'Lubrication_Status'. The data must be preprocessed in the same way as the sample data.

3. **Model Training:**
   - The script trains an XGBoost classifier to predict maintenance requirements. It also performs hyperparameter tuning using GridSearchCV to find the best model parameters.

4. **User Input:**
   - The script allows users to input sensor data and equipment details for prediction. It provides a simple command-line interface for this purpose.

5. **Predictions:**
   - After receiving user input, the script uses the trained model to predict whether maintenance is required. It provides feedback to the user based on the prediction.

## Customization

You can customize the code by:

- Using your own dataset by replacing 'Predictive Maintenance.csv' with your data.
- Modifying the hyperparameter grid in the hyperparameter tuning section to fine-tune the model.
- Adding more features or sensor readings to improve the model's accuracy.

## Contributors

- Masoom Abbas <masooma@hexaware.com>
- Abhishek Soni <abhisheks@hexaware.com>
- Jaswant Reddy Lekkala <jaswanthreddyl@hexaware.com>
- Sriram Nandakumar <sriramn2@hexaware.com>


## Issues and Feedback

If you encounter any issues or have feedback, please open an issue on this GitHub repository.

