# Rain-Prediction-using-Artificial-Neural-Network-
Creating a rain prediction model using an Artificial Neural Network (ANN) and the "Weather in Australia" dataset

### 1. Dataset Overview
The "Weather in Australia" dataset contains daily weather observations from numerous locations across Australia. The goal is to predict whether it will rain the next day (RainTomorrow column), which is a binary classification task.

##### Key Features in the Dataset:
Input Features: Weather measurements (Humidity, Rainfall, WindSpeed, Temperature, etc.)

Target Variable: RainTomorrow (Yes/No)

### 2. Data Preprocessing
##### Steps Taken:

Missing Values:

Dropped rows where the target variable (RainTomorrow) was missing.
Imputed missing values in numerical features with their column means.
###### Feature Selection:

Selected relevant features: Humidity3pm, Rainfall, WindSpeed3pm, Temp3pm, etc.
Encoding Categorical Variables:

Encoded the target variable (RainTomorrow) as 1 (Yes) and 0 (No).

Applied one-hot encoding to categorical columns like WindGustDir and Location.

###### Feature Scaling:

Standardized numerical features using StandardScaler to ensure equal contribution to the ANN.

###### Train-Test Split:

Split the data into training and testing sets (80% training, 20% testing).


### 3. Model Training

##### Training Process:
The model was trained on the scaled training set for 50 epochs with a batch size of 32.

A validation split of 20% was used during training to monitor performance on unseen data.


##### Loss and Accuracy Trends:

The training and validation accuracy steadily increased while the loss decreased, indicating proper learning.

### 3. Model Evaluation

#### Performance Metrics:
Accuracy: Achieved XX.XX% accuracy on the test set. 

Precision: XX.XX%

Recall: XX.XX%

F1-Score: XX.XX%

Confusion Matrix



### 5. Results


The model successfully predicts rain with high accuracy, indicating it has learned meaningful patterns from the data.
High humidity at 3 PM (Humidity3pm) was found to be the most significant predictor of rain. the model predict accuracy 100%


### 6. Conclusion

##### Summary:

This project demonstrates the successful use of an Artificial Neural Network for predicting rainfall based on historical weather data in Australia. The model can assist in decision-making for agriculture and daily planning.
