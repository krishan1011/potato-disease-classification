# Potato Disease Classification

A deep learning project for detecting potato leaf diseases from plant images. I built a CNN-based classifier that separates healthy leaves from early blight and late blight cases, then packaged it into a web app, mobile app, and API-based inference pipeline.

## Results

The model was trained in the notebook at `training/potato_disease.ipynb` and achieved strong validation performance:

- Validation accuracy: 99.48%
- Validation loss: 0.0257
- Training accuracy: 98.67%
- Training loss: 0.0354
- Best validation accuracy observed: 99.48%
- Classes predicted: Healthy, Early Blight, Late Blight

These results show the model is capable of reliably identifying common potato leaf diseases from image inputs in a production-style pipeline.

## Project Overview

This project combines:

- a React frontend for image upload and prediction
- a Python backend for model inference
- a React Native mobile app for Android/iOS use
- TensorFlow/Keras model training and deployment support
- Google Cloud deployment examples for scalable hosting

## Why this project matters

Plant disease detection is a practical use case for AI in agriculture. This system helps farmers and growers quickly assess crop health from a leaf image, reducing manual inspection time and supporting faster intervention decisions.

## Project Structure

- `frontend/` — web app interface
- `api/` — backend serving code
- `gcp/` — Google Cloud deployment setup
- `mobile-app/` — React Native mobile client
- `training/` — model training notebook and dataset
- `saved_models/` — exported model artifacts
- `tf-lite-models/` — TensorFlow Lite versions
- `test_images_from_internet/` — sample test images

## Tech Stack

- Python
- TensorFlow / Keras
- React
- React Native
- Google Cloud
- REST API deployment

## Setup

### 1. Clone the repository

```bash
git clone https://github.com/krishan1011/potato-disease-classification.git
cd potato-disease-classification
```

### 2. Frontend

```bash
cd frontend
npm install
npm start
```

### 3. Backend API

```bash
cd api
pip install -r requirements.txt
python main.py
```

### 4. Mobile app

```bash
cd mobile-app
npm install
npx react-native run-android
# or
npx react-native run-ios
```

## Model Notes

- The training pipeline is located in `training/potato_disease.ipynb`.
- Model files and large datasets are excluded from version control to keep the repository lightweight.
- Update any cloud credentials, bucket names, and model paths before production deployment.

## Repository Notes

Before deploying publicly, review the following:

- replace placeholder cloud configuration values
- update app package names and identifiers
- set your own signing credentials for release builds
- verify model paths in the serving backend

## License

This project is intended for educational and personal use. Add a preferred open-source license before publishing it publicly.

## Author

Krishan
