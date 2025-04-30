
# ✈️ Flight Price Prediction using Machine Learning
This project predicts airline ticket prices based on flight and booking details. The goal was to build a robust regression pipeline that can handle real-world data and deliver accurate price predictions using traditional machine learning techniques.

# 🧠 Objective
Predict the price of flight tickets using features such as airline, source, destination, duration, stops, and more.
Apply data cleaning, feature engineering, and regression modeling.
Focus on RMSE (Root Mean Squared Error) and R² score as primary evaluation metrics.
# 📊 Dataset
Source: Kaggle – Flight Fare Prediction Dataset
Total records: ~10,000 flight bookings
Features: Airline, Date of Journey, Source, Destination, Route, Duration, Total Stops, Additional Info, Price
# 🧪 Workflow
Phase 1: Data Exploration & Cleaning
Inspected and visualized data for missing values and outliers.
Cleaned and preprocessed features (e.g., converted dates, extracted durations, handled categorical variables).
Phase 2: Feature Engineering
Created new features (e.g., journey day/month, total travel time).
Encoded categorical variables using one-hot encoding.
Phase 3: Model Building & Evaluation
Tried multiple regression models (Linear Regression, Random Forest, etc.).
Used GridSearchCV for hyperparameter tuning.
Evaluated models using RMSE and R² score.
Phase 4: Final Model Selection
Selected the best-performing model (e.g., Random Forest Regressor) based on validation results.
# 🧱 Final Model Pipeline
python
Copy Code
Pipeline([
  ('preprocessing', ColumnTransformer([...]),  # e.g., OneHotEncoder, StandardScaler
  ('regressor', RandomForestRegressor())
])
# 📈 Results
Metric	Value (approx.)
RMSE	~1,800 INR
R²	~0.85
The model explains about 85% of the variance in ticket prices.
Low RMSE indicates good predictive accuracy on test data.
# 💾 Model Persistence
Trained pipeline saved using joblib for easy reuse and deployment.
Ready for integration into web apps or further tuning.
# ✅ Conclusion
This project demonstrates the effectiveness of classical machine learning for price prediction tasks. Careful data cleaning, feature engineering, and model selection led to a robust solution with strong predictive performance.

# 📁 Files Included
Flights_price_prediction_code.ipynb — Full code, EDA, modeling, and results
flight_fare.csv
# 🚀 Future Improvements

Explore advanced models (e.g., XGBoost, LightGBM)
Add more features (e.g., holiday/seasonality, demand trends)
Deploy as a web API or integrate into travel platforms


# 💾 Screen Shots
<img width="703" alt="Screenshot 2025-04-30 at 12 30 32 PM" src="https://github.com/user-attachments/assets/816e787a-4c4a-4511-a912-d44297e7ff49" />
<img width="702" alt="Screenshot 2025-04-30 at 12 31 19 PM" src="https://github.com/user-attachments/assets/89338354-0fb3-43a2-b3a5-2d6c93edbc2d" />
<img width="700" alt="Screenshot 2025-04-30 at 12 31 42 PM" src="https://github.com/user-attachments/assets/41c3a01e-3000-46cc-8405-a5015b2fbe78" />
<img width="629" alt="Screenshot 2025-04-30 at 12 32 16 PM" src="https://github.com/user-attachments/assets/5b0f4187-ccf9-4343-a40d-cb60e40c5b1a" />
<img width="619" alt="Screenshot 2025-04-30 at 12 32 59 PM" src="https://github.com/user-attachments/assets/3794c705-13a6-481f-bf41-ccf6f4dcfae6" />

