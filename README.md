# Potato Disease Detector

AI-powered potato disease detection system for identifying common potato leaf diseases from image uploads using deep learning.

This project combines a web app, mobile app, and model-serving backend to detect diseases such as Early Blight, Late Blight, and Healthy leaves with predicted confidence scores.

## Features

- React web interface for image upload and prediction
- React Native mobile app for Android and iOS
- TensorFlow/Keras model inference pipeline
- Cloud deployment support for GCP hosting
- Image-based classification workflow for field and lab use

## Overview

The app is designed to help farmers, researchers, and plant-health enthusiasts quickly assess potato crop health from leaf images. Users can upload an image and receive a predicted disease label with confidence level.

## Project Structure

- `frontend/` — web app for image upload and classification
- `api/` — backend API code for model serving
- `gcp/` — Google Cloud deployment scripts
- `mobile-app/` — React Native mobile app
- `training/` — training notebook and dataset folder
- `saved_models/` — saved model outputs
- `tf-lite-models/` — TensorFlow Lite model files
- `test_images_from_internet/` — sample images for testing

## Tech Stack

- Python
- TensorFlow / Keras
- React
- React Native
- Material UI
- Google Cloud Storage support

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/krishan1011/potato-disease-classification.git
cd potato-disease-classification
```

### 2. Frontend setup

```bash
cd frontend
npm install
npm start
```

### 3. API setup

```bash
cd api
pip install -r requirements.txt
python main.py
```

### 4. Mobile app setup

```bash
cd mobile-app
npm install
npx react-native run-android
# or
npx react-native run-ios
```

## Model Notes

- Place your trained model in the appropriate folder used by your backend.
- Update any cloud bucket names or model paths in config files before deployment.
- The example configuration can be customized for your own environment.

## Important

Before publishing or deploying, make sure to:

- replace placeholder GCP bucket names
- set your own custom app IDs and package names
- update the app title and branding if needed
- generate your own signing keys for release builds

## License

This project is provided for educational and personal use. Add your preferred license before publishing publicly.

## Author

Krishan
