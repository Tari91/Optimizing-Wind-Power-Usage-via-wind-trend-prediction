# Wind Power Optimization via Wind Trend Prediction

This project demonstrates how to **optimize wind power usage** by forecasting wind speed trends using synthetic data and a deep learning model (LSTM). It also includes a rule-based logic for making energy usage decisions such as storing excess energy or activating backup power.

## 📊 Project Components

- **Synthetic Data Generation**: Simulates hourly wind speed data for 1 year using sinusoidal patterns with noise.
- **Data Normalization**: Prepares the data for input into the neural network.
- **LSTM Time-Series Model**: Predicts future wind speeds using historical data.
- **Trend-Based Optimization**: Makes simple operational decisions based on wind predictions.
- **Excel Export**: The generated data is saved in an Excel file (`synthetic_wind_speed_data.xlsx`).

## 📁 Files Included

- `wind_power_prediction.py`: Main script that handles data generation, training, prediction, and optimization.
- `synthetic_wind_speed_data.xlsx`: Excel sheet containing 1 year of hourly synthetic wind speed data.
- `README.md`: Project description and usage instructions.

## 📦 Requirements

Install the required packages via pip:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow
🚀 How to Run
Run the Python script:

bash


python wind_power_prediction.py
It will:

Generate synthetic data.

Train an LSTM model on wind speed time series.

Predict future wind speeds.

Apply simple rule-based optimization decisions.

Display prediction plot and save wind data to Excel.

⚡ Optimization Logic
A simple logic determines the energy strategy:

Wind speed > 12 m/s: Store excess energy.

Wind speed < 5 m/s: Activate backup power.

Otherwise: Normal operation.

📈 Sample Output
A line plot comparing actual vs predicted wind speed.

Hourly strategy recommendations based on predictions.

🔧 Future Work
Integrate real-world wind farm data.

Model energy storage system (battery).

Apply advanced optimization (e.g., Linear Programming, RL).

Web dashboard to visualize trends and strategies.

🧠 Author
Tarinabo williamtarinabo@gmail.com
