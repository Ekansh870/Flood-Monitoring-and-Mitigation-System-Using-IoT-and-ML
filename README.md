**Final year Project : Flood Monitoring and Mitigation System (IoT + ML)**

**Objective:**
This project integrates IoT sensors with Machine Learning to build a **Flood Monitoring and Prediction System**.It aims to provide real-time monitoring of water levels, 
rainfall, and temperature, while also predicting the likelihood of floods using a trained Random Forest model.The system can serve as an early warning solution, enabling 
communities and authorities to take timely preventive measures.

**Technologies Used:**
```
**IoT Hardware (for data collection):**
1. ESP32 Microcontroller
2. Ultrasonic Sensor (water level detection)
3. LM35 Temperature Sensor
4. GPRS 900A Module (remote data transmission)
5. LCD 16x2 Display with I²C

**Software & ML Stack:**
1. Python
2. Pandas, NumPy → Data handling
3. Matplotlib, Seaborn → Visualization
4. Scikit-learn → ML model training (Random Forest)
5. Joblib → Model persistence
6. Streamlit → Interactive web application
```

**Workflow:**
```
**1.Data Collection**
Real-time environmental data from IoT sensors.
Historical dataset (flood_20years_dataset.csv) for training.
Data Preprocessing & Model Training (in project.ipynb)
**2.Cleaning and encoding data.**
Training a Random Forest Classifier for flood prediction.
Model saved as flood_prediction_random_forest.pkl.
**3.Streamlit App (main2.py)**
Users can input environmental factors:
    Year
    Month
    Rainfall (mm)
    River Water Level (m)
    Temperature (°C)

Model predicts High Risk or Low Risk of flooding.
Provides warnings and safety instructions accordingly.
```
**How to Run:**
```
1.Clone the repository:
git clone https://github.com/your-username/flood-monitoring-system.git
cd flood-monitoring-system

2.Install dependencies:
pip install -r requirements.txt

3.Run the Streamlit app:
streamlit run main2.py
```

**Impact:**

1. Provides real-time flood monitoring using IoT sensors.
2. Uses Machine Learning to predict flood risks from historical and live data.
3. Acts as an early warning system for communities.
4. Helps in disaster preparedness and mitigation strategies.
