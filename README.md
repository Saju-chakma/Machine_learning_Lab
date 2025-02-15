# Machine Learning Lab
Course Supervised by Md. Mynoddin </br>
Author: Saju Chakma, Auntor Chakma</br>
Project name : BD. Weather Prediction using Machine Learning</br>

<h2>Weather Prediction using Machine Learning<h2/>

<h3>Introduction</h3>
<p>Weather prediction is an essential application of data science and meteorology, helping individuals, businesses, and governments make informed decisions based on atmospheric conditions. With the advent of machine learning, predicting weather has become more accurate by leveraging large datasets, statistical models, and real-time data processing. This project implements machine learning techniques to analyze and predict weather conditions effectively.</p>
<h3>Overview </h3>
<p> This project focuses on predicting weather conditions using machine learning techniques. It preprocesses weather data, applies classification models, and evaluates their performance to make accurate predictions.</p>
<h2>Features</h2>
<ul>
    <li>Data preprocessing and feature scaling</li>
    <li>Multiple machine learning models including Random Forest, SVM, XGBoost, and Logistic Regression</li>
    <li>Model evaluation using accuracy, precision, recall, and F1-score</li>
    <li>Data balancing using SMOTE</li>
    <li>Visualization using Matplotlib and Seaborn</li>
</ul>
</ul>

<h2>Installation</h2>
<p>To run this project, install the required dependencies </p>
<h2>Dataset</h2>
<p>The project uses a weather dataset. Ensure the dataset file Chittagong.csv is in the working directory before running the notebook.</p>

<h2>Data Preprocessing</h2>
<ol>
    <li>Load the dataset:</li>
    <li>Read the dataset using 'Chittagong.csv'</li>
    <li>Handle missing values and perform feature scaling using StandardScaler.</li>
    <li>Balance the dataset using SMOTE to address class imbalances.</li>
</ol>

<h2>Model Training</h2>
<ol>
    <li>Split the data into training and testing sets:</li>
    <li>Train models such as Random Forest, SVM, and XGBoost:</li>
    <li>Perform hyperparameter tuning using RandomizedSearchCV.</li>
</ol>

<h2>Visualization</h2>
<ul>
    <li>Use Matplotlib and Seaborn for exploratory data analysis.</li>
    <li>Visualize feature importance and model performance metrics.</li>
</ul>

<h2>Usage</h2>
<p>Run the Jupyter Notebook:</p>
<p>jupyter notebook </p>

<h2>Dependencies</h2>
<ul>
    <li>Python 3.x</li>
    <li>Jupyter Notebook</li>
    <li>NumPy</li>
    <li>Pandas</li>
    <li>Matplotlib</li>
    <li>Seaborn</li>
    <li>Scikit-Learn</li>
    <li>XGBoost</li>
    <li>Imbalanced-learn</li>
</ul>
<h2>Deploy in local server</h2>
<p>Running the Flask API Once the model is trained, the Flask API can be started using: python main.py </p>

<h2>Future Improvements</h2>
<ul>
    <li>Incorporate deep learning models for better accuracy</li>
    <li>Experiment with hyperparameter tuning</li>
    <li>Add real-time weather data integration</li>
</ul>




