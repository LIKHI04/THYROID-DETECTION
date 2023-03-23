# THYROID-DETECTION
Thyroid Disease Detection
Thyroid disease is a very common problem in India, more than one crore people are suffering with the disease every year. Thyroid disorder can speed up or slow down the metabolism of the body.

The main objective of this project is to predict if a person is having compensated hypothyroid, primary hypothyroid, secondary hypothyroid or negative (no thyroid) with the help of Machine Learning. Classification algorithms such as Random Forest, XGBoost and KNN Model have been trained on the thyroid dataset, UCI Machine Learning repository. After hyperparameter tuning XGBoost model has performed well with better accuracy, precision and recall. Application has deployed on Heroku with the help of flask framework.

Webpage Link
For One-User-Input Prediction
Heroku: https://tddoneinput.herokuapp.com/

For Bulk Prediction
Heroku: https://batchprediction.herokuapp.com/

AWS: http://tddbulkprediction-env.eba-uqgwbduj.us-east-2.elasticbeanstalk.com/

Demo
Technical Aspects
Python 3.7 and more
Important Libraries: sklearn, pandas, numpy, matplotlib & seaborn
Front-end: HTML, CSS
Back-end: Flask framework
IDE: Jupyter Notebook, Pycharm & VSCode
Database: Cassandra
Deployment: Heroku, AWS
How to run this app
Code is written in Python 3.7 and more. If you don't have python installed on your system, click here https://www.python.org/downloads/ to install.

Create virtual environment - conda create -n myenv python=3.7
Activate the environment - conda activate myenv
Install the packages - pip install -r requirements.txt
Run the app - python run app.py
Workflow
Data Collection
Thyroid Disease Data Set from UCI Machine Learning Repository.

Link:https://archive.ics.uci.edu/ml/datasets/thyroid+disease

Data Pre-processing
Missing values handling by Simple imputation (KNN Imputer)
Outliers detection and removal by boxplot and percentile methods
Categorical features handling by ordinal encoding and label encoding
Feature scaling done by Standard Scalar method
Imbalanced dataset handled by SMOTE
Drop unnecessary columns
Model Creation and Evaluation
Various classification algorithms like Random Forest, XGBoost, KNN etc tested.
Random Forest, XGBoost and KNN were all performed well. XGBoost was chosen for the final model training and testing.
Hyper parameter tuning was performed using RandomizedSearchCV
Model performance evaluated based on accuracy, confusion matrix, classification report.
Database Connection
Cassandra database used for this project.

Model Deployment
The final model is deployed on Heroku using Flask framework.

User Interface
Single User Input Prediction User Interface
tddone

Batch File Prediction User Interface
Homepage: A very simple UI with single page.
wireframe_tdd_1

User need to upload CSV file and click predict button for prediction to start.
wireframe_tdd_2

User can download their result by clicking download button below.
wireframe_tdd_3

Downloaded CSV file will contain index numer with type of thyroid disease patient is suffering from.
wireframe_tdd_4

User can also download sample csv file for reference.
wireframe_tdd_5

Data in Cassandra Database.
DataInCassandraDB




