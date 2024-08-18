# -_-.
This repository contains the code and project artifacts for the Code Alpha Internship program. It includes implementation details, project documentation, and resources utilized throughout the internship. The codebase features various modules and examples demonstrating key concepts and skills acquired during the internship. The code here will run in jypyter file in python language 
**Project no 1**
**1. Titanic Survival Prediction**
**Objective:**
Predict the likelihood of a passenger surviving the Titanic disaster using a Random Forest Classifier.
Perform detailed exploratory data analysis (EDA) on all columns to understand the factors influencing survival.
**1. Data Preparation:**
**Load the Titanic Dataset:**
Load both the training and test datasets. Ensure the training dataset contains the Survived column as the target variable, while the test dataset does not.
**Handle Missing Data:**
Impute missing values for columns like **Age, Fare, and Embarked and Cabin** in both datasets using strategies like the median or mode.
**Convert Categorical Variables:**
Convert categorical variables like Sex, Embarked, and any other relevant features into numerical values using one-hot encoding or label encoding.
**Feature Engineering:**
**Title Extraction:** Extract titles (e.g., Mr., Mrs., Miss) from the Name column and create a new feature called Title.
**Age Groups:** Create age groups (e.g., children, teens, adults, seniors) to categorize passengers.
**Family Size:** Combine SibSp and Parch into a new feature called FamilySize.
**IsAlone:** Create a binary feature indicating whether a passenger was traveling alone or with family.
**2. Exploratory Data Analysis (EDA):
Survival Rates Analysis:**
Analyze survival rates across different features like Pclass, Sex, Age, Fare, Embarked, and the newly engineered features (Title, FamilySize, IsAlone).
**Distribution Visualization:**
**Histograms and Bar Charts**: Visualize the distribution of survival rates for numerical features (Age, Fare) and categorical features (Sex, Pclass, Embarked).
**Heatmaps:** Show correlations between features and survival to identify key predictors.
**Pie Charts**: Display the proportion of survivors and non-survivors within various groups, such as gender and passenger class.
**Detailed Feature Analysis:**
**Age Groups:** Explore survival rates within the created age groups.
**Title Analysis:** Examine how different titles affected survival rates.
**Family Size and IsAlone:** Analyze how traveling alone or with family influenced survival.
**3. Modeling with Random Forest Classifier:**
**Model Implementation:**
Use the Random Forest Classifier to model the relationship between features and survival using the training dataset.
Train the model on the training data without performing cross-validation or other evaluation techniques.
**Prediction on Test Dataset:**
Use the trained Random Forest model to predict survival on the test dataset.
Output the predictions, typically as a CSV file, containing the PassengerId and the corresponding survival prediction (Survived).
**Project no 2**
**2. Stock Price Prediction Using LSTM**
**Objective:**
Predict future stock prices using a Long Short-Term Memory (LSTM) model, which is well-suited for time-series forecasting.
**Data Collection and Preparation:**
Load historical stock price data, typically including columns like Date, Open, High, Low, Close, and Volume.
Perform data preprocessing, such as normalizing or removing the outliers using IQR from the data(if exist), particularly the 'Close' price, to ensure the LSTM model performs optimally.
Create sequences of data (e.g., 60 days of historical prices) to be used as inputs for the LSTM model.
**Exploratory Data Analysis (EDA):**
Plot the historical stock prices to visualize trends, patterns, and volatility.
Analyze correlations between different features (e.g., volume and price) and identify potential predictors.
Investigate seasonality and other time-based patterns in the stock prices.
**Modeling:**
Implement the LSTM model using a deep learning framework like TensorFlow or Keras.
Define the architecture of the LSTM model, including layers like LSTM cells, Dense layers, and activation functions.
Split the data into training and testing sets, ensuring that the time series nature of the data is respected.
Train the model on the training set, using a suitable loss function and optimizer.
**Evaluation:**
Predict stock prices on the test set and compare them with actual prices.
Use metrics such as Mean Squared Error (MSE) or Root Mean Squared Error (RMSE) to assess model performance.
Visualize the predicted vs. actual stock prices to evaluate the model’s accuracy visually.
