<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Weather Prediction for Chittagong</title>
</head>
<body>
    <h3>This Project is supervised By</h3>
    <strong>Md Mynoddin Sir,</strong><br>
    <strong>Assistant Professor,</strong><br>
    <strong>Department of CSE, RMSTU.</strong>

    <h1>Weather Prediction for Chittagong</h1>
    <p>A machine learning-based <strong>weather prediction system</strong> designed to forecast weather conditions in <strong>Chittagong, Bangladesh</strong> using historical meteorological data. The project applies <strong>advanced data preprocessing, hyperparameter tuning, and ensemble learning</strong> to enhance prediction accuracy and generalization. A <strong>Flask web application</strong> with a structured <strong>Bootstrap UI</strong> allows users to input weather parameters and obtain real-time predictions.</p>

    <hr>

    <h2>Table of Contents</h2>
    <ul>
        <li><a href="#introduction">Introduction</a></li>
        <li><a href="#dataset">Dataset</a></li>
        <li><a href="#methodology">Methodology</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#usage">Usage</a>
            <ul>
                <li><a href="#training-the-model">Training the Model</a></li>
                <li><a href="#running-the-flask-application">Running the Flask Application</a></li>
                <li><a href="#using-the-web-interface">Using the Web Interface</a></li>
            </ul>
        </li>
        <li><a href="#results">Results</a></li>
        <li><a href="#future-enhancements">Future Enhancements</a></li>
    </ul>

    <h2 id="introduction">Introduction</h2>
    <p>Weather forecasting is a crucial component in various sectors, including agriculture, transportation, and disaster management. This project leverages <strong>historical weather data</strong> to develop a predictive model capable of classifying weather conditions into <strong>Rain, High Temperature, Normal Temperature, or Cold</strong>.</p>
    <p>By integrating <strong>RandomizedSearchCV</strong>, <strong>SMOTE</strong>, and a <strong>stacking ensemble</strong>, the model achieves <strong>higher accuracy</strong> while minimizing the risks of overfitting. A <strong>Flask-based web application</strong> provides a structured interface where users can input relevant weather parameters and obtain real-time predictions with confidence scores.</p>

    <hr>

    <h2 id="dataset">Dataset</h2>
    <p>The dataset used for this project is obtained from <strong>Mendeley Data</strong>, consisting of <strong>daily meteorological records</strong> for Chittagong.</p>
    <ul>
        <li><strong>Temperature (°C)</strong></li>
        <li><strong>Rainfall (mm)</strong></li>
        <li><strong>Humidity (%)</strong></li>
        <li><strong>Sunshine (hours)</strong></li>
        <li><strong>Date (year, month, day)</strong></li>
    </ul>
    <p>Download the dataset from: <a href="https://data.mendeley.com/datasets/tbrhznpwg9/1">Mendeley Data - Chittagong Weather</a></p>

    <h2 id="methodology">Methodology</h2>
    <h3>Data Preprocessing</h3>
    <ul>
        <li><strong>Handling Missing Values:</strong> Median imputation for numerical features.</li>
        <li><strong>Feature Engineering:</strong> Converting Year, Month, and Day into a single Date feature.</li>
        <li><strong>Class Imbalance Handling:</strong> <strong>SMOTE</strong> ensures balanced class representation.</li>
    </ul>

    <h3>Model Development & Hyperparameter Tuning</h3>
    <ul>
        <li><strong>Algorithms Implemented:</strong> Random Forest, Gradient Boosting, XGBoost, SVM, Logistic Regression.</li>
        <li><strong>Optimization Strategy:</strong> RandomizedSearchCV with Stratified K-Fold cross-validation.</li>
    </ul>

    <h3>Stacking Ensemble</h3>
    <p>A <strong>StackingClassifier</strong> is implemented to combine multiple models and improve predictive performance.</p>

    <h2 id="installation">Installation</h2>
    <h3>Step 1: Clone the Repository</h3>
    <pre>
git clone https://github.com/saju-chakma/weather_prediction_chittagong.git
cd weather_prediction_chittagong
    </pre>

    <h3>Step 2: Create and Activate a Virtual Environment</h3>
    <pre>
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
    </pre>

    <h3>Step 3: Install Dependencies</h3>
    <pre>
pip install -r requirements.txt
    </pre>

    <h2 id="usage">Usage</h2>
    <h3 id="training-the-model">Training the Model</h3>
    <p>To train the model and build the ensemble classifier, execute:</p>
    <pre>
python train_model.py
    </pre>

    <h3 id="running-the-flask-application">Running the Flask Application</h3>
    <p>To launch the Flask web application, execute:</p>
    <pre>
python app.py
    </pre>
    <p>By default, the application will run on: <a href="http://127.0.0.1:5000">http://127.0.0.1:5000</a></p>

    <h3 id="using-the-web-interface">Using the Web Interface</h3>
    <ol>
        <li>Enter weather parameters: Rainfall, Temperature, Humidity, Sunshine, Date.</li>
        <li>Click "Predict Weather".</li>
        <li>View Predictions.</li>
    </ol>

    <h2 id="results">Results</h2>
    <p>The <strong>stacking ensemble</strong> consistently outperforms individual models by leveraging multiple classifiers.</p>
    <ul>
        <li><strong>Higher Accuracy:</strong> The ensemble achieves superior classification accuracy.</li>
        <li><strong>Reduced Overfitting:</strong> Early stopping and cross-validation strategies prevent overfitting.</li>
    </ul>

    <h2 id="future-enhancements">Future Enhancements</h2>
    <ul>
        <li>Integration of Deep Learning Models - Implement LSTM-based RNNs.</li>
        <li>Real-Time Weather API Integration.</li>
        <li>Automated Model Retraining.</li>
    </ul>
</body>
</html>
