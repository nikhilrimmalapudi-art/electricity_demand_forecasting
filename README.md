# electricity_demand_forecasting
# Smart Grid Electricity Demand Forecasting ⚡

AI-based electricity demand forecasting system for smart grids using machine learning and contextual time-series features.

---

# 📌 Problem Statement

Electricity demand changes dynamically due to:
- weather conditions
- industrial activity
- human behavior
- weekends and holidays

Incorrect forecasting can lead to:
- power wastage
- overload conditions
- inefficient electricity distribution

This project predicts next-day hourly electricity demand to support smarter load scheduling and smart-grid optimization.

---

# 🚀 Features

✅ Hourly electricity demand forecasting  
✅ Weather-integrated forecasting  
✅ XGBoost machine learning model  
✅ Interactive Gradio dashboard  
✅ Plotly visualization graphs  
✅ RMSE and MAPE evaluation  
✅ Peak demand analysis  
✅ Smart-grid deployment explanation  

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- XGBoost
- Scikit-learn
- Plotly
- Gradio

---

# 📂 Datasets Used

## 1. energy_dataset.csv
Contains:
- historical hourly electricity demand

## 2. weather_features.csv
Contains:
- temperature readings
- weather-related information

Dataset source:
Kaggle Hourly Energy Demand & Weather Dataset

---

# ⚙️ Machine Learning Workflow

```text
Dataset
   ↓
Preprocessing
   ↓
Feature Engineering
   ↓
XGBoost Training
   ↓
Forecast Generation
   ↓
Visualization & Evaluation
```

---

# 📊 Features Used for Forecasting

| Feature | Description |
|---|---|
| Hour | Hour of the day |
| Day of Week | Weekday information |
| Month | Seasonal effect |
| Weekend | Weekend detection |
| Previous Hour Load | Historical demand |
| Previous Day Load | Daily demand pattern |
| Temperature | Weather impact |
| Holiday Encoding | Holiday-like behavior |
| Sin/Cos Hour Encoding | Cyclical time representation |

---

# 🤖 Model Used

## XGBoost Regressor

Full Form:
### Extreme Gradient Boosting

### Why XGBoost?
- fast training
- strong forecasting performance
- handles nonlinear patterns
- efficient on structured datasets

---

# 📈 Evaluation Metrics

## RMSE
Root Mean Squared Error

Measures:
- average prediction error magnitude

Unit:
- MW (Megawatts)

---

## MAPE
Mean Absolute Percentage Error

Measures:
- percentage forecasting accuracy

---

# 📌 Results

| Metric | Value |
|---|---|
| RMSE | ~588 MW |
| MAPE | ~1.37% |

Lower RMSE and MAPE indicate better forecasting performance.

---

# 📉 Dashboard Features

The interactive dashboard includes:

- Predicted Demand KPI
- RMSE KPI
- MAPE KPI
- Peak Demand Hour
- 24-Hour Electricity Forecast Graph
- Actual vs Predicted Comparison Graph
- Model Analysis Section
- Real-World Deployment Section

---

# 🖥️ Dashboard Workflow

1. User selects:
   - Date
   - Hour

2. System automatically:
   - extracts contextual features
   - loads historical demand information
   - performs feature encoding

3. XGBoost model predicts:
   - future electricity demand

4. Dashboard visualizes:
   - forecast waveform
   - actual vs predicted comparison
   - evaluation metrics

---

# 🌍 Real-World Applications

This system can integrate with:
- smart meters
- IEX electricity market data
- MESCOM infrastructure
- weather APIs

Benefits:
- smarter load scheduling
- peak demand management
- efficient electricity distribution
- smart-grid optimization

---

# ⚠️ Model Challenges

The model struggles most during:
- sudden demand spikes
- extreme weather conditions
- unusual holiday behavior

---

# 🔮 Future Improvements

- live weather API integration
- real-time smart meter integration
- deep learning forecasting models
- renewable energy optimization

---

# ▶️ Installation

Install required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn xgboost gradio plotly joblib
```

---

# ▶️ Run the Project

## Step 1: Train the Model

Run:

```bash
python train_model.py
```

This creates:

```text
model.pkl
```

---

## Step 2: Launch Dashboard

Run:

```bash
python app.py
```

---

# 📁 Project Structure

```text
Smart-Grid-Electricity-Demand-Forecasting/
│
├── energy_dataset.csv
├── weather_features.csv
├── model.pkl
├── train_model.py
├── app.py
├── README.md
```

---

# 📸 Output Screenshots

Dashboard includes:
- forecasting waveform
- actual vs predicted comparison
- KPI metrics
- deployment analysis

---

# 👨‍💻 Team

Fusion Techathon Project  
Domain: Energy / Infrastructure

---

# 📌 Conclusion

This project demonstrates how machine learning can support smarter and more efficient smart-grid electricity management through accurate hourly electricity demand forecasting.
