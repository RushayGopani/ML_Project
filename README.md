# End-to-End Machine Learning Project

A complete machine learning pipeline covering data ingestion, preprocessing, model training, evaluation, and deployment through a Flask web application.

## Project Overview
This project implements a full ML workflow — from raw data to a working prediction interface — following modular, production-style coding practices rather than a single notebook.

## Tech Stack
- **Language:** Python
- **ML Libraries:** scikit-learn, CatBoost, Pandas, NumPy
- **Web Framework:** Flask
- **Deployment:** AWS Elastic Beanstalk (planned/in progress)

## Project Structure

```text
.
├── src/               # Core ML pipeline code (data ingestion, transformation, model training)
├── notebook/          # EDA and experimentation notebooks
├── templates/         # HTML templates for the Flask app
├── artifacts/         # Saved model and preprocessing objects
├── app.py             # Flask application entry point
├── application.py     # WSGI entry point for deployment
└── requirement.txt    # Project dependencies
```
## How It Works
1. **Data Ingestion** – Loads and splits the raw dataset
2. **Data Transformation** – Handles preprocessing, encoding, and scaling
3. **Model Training** – Trains and evaluates multiple models, selecting the best performer
4. **Prediction Pipeline** – Serves predictions through a Flask web interface

## Running Locally
```bash
pip install -r requirement.txt
python app.py
```

## AWS Deployment

### Elastic Beanstalk Dashboard

![AWS Dashboard](screenshots/aws-dashboard.png)

### Prediction Result

![Prediction Result](screenshots/prediction-result.png)
