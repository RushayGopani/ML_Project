End-to-End Machine Learning Project

A complete machine learning pipeline covering data ingestion, preprocessing, model training, evaluation, and deployment through a Flask web application.

Project Overview

This project implements a full ML workflow — from raw data to a working prediction interface — following modular, production-style coding practices rather than a single notebook.

Tech Stack


Language: Python
ML Libraries: scikit-learn, CatBoost, Pandas, NumPy
Web Framework: Flask
Deployment: AWS Elastic Beanstalk (planned/in progress)


Project Structure

├── src/              # Core ML pipeline code (data ingestion, transformation, model training)
├── notebook/         # EDA and experimentation notebooks
├── templates/        # HTML templates for the Flask app
├── artifacts/        # Saved model and preprocessing objects
├── app.py            # Flask application entry point
├── application.py    # WSGI entry point for deployment
└── requirement.txt   # Project dependencies

How It Works


Data Ingestion – Loads and splits the raw dataset
Data Transformation – Handles preprocessing, encoding, and scaling
Model Training – Trains and evaluates multiple models, selecting the best performer
Prediction Pipeline – Serves predictions through a Flask web interface


Running Locally

bashpip install -r requirement.txt
python app.py

Status

Model training pipeline complete. AWS deployment in progress.
