# Rain Prediction Using Logistic Regression

Predict whether it will rain based on humidity, temperature, and pressure — in real time!
Built using Python, Logistic Regression, and a real-world Kaggle weather dataset.

## Dataset

We use the long-term weather time-series dataset from Kaggle:
Weather Dataset on Kaggle: [https://www.kaggle.com/datasets/alistairking/weather-long-term-time-series-forecasting](https://www.kaggle.com/datasets/alistairking/weather-long-term-time-series-forecasting)

Data is downloaded programmatically using kagglehub!

## Features Used

| Feature | Description                 |
| ------- | --------------------------- |
| rh      | Relative Humidity (%)       |
| T       | Air Temperature (°C)        |
| p       | Atmospheric Pressure (mbar) |

The target variable is:

* rain: Converted to 0 (no rain) or 1 (rain)

## What This Project Does

* Downloads dataset from Kaggle using kagglehub
* Preprocesses data and selects important features
* Trains a Logistic Regression model
* Evaluates the model with Mean Squared Error
* Takes real-time weather input from the user
* Predicts whether it will rain or not!

## How to Run

1. Install dependencies:
   pip install pandas scikit-learn kagglehub

2. Login to Kaggle:
   kagglehub.login()

3. Run the Python script:
   python rain\_prediction.py

4. Enter real-time values when prompted:
   Enter Humidity (rh %): 85
   Enter Temperature (°C): 25
   Enter Atmospheric Pressure (mbar): 1012

5. Get your prediction:
   🌧️ Prediction: It is likely to RAIN.

## Sample Output

✅ Model trained successfully.
📊 Mean Squared Error (MSE): 0.14

🔎 Enter real-time weather data to predict rain:
☀️ Prediction: No rain expected.

## Future Ideas

* Add a web-based UI using Streamlit or Flask
* Use more features (wind speed, dew point, etc.)
* Try advanced models like Random Forest or XGBoost
* Integrate with live weather APIs

## Author

Kushi B
Project built for learning and demonstration purposes. Contributions welcome!
