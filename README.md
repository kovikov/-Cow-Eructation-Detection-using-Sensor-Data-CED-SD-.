![image](https://github.com/user-attachments/assets/48d7b286-beaa-47fc-b0c3-a973616fd5a5)



# -Cow-Eructation-Detection-using-Sensor-Data-CED-SD-.

Cow Eructation Detection using Sensor Data (CED-SD)

📌 Project Overview

Cow Eructation Detection using Sensor Data (CED-SD) is a data-driven project aimed at analyzing breath temperature and gas concentration (CH₄ and CO₂) in cows. This project leverages sensor data and machine learning to detect eructation (belching) events, a crucial aspect of methane emissions in livestock.

This study provides actionable insights into methane emissions, helping researchers and agricultural experts develop strategies for reducing greenhouse gas contributions from cattle.

🎯 Objectives

Analyze temperature and gas sensor data collected from two cows.

Detect eructation events by identifying spikes in methane concentration.

Develop a predictive model using machine learning to forecast eructation events based on temperature and gas data.

Provide insights into the relationship between CH₄, CO₂, and breath temperature.

📂 Dataset Description

The dataset consists of two types of sensor data collected over a 1-hour period from two cows (Cow A & Cow B):

Thermistor Data (cowA_therm-0.csv, cowA_therm-2.csv, cowB_therm-0.csv, cowB_therm-2.csv)

time_ms: Epoch timestamp in milliseconds.

thermistor_id: Identifier of the thermistor.

raw: Raw voltage readings.

temperature: Temperature in Celsius.

Gas Sensor Data (cowA_gas.csv, cowB_gas.csv)

epoch_ms: Epoch timestamp in milliseconds.

co2: CO₂ concentration in the exhaled breath (%).

co2temp: Temperature in the gas sensor box (°C).

ch4: CH₄ concentration in the exhaled breath (%).

ch4temp: Temperature in the gas sensor box (°C).

🛠️ Methodology

Data Preprocessing

Convert timestamps into a readable format.

Handle missing values using interpolation for gas data and dropping for thermistor data.

Merge gas and thermistor data for each cow using timestamp alignment.

Exploratory Data Analysis (EDA)

Visualized temperature trends over time.

Analyzed CH₄ and CO₂ concentration changes.

Generated correlation heatmaps to study relationships among features.

Eructation Detection Algorithm

Defined CH₄ spike thresholds to classify eructation events.

Identified significant CH₄ increases using a diff-based thresholding method.

Labeled events and visualized methane release patterns.

Machine Learning Model for Prediction

Selected Random Forest Classifier for binary classification (eructation vs. no eructation).

Used temperature and gas concentrations as features.

Evaluated model performance using accuracy, precision, recall, and F1-score.

📊 Key Findings

CH₄ and CO₂ exhibit a moderate positive correlation (0.3), suggesting simultaneous release.

Breath temperature does not strongly influence CH₄ concentration, indicating independent processes.

Certain timestamps showed significant CH₄ spikes, confirming eructation events.

Machine learning predictions achieved high accuracy, validating the effectiveness of the model.

🚀 How to Use

1️⃣ Prerequisites

Ensure you have the following installed:

Python 3.x

Pandas, Matplotlib, Seaborn, Scikit-learn

2️⃣ Running the Code

Clone the repository and run the Jupyter Notebook:

jupyter notebook Cow_Eructation_Detection_using_Sensor_Data__(CED_SD).ipynb

🏆 Conclusion

This project successfully demonstrates how sensor data and machine learning can be used to detect cow eructation events and analyze methane emissions. The insights gained can help in designing sustainable livestock management strategies to reduce greenhouse gas emissions.

For further improvements, deep learning techniques and real-time monitoring systems can be integrated to enhance prediction accuracy and scalability.

📩 Contact



🔗 Project Lead: Adrian Marina🔗 Data Science & AI Expert
