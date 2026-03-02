# 🌱 Crop Recommendation System
A Machine Learning web application that predicts the most suitable crop to cultivate based on soil nutrients and environmental conditions. Built with Python, Flask, NumPy, and a trained ML model, this system provides real-time crop recommendations through a simple web interface.

## 📌 Project Overview
###### This project uses soil parameters:
- Nitrogen (N)
- Phosphorus (P)
- Potassium (K)
- Temperature
- Humidity
- pH
- Rainfall

The trained model predicts the best crop based on the given inputs and displays the result instantly The Flask backend loads a serialized ML model using pickle and serves predictions through a POST endpoint.

## 🏗️ Project Structure
###### Crop-Recommendation-System
- app.py                      # Flask application :contentReference[oaicite:1]{index=1}
- crop_prediction_model.ipynb # Model training notebook
- model.pkl                   # Trained ML model (generated after training)
- Crop_recommendation.csv     # Dataset :contentReference[oaicite:2]{index=2}
- templates
    - index.html              # Frontend form :contentReference[oaicite:3]{index=3}
- static
    - styles.css              # Styling file :contentReference[oaicite:4]{index=4}

## ⚙️ Tech Stack
- Python
- Flask
- NumPy
- Scikit-learn
- HTML5
- CSS3

## 🚀 How It Works
- User enters soil and environmental values.
- Data is sent via POST request to /predict.
- Flask converts inputs to float values.
- Model generates prediction.
- Result is rendered back on the same page.
- Prediction route logic is implemented in app.py 

## 🧠 Model Training
The model training process is implemented in: crop_prediction_model.ipynb

###### Typical steps:
- Data preprocessing
- Feature selection
- Model training (e.g., RandomForestClassifier)
- Model serialization using pickle

###### After training:
- pickle.dump(model, open("model.pkl","wb"))

## 📊 Dataset
###### The dataset used for training:
- Crop_recommendation.csv

It contains soil nutrient values and corresponding crop labels.

## 🎯 Features
- User-friendly web interface
- Real-time prediction
- Lightweight Flask backend
- Deployable on cloud platforms
- Easy integration with other agricultural systems

## 📂 Dataset Link

Dataset Source: https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset