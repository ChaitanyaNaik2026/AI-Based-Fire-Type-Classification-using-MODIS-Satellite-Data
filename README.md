🔥 AICTE Deforestation & Fire Detection – Final Project

This repository contains the final project developed under the AICTE initiative for deforestation and fire detection in India using the MODIS (Moderate Resolution Imaging Spectroradiometer) dataset.

The project includes:

Jupyter Notebooks for data exploration, preprocessing, and model training.

A Streamlit web application for real-time fire type classification.

Pre-trained model and scaler files for quick deployment.

📊 Project Overview

Forest fires are a major cause of deforestation in India. Detecting them early helps mitigate large-scale environmental damage.
This project uses MODIS satellite data and machine learning classification models to identify the type of fire:

🌱 Vegetation Fire

🌊 Offshore Fire

🌍 Other Static Land Source

The trained model is integrated into a Streamlit app where users can input satellite readings and get instant predictions.

🗂️ Repository Structure
AICTE-deforestation-detection-Final/
│
├── Classification_of_Fire_Types_in_India_Using_MODIS_dataset.ipynb   # Notebook with analysis & training
├── FINAL FIRE FOREST DETECTION.ipynb                                  # Additional project notebook
├── FINAL PROJECT.ipynb                                                # Main project notebook
├── app.py / app (2).py                                                # Streamlit app for predictions
├── best_fire_detection_model.pkl                                      # Trained ML model
├── scaler.pkl                                                         # Fitted scaler for preprocessing
├── WEEK-1/                                                            # Weekly work (Week 1)
├── week_2/                                                            # Weekly work (Week 2)
└── README.md                                                          # Project documentation (this file)

⚙️ Requirements

Create a requirements.txt with the following (example):

streamlit
numpy
pandas
matplotlib
scikit-learn
joblib


Install dependencies with:

pip install -r requirements.txt

🚀 How to Run the Streamlit App

Clone this repository:

git clone https://github.com/insanityGG/AICTE-deforestation-detection-Final.git
cd AICTE-deforestation-detection-Final


Install dependencies:

pip install -r requirements.txt


Run the Streamlit app:

streamlit run "app (2).py"


Enter MODIS satellite readings in the input fields:

Brightness

Brightness T31

Fire Radiative Power (FRP)

Scan

Track

Confidence Level (low / nominal / high)

Click Predict Fire Type → The model will output one of:

🌱 Vegetation Fire

🌊 Offshore Fire

🌍 Other Static Land Source

📈 Model Training

Data Preprocessing

Normalization using scaler.pkl

Confidence level mapped as: low=0, nominal=1, high=2

Classifier

Model trained on MODIS dataset features

Saved as best_fire_detection_model.pkl

✅ Example Prediction

Input:

Brightness = 300

Brightness T31 = 290

FRP = 15

Scan = 1

Track = 1

Confidence = nominal

Output:

Predicted Fire Type: Vegetation Fire

🔮 Future Improvements

Add more fire categories for detailed classification.

Expand dataset for better generalization.

Deploy as a web service with API endpoints.

Integrate alert system for forest authorities.
