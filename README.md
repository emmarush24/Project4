### Project 4 Salary Prediction

This project focused on creating a predictive model to determine salaries of various data jobs. Raw data was retreived from the Kaggle website which is listed below:

https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023?resource=download

Extracting, manipulating, and cleaning the data was required before analysis could continue. Some examples of this included dropping data from years 2020 and 2021 due to lack of data. Job titles were edited to be more uniformed as slightly different worded titles were used for essentially the same job position. A boxplot was used to determine outliers in the dataset, which were then removed before building the predictive model 

The predictive model which was found a combination of the most accurate/efficient was a Random Forest model. A neural network also produced accurate results, however, required much more computing power (epochs over 500 required) to produce a similar accuracy. Steps to create the Random Forest model included:
-	Changing categorical data to numerical using the get.dummies function
-	Split data into features and target arrays
-	Split data into training and testing sets
-	Create a Standard Scaler and scale data
-	Train/Fit/Predict a RandomForestRegressor model
-	Evaluate predictions to determine accuracy of the model
The model predictions are within 75% accuracy for each of the job titles in the dataset. The code allows users to choose one out of the 4 jobs to receive a predicted salary in the dataset. The input added with the idea that future cleaned data could be added to the dataframe to create a more robust model containing more job titles. 
