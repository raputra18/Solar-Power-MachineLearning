# 🌞 Solar Power Prediction using LDR Sensor Data and Random Forest

### 📘 Overview

This project aims to predict the output power (Watt) of a solar panel concentrator system using machine learning.
The system uses multiple LDR sensors placed on different parts of the panel (left, right, and upper side) to track sunlight intensity, along with voltage and current measurements.

By training a Random Forest Regressor, this project achieves a highly accurate prediction of solar power based on real-world data collected from an IoT-based solar concentrator prototype.

⸻⸻⸻

### ⚙ Dataset Description
The dataset was collected over 3 days, each containing about 150 data samples recorded every 2 minutes in two modes:

  •	Tracking mode: the system automatically follows sunlight.

  •	Static mode: the system stays fixed.

##### Feature ||	Description 

waktu	Timestamp || (HH:MM)\
Hari	|| Day of experiment (1-3)\
Mode ||	Tracking/Static\
LDR_L1, LDR_L2, LDR_L3 ||	Left-side LDR sensor readings\
LDR_R1, LDR_R2, LDR_R3 ||	Right-side LDR sensor readings\
LDR_U1, LDR_U2, LDR_U3, LDR_U4 ||	Upper-side LDR sensor readings\
Arus ||	Current (A)\
tegangan ||	Voltage (V)\
Daya ||	Power (W)\\
##### Total Data: 451 rows

⸻⸻⸻

### 🧠 Machine Learning Pipeline
##### 1.	Import and Clean Data – Handle commas as decimals, convert numeric columns.
##### 2.	Feature Selection – Use 10 LDR sensors + current and voltage as inputs.
##### 3.	Train/Test Split – 80% training, 20% testing.
##### 4.	Model – RandomForestRegressor (n_estimators=100)
##### 5.	Evaluation Metrics:
###### •	R² Score: 0.995
###### •	Mean Absolute Error (MAE): 0.091
###### •	Root Mean Square Error (RMSE): 0.212

⸻⸻⸻

### 📊 Results & Insights
##### •	The model achieved very high accuracy (R² = 0.995), meaning it can effectively predict solar output power.
##### •	Voltage and upper LDR sensors showed the highest influence on power generation.
##### •	This approach can be implemented for real-time energy monitoring or IoT-based solar optimization systems.

⸻⸻⸻

### 🖼 Visualizations
##### •	Predicted vs Actual Power
##### •	Feature Importance Graph
##### •	Time-series comparison (first 100 samples)

#### (All visualizations are automatically generated in the notebook.)

⸻⸻⸻

### 🧰 Tools & Libraries
#### •	Python
#### •	Pandas, NumPy
#### •	scikit-learn
#### •	Matplotlib
#### •	Google Colab

⸻⸻⸻

###  🚀 How to Run
1.	Clone this repository
   git clone https://github.com/<raputra18>/Solar-Power-MachineLearning.git
2. Upload data_putra.csv to your Colab or local folder
3. Run the notebook:
   Prediksi_Daya_Konsentrator_PanelSurya.ipynb
4. View the evaluation results and generated plots.

⸻⸻⸻⸻⸻⸻⸻

## ✍ Author

#### Rahmadi Putra Aji. Undergraduate Student – Instrumentation and Control Engineering (TRIK), Universitas Gadjah Mada
#### 📍 Interested in IoT, Control Systems, and Applied Machine Learning

