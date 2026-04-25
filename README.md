# House Price Prediction using Machine Learning
Overview

This project implements a machine learning-based system to predict house prices based on various property features such as area, number of bedrooms, bathrooms, and additional amenities.

The solution uses a complete pipeline that integrates data preprocessing, feature encoding, and a regression model to generate accurate price predictions. An interactive user interface is also built using Jupyter widgets for real-time predictions.

Problem Statement

Real estate pricing depends on multiple factors including property size, location features, and amenities. Manually estimating prices is often inaccurate and inconsistent.

This project aims to:

Build a predictive model for estimating house prices
Automate feature processing and encoding
Provide an interactive system for real-time predictions
Key Features
Machine Learning Pipeline
End-to-end pipeline using Scikit-learn
Includes preprocessing and model training in a single workflow
Data Preprocessing
Separation of numerical and categorical features
One-Hot Encoding for categorical variables
Handling unseen categories using handle_unknown="ignore"
Model Training
Random Forest Regressor with 200 estimators
Handles non-linear relationships effectively
Model Evaluation
R² Score for performance measurement
Mean Absolute Error (MAE) for prediction accuracy
Interactive User Interface
Built using ipywidgets
Allows users to input property details
Displays predicted price dynamically
Machine Learning Approach
Model Used
Random Forest Regressor
Features Used

Numerical Features:

Area
Bedrooms
Bathrooms
Stories
Parking

Categorical Features:

Main road access
Guest room availability
Basement
Hot water heating
Air conditioning
Preferred area
Furnishing status
Pipeline Structure
ColumnTransformer for preprocessing
OneHotEncoder for categorical variables
Random Forest for prediction
Dataset Information
Dataset Fields
Feature	Description
area	Size of the house (square feet)
bedrooms	Number of bedrooms
bathrooms	Number of bathrooms
stories	Number of floors
parking	Parking spaces
mainroad	Access to main road
guestroom	Availability of guest room
basement	Basement presence
hotwaterheating	Hot water system
airconditioning	AC availability
prefarea	Preferred location
furnishingstatus	Furnishing condition
price	Target variable
Preprocessing Steps
Identification of feature types
Encoding categorical features
Train-test split (80/20)
Integration into a unified pipeline
Model Performance
R² Score: Indicates how well the model explains variance
Mean Absolute Error: Measures average prediction error

These metrics ensure the model provides reliable predictions for unseen data.

Installation and Setup
Step 1: Clone the Repository
git clone https://github.com/your-username/House-Price-Prediction.git
cd House-Price-Prediction
Step 2: Install Dependencies
pip install -r requirements.txt
Step 3: Run the Notebook

Open the notebook in Jupyter or Google Colab and execute all cells.

Usage
Upload the dataset CSV file
Train the model using the pipeline
Enter property details in the UI
Get real-time predicted house price
Project Structure
House-Price-Prediction/
│
├── House Price Prediction.ipynb
├── data.csv
├── README.md
Limitations
Model depends on dataset quality
Does not include location-based geospatial features
Limited to structured input data
Future Improvements
Integration of location-based features (latitude/longitude)
Use of advanced models like Gradient Boosting or XGBoost
Deployment as a web application
Integration with real estate APIs
Learning Outcomes

This project demonstrates:

Data preprocessing using pipelines
Handling categorical data with encoding
Regression model development
Model evaluation techniques
Building interactive ML interfaces
Author

Jiten Hudda
B.Tech CSE (Artificial Intelligence)
Amity University Punjab

Conclusion

This project showcases the application of machine learning in real estate price prediction by combining preprocessing, modeling, and user interaction into a complete system.
