This project aims to build a Machine Learning Regression to predict Youtube adview counnt based on other youtube matrics.  


# YouTube AdView Prediction

Project Overview
This project focuses on developing a Machine Learning Regression Model to predict YouTube ad view counts based on various YouTube metrics. The objective is to analyze video engagement statistics and utilize regression techniques to forecast ad views accurately.


Technologies Utilized
•	Programming Language: Python
•	Libraries:
o	Data Processing: Pandas, NumPy
o	Data Visualization: Matplotlib, Seaborn
o	Machine Learning: Scikit-learn
o	Deep Learning: Keras, TensorFlow


Dataset Description
The dataset consists of multiple attributes that contribute to YouTube video engagement, including:
•	Views
•	Likes
•	Dislikes
•	Comments
•	Category
•	Duration
•	AdView Count (Target Variable)
Data preprocessing steps such as handling missing values, outlier removal, and feature engineering were applied to ensure data quality and improve predictive accuracy.


Exploratory Data Analysis (EDA)
•	Data Cleaning: Addressing missing values and removing anomalies.
•	Feature Engineering: Converting categorical variables and transforming duration into a numerical format.
•	Data Visualization: Implementing histograms, correlation heatmaps, and distribution plots to understand data patterns.

Model Training and Evaluation
The following regression models were trained and evaluated:
1.	Linear Regression
2.	Support Vector Regression (SVR)
3.	Decision Tree Regressor
4.	Random Forest Regressor
5.	Artificial Neural Network (ANN)


Model Evaluation Metrics
Each model was assessed based on the following evaluation criteria:
•	Mean Absolute Error (MAE)
•	Mean Squared Error (MSE)
•	Root Mean Squared Error (RMSE)
The Decision Tree Regressor and ANN models demonstrated superior performance compared to other models.


Model Deployment
•	The Decision Tree Regressor model was saved as decisiontree_youtubeadview.pkl using joblib.
•	The Artificial Neural Network (ANN) model was saved as ann_youtubeadview.h5 using Keras.
How to Execute the Project
1.	Clone the repository:
    git clone https://github.com/your-username/your-repo-name.git  
    cd your-repo-name  
2.	Install dependencies:
    pip install -r requirements.txt  
3.	Run the script:
    python youtube_adviewprediction.py 

 
Future Scope
•	Implementing feature selection techniques to enhance model accuracy.
•	Performing hyperparameter tuning for optimal model performance.
•	Deploying the model as a web application for real-time predictions.
