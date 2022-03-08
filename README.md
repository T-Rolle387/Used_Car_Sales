# Used_Car_Sales
This notebook is a machine learning project with the goal of predicting the sale price of a used car in the UK. I created this notebook as a side project to learn more about regression models when predicting a quantity using time series data with the year feature converted as a datetime object.

User Interface:

![Screenshot 2022-02-25 201223](https://user-images.githubusercontent.com/79055002/155822718-77b7d8eb-3cca-48ac-96e7-907b01ae0870.png)

1. Problem Definition
   How well can we predict the future sale price of a used vehicle given its characteristics and previous examples of how much similar used cars have sold for?

2. Data
   The data is downloaded from Kaggle at the following link: https://www.kaggle.com/adityadesai13/used-car-dataset-ford-and-mercedes

   Note: This dataset has been obtained from the UK. The predict method would not be accurate of used vehicles within the United States.

   There are four datasets the model was trained on and tested with:

   *audi.csv contains data on used Audi vehicles.
   
   *bmw.csv contains data on used BMW vehicles.
   
   *toyota.csv contains data on used Toyota vehicles.
   
   *ford.csv contains data on used Ford vehicles.
   
    The master.csv file is comprised of these four data sets with a "make" column added to distinguish the vehicles make as a feature. No other feature engineering is noted.

3. Evaluation
   The evaluation metric for this project is the RMSLE(root mean squared log error) between the actual and predicted used car sale prices.

   Simplified, the goal is to minimize prediction errors.

4. Features
  Make
  Model
  Year
  Transmission
  Fuel type
  Tax
  MPG
  Engine size

Feature Importance Visualization:

![feature_importance](https://user-images.githubusercontent.com/79055002/155822823-998c22d4-b07e-4953-aac6-8289b99b45df.png)

   Relationship between input and output:

![input_output_relationship](https://user-images.githubusercontent.com/79055002/155822926-52578958-db31-4b8e-8a44-bfa6f7968cd3.png)

5. Modelling

  A Random Forest Regression model was used to train the data.

  To find out more about Random Forest Regression click here: https://www.askpython.com/python/examples/random-forest-regression

  Cross-Validation Scores:
  
      *Training MAE': 900.1715187801835
      *Test MAE': 1171.20809488802
      *Training RMSLE': 0.07756558813078307
      *Test RMSLE': 0.10309054329424935
      *Training R^2': 0.9773507602618778
      *Test R^2': 0.9644690670642001




