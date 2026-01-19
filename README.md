# Flight Fare Prediction

##  Problem Statement
Flight ticket prices vary based on factors such as airline, source, destination, journey date, and number of stops.  
This project predicts flight ticket prices using machine learning to help users and travel platforms estimate fares in advance.
## Objective
-To analyze flight fare data.
-To identify important factors affecting ticket prices.
-To build a machine learning model that predicts flight fares accurately.
## Dataset
- Features:
  - Airline
  - Date of journey
  - Source
  - Destination
  - Route
  - Departure time
  - Arival time
  - Total Stops
  - Additional info
  - Price
## Approach
Data loading and understanding  
- Data cleaning and handling missing values  
- Feature engineering (date extraction, duration conversion, encoding)  
- Exploratory Data Analysis (EDA)  
- Model building and training  
- Model evaluation and comparison  
## Feature Engineering
- Extracted day and month from journey date  
- Converted duration into total minutes  
- Encoded categorical features such as airline, source, and destination  
- Removed irrelevant columns  

## Models Used
- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- xgboost  
## Model Evaluation
The performance of different regression models was evaluated using MAE, RMSE, and R² Score.  
- MAE (Mean Absolute Error): Average absolute difference between predicted and actual prices  
- RMSE (Root Mean Squared Error): Penalizes larger errors more heavily  
- R² Score: Indicates how well the model explains price variability  
##  Model Performance Comparison
| Model | MAE | RMSE | R² Score |
|------|-----|------|----------|
| Linear Regression | 1972.87 | 2863.63 | 0.6197 |
| Decision Tree | 1298.87 | 2187.58 | 0.7781 |
| Random Forest (Tuned) | 1122.30 | 1844.90 | 0.8421 |
| XGBoost (Tuned) | 1169.08 | 1754.99 | 0.8572 |
**XGBoost (Tuned)** achieved the highest R² score and lowest RMSE, indicating strong predictive performance for flight fare estimation.
## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter Notebook  
##  Business Impact
- Helps users estimate flight ticket prices before booking
- Supports travel platforms in fare prediction and pricing strategy
- Reduces uncertainty and improves customer decision-making
