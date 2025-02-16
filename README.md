# Photovoltaic Energy Time Series Forecasting with LSTM and Attention

This project implements an LSTM-based model with and without Attention mechanisms for time series forecasting using photovoltaic energy production data.

## 📌 Project Overview

The script loads photovoltaic energy production data from multiple years, processes it, and trains an LSTM model to predict future values. Two versions of the model are implemented:
1. **LSTM without Attention**
2. **LSTM with Attention**

The results are compared using Mean Squared Error (MSE) and visualization techniques.

## 📂 Dataset

The dataset consists of photovoltaic energy production data from **2010 to 2017**, retrieved from the `50hertz` API. The data is processed to:
- Convert dates into numerical features (Day, Month, Year).
- Normalize the energy production values.
- Split the data into training and testing sets.



## 📜 Usage

### 2️⃣ Model Training

The script trains two models:

#### ✅ LSTM Without Attention
- Uses a single LSTM layer without an attention mechanism.

#### ✅ LSTM With Attention
- Introduces an **Attention** layer to enhance feature focus.

### 3️⃣ Evaluation
- Both models are evaluated using **Mean Squared Error (MSE)**.
- The training loss and validation loss are visualized.

## 📊 Results Visualization

The script plots:
1. **Training and Validation Loss** over epochs.
2. **Predicted vs. Real Data** for the test set.

## 🔍 Key Functions

- `reg_data(df)`: Cleans and processes raw data.
- `split_data(df)`: Splits data into training and testing sets.
- `Split_weekly(df, look_back=7)`: Creates sequences for time series forecasting.
- `ploter_Erreur(hist)`: Plots training history.



## 👨‍💻 Author

- **Mbarek Lamin**
- Contact: `laminmbarek2022@gmail.com`

