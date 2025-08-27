# Energy Consumption Forecasting using LSTMs  

This project implements a **Long Short-Term Memory (LSTM)** based deep learning model to forecast household energy consumption. The model leverages sequential patterns in time series data to provide accurate predictions, supporting applications in energy optimization and smart grids.  

---

##  Dataset  
- **Source:** UCI Machine Learning Repository (household power consumption).  
- **Sampling Rate:** One-minute interval data over ~4 years.  
- **Features:** Date, time, voltage, current, and power consumption values.  
- **Target:** Daily energy consumption forecast.  

---

##  Model Architecture  
- Input sequences framed from normalized data.  
- LSTM layers to capture short- and long-term dependencies.  
- Dropout and Early Stopping to control overfitting.  
- Output: Predicted energy consumption values.  
- Optimizer: Adam, evaluated with MAE & RMSE.  

---

##  Results  
- The model successfully captured **daily and weekly consumption cycles**.  
- Predictions aligned closely with ground truth, especially for regular usage patterns.  
- **Metrics:** Low MAE and RMSE values confirmed accuracy.  
- Occasional deviations occurred during sudden spikes, showing the model’s sensitivity to irregular behavior.  
<img width="839" height="528" alt="download (2)" src="https://github.com/user-attachments/assets/ef092132-1121-4ffe-bdd4-d4b59e692156" />

---

##  Observations  
The LSTM-based forecasting model demonstrated strong performance in capturing both short-term and long-term energy consumption trends. It effectively recognized seasonality such as daily peaks in the morning and evening, as well as weekly usage cycles. Regularization techniques like dropout and early stopping ensured the model generalized well without significant overfitting. While it struggled to fully capture sudden irregular spikes in energy usage, the overall predictive accuracy was high, making it reliable for real-world applications. With improvements such as bidirectional LSTMs, attention mechanisms, or incorporating external factors like weather data, the system could achieve even greater robustness.  

---

##  How to Run  

1. Clone repository:  
   ```bash
   git clone https://github.com/your-username/energy-forecasting-lstm.git
   cd energy-forecasting-lstm

