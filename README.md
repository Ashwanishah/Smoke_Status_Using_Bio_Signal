---

# Binary Prediction of Smoker Status Using Bio-Signals

This project uses bio-signal data to predict whether an individual is a smoker or non-smoker through machine learning. The model is integrated into a Flask web application, providing a user-friendly interface for real-time predictions.

## Project Overview

- **Jupyter Notebook**: `Binary Prediction of Smoker Status using Bio-Signals.ipynb` – This notebook covers the complete workflow, including data loading, exploratory analysis, data preprocessing, model training, and evaluation.
- **Dataset**: `train.csv` – A CSV file containing bio-signal features and labels, indicating whether the individual is a smoker or not.
- **Flask Application**: `app.py` – A Python script that implements a Flask web application for deploying the trained model and making predictions based on user input.

## Dataset Details

The dataset (`train.csv`) consists of various bio-signal attributes that can be used to predict smoker status. The features include indicators such as heart rate, age, and other biometric measurements. The target label is binary (1 for smoker, 0 for non-smoker).

### Key Features:

- **Age**: The individual's age.
- **Heart Rate**: Resting heart rate.
- **Bio-Signal Indicators**: Various other signals, like respiratory rate, oxygen saturation, etc.
- **Smoker Status**: The binary target label (1 = smoker, 0 = non-smoker).

## Project Workflow

The project follows a structured pipeline:

### 1. Data Loading

The dataset is loaded into a Jupyter notebook, followed by an initial inspection to understand its structure, check for missing values, and identify the types of features (numerical, categorical).

### 2. Exploratory Data Analysis (EDA)

The next step involves analyzing the distributions of features, visualizing relationships, and identifying any patterns that may aid in predicting smoker status. This includes:
- **Feature Distribution**: Understanding the spread of key features like age and heart rate.
- **Correlation Analysis**: Examining relationships between features to determine any strong predictors.

### 3. Data Preprocessing

Data preprocessing ensures the dataset is ready for machine learning. Steps include:
- **Handling Missing Data**: Filling or removing any missing entries to ensure data completeness.
- **Feature Scaling**: Standardizing or normalizing numerical features to ensure uniformity across the dataset.

### 4. Model Building

Multiple machine learning models are tested, including logistic regression, decision trees, or other classification algorithms. Each model is trained, and its performance is evaluated using metrics such as accuracy, precision, recall, and F1-score.

### 5. Web Application (Flask)

The trained model is deployed as a Flask web application:
- **Input**: Users can enter values for various bio-signals, such as age, heart rate, and other key metrics.
- **Output**: The model returns a prediction of whether the user is likely to be a smoker or non-smoker.

## Installation

To run the project locally:

1. **Clone the repository**:
    Download the project files to your local environment.

2. **Install dependencies**:
    Install the required libraries using:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Flask app**:
    Start the Flask application by running:
    ```bash
    python app.py
    ```

## Usage

- **Access the Web App**: Once the Flask app is running, access it via your web browser. Input the necessary bio-signal values to get predictions.
- **Modify and Experiment**: You can experiment with the notebook to tweak the model, try new algorithms, or optimize the pipeline.

## Project Results

The Jupyter notebook includes the performance results of the trained model, showcasing how well it predicts smoker status based on bio-signal inputs. The model evaluation metrics (accuracy, precision, recall) provide insights into its effectiveness.

## Future Improvements

- **Advanced Feature Engineering**: Additional bio-signal features or derived metrics could enhance model accuracy.
- **Hyperparameter Tuning**: Further tuning of model parameters may yield better results.
- **Scaling Deployment**: Deploying the Flask application to platforms like Heroku, AWS, or GCP for wider accessibility.

---
