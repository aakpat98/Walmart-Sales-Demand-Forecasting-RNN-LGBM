# Walmart Demand Forecasting

This project tackles the challenge of forecasting daily product demand across Walmart stores using real-world sales, pricing, and event data from the M5 Forecasting competition. We evaluate multiple models including LightGBM, LSTM/GRU, and Seq2Seq GRU, balancing forecasting accuracy with speed, interpretability, and deployability.

---

## 📁 Project Structure

| File                             | Description                                               |
|----------------------------------|-----------------------------------------------------------|
| `walmart_forecasting_LGBM.ipynb` | LightGBM model with feature engineering                  |
| `walmart_forecasting_LSTM_GRU.ipynb` | LSTM and GRU sequential models using rolling windows     |
| `walmart_forecasting_seq2seq_GRU.ipynb` | Seq2Seq GRU for one-shot 28-day forecasting              |
| `Presentation Slides.pdf`        | Final presentation delivered to stakeholders             |
| `Project WriteUp.pdf`            | Detailed write-up covering methodology and findings      |

---

## 📦 Data Source

The raw data files (`calendar.csv`, `sell_prices.csv`, `sales_train_validation.csv`, and `sales_train_evaluation.csv`) are not included in this repository due to file size limits.

You can download the full dataset directly from Kaggle:  
🔗 [M5 Forecasting - Accuracy | Kaggle Dataset](https://www.kaggle.com/competitions/m5-forecasting-accuracy/data)

---

## 📌 Objectives

- Forecast item-level sales over a 28-day horizon
- Support smarter inventory and replenishment decisions
- Compare traditional ML (LightGBM) with deep learning models
- Prioritize interpretability, efficiency, and business alignment

---

## 🧠 Models Explored

### ✅ LightGBM
- Fast and interpretable
- Extensive feature engineering (lags, price dynamics, calendar)

### ✅ LSTM & GRU
- Sequence models using 14-day input windows
- Event-aware forecasts with rolling predictions

### ✅ Seq2Seq GRU
- One-shot 28-day global forecast
- Lightweight, fast to train, with transposed sales input

---

## 📊 Key Findings

- GRU outperformed all models with the lowest WRMSSE score
- LightGBM was interpretable but underperformed on sequence trends
- Seq2Seq GRU was the most efficient but less accurate due to limited features

---

## 🏁 Results

- Final GRU model: best trade-off between accuracy, training time, and resource usage
- Presentation and write-up summarize both technical and business insights

---

## 📎 Credits

This project was built as part of a graduate-level course on applied machine learning and time series forecasting. The dataset is from the [M5 Forecasting competition](https://www.kaggle.com/competitions/m5-forecasting-accuracy/overview).

---

## 📜 License

MIT License
