# 🌞 Solar Power Prediction using LDR Sensor Data and Random Forest

### 📘 Overview

This project aims to predict the output power (Watt) of a solar panel concentrator system using machine learning.
The data was collected from an IOT-based vertical solar concentrator that uses LDR sensors, ESP32-Dev-Kit, and viltage/current measurements.

A Random Forest Regressor model is trained to predict solar panel power output with very high accuracy.
This work demonstrates how sensor-based solar systems can be integrated with data analitycs for intelligent performance prediction

⸻⸻⸻

### ⚙ Dataset Description
The dataset was collected over 3 days, with approximately 150 records per day at 2-minute intervals. Each day includes two modes:

#### •	Tracking mode: 
the system automatically follows sunlight.

#### •	Static mode: 
the system stays fixed.

#### Feature ||	Description 

waktu	|| Timestamp (HH:MM)\
Hari	|| Day of experiment (1-3)\
mode ||	Tracking/Static\
LDR_L1, LDR_L2, LDR_L3 ||	Left-side LDR sensor readings\
LDR_R1, LDR_R2, LDR_R3 ||	Right-side LDR sensor readings\
LDR_U1, LDR_U2, LDR_U3, LDR_U4 ||	Upper-side LDR sensor readings\
Arus ||	Current (A)\
tegangan ||	Voltage (V)\
Daya ||	Power (W)\

**Total Data: 450 samples**

⸻⸻⸻

### 🔍 Exploratory Data Analysis (EDA)
•	Left and right LDR sensors show consistent light intensity differences throughout the day.\
•	Strong correlation is found between voltage and output power, confirming the physical relationship.\
•	The upper LDR sensors provide valuable sunlight direction information for tracking accuracy.

⸻⸻⸻

### 🧠 Machine Learning Pipeline
1.	Data Cleaning - Fix decimal formats and convert numeric values.
2.	Feature Selection – 10 LDR sensors + current and voltage as features.
3.	Train/Test Split – 80% training, 20% testing.
4.	Model – RandomForestRegressor (n_estimators=100)
5.	Evaluation Metrics:\
•	R² Score: **0.995**\
•	Mean Absolute Error (MAE): **0.091**\
•	Root Mean Square Error (RMSE): **0.212**

⸻⸻⸻

### 📊 Results & Insights
•	The model predics power output with **very high accuracy**.\
•	The most influential features are **voltage** and **upper LDR sensors**.\
•	This model can be integrated into **real time solar monitoring system** for power estimation and performance analysis.

⸻⸻⸻

### 🖼 Visualizations
•	Predicted vs Actual Power\
•	Feature Importance Graph\
•	Time-series comparison (first 100 samples)

(_All visualizations are automatically generated in the notebook_.)

⸻⸻⸻

### 🧰 Tools & Libraries
**•	Python**\
**•	Pandas, NumPy**\
**•	scikit-learn**\
**•	Matplotlib**\
**•	Google Colab**

⸻⸻⸻

###  🚀 How to Run
1.	Clone this repository:\
   git clone https://github.com/raputra18/Solar-Power-MachineLearning.git
2. Install dependencies:\
   pip install -r requirements.txt 
3. Open the notebook:\
   notebooks/model_training.ipynb
4. Uploud your data_putra.csv file inside the /data/folder if not already included. 
5. Run all cells in Google Colab or Jupyter Notebook to see results and visualizations.

⸻⸻⸻

### 🚧 Future Work
•	Integrate with **Firebase IoT dashboard** for real-time prediction.\
•	Compare model performance with **Neural Network regression** or **XGBoost**.\
•	Apply model on **different weather conditions** for robustness testing.


⸻⸻⸻⸻⸻⸻⸻

## ✍ Author

#### Rahmadi Putra Aji 
#### Undergraduate Student – Instrumentation and Control Engineering (TRIK), Universitas Gadjah Mada
#### 📍 Passionate about IoT, Control Systems, and Applied Machine Learning
📧 rahmadi.putra.aji@mail.ugm.ac.id


