🔥 Fire Type Classification using MODIS Data
📌 Project Overview

This project focuses on deforestation and fire detection in India using the MODIS (Moderate Resolution Imaging Spectroradiometer) dataset. A machine learning model has been trained to classify fire events into different categories based on satellite observations. The project is deployed as an interactive Streamlit web application where users can input fire attributes and receive predictions on the fire type.

🚀 Features

Predicts fire type from satellite parameters.

Uses a pre-trained ML model (best_fire_detection_model.pkl).

Inputs include:

Brightness

Brightness T31

Fire Radiative Power (FRP)

Scan

Track

Confidence level (Low / Nominal / High)

Outputs one of the following fire categories:

🌱 Vegetation Fire

🏞 Other Static Land Source

🌊 Offshore Fire

🛠 Tech Stack

Python

Scikit-learn (for ML model training)

Streamlit (for web app deployment)

NumPy & Joblib (for data handling and model loading)

📂 Project Structure
├── app.py                       # Streamlit app for fire type prediction
├── Classification_of_Fire_Types_in_India_Using_MODIS_dataset.ipynb  # Model training notebook
├── best_fire_detection_model.pkl # Trained ML model
├── scaler.pkl                   # Feature scaler
└── README.md                    # Project documentation

▶️ How to Run

Clone the repository:

git clone https://github.com/ChaitanyaNaik2026/AICTE-deforestation-detection-Final.git
cd AICTE-deforestation-detection-Final


Install dependencies:

pip install -r requirements.txt


Run the Streamlit app:

streamlit run app.py


Open your browser at http://localhost:8501.

📊 Dataset

The dataset used is from MODIS satellite fire observations, focusing on fire occurrences across India.
It includes features such as brightness, temperature (T31), FRP, scan, track, and confidence levels.

🌍 Use Cases

Deforestation detection

Fire monitoring and classification

Environmental impact studies
