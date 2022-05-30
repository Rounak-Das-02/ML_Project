# Machine Learning Project - 3rd Semester UnderGrad

## Second Hand Car Price Prediction

Faculty incharge - Dr. Sanatan Sukhija

Project Abstract :-

While buying a used-car/ second-hand car, it is difficult to know whether the price posted in the ad is worth the actual price or not. Moreover, there are many factors that determine the worth of a car. Our project is to make a prediction model to determine the price of used cars. We will also be predicting the price of the car based on its location.

Source of Dataset- https://www.kaggle.com/austinreese/craigslist-carstrucks-data


 Steps to run it (One Drive link) : 

 Requirements : sklearn, numpy, pandas, xgboost==0.90

        1.  The data is uploaded on onedrive link, but running the files in colab is recommended.

        2.  Run data_preprocessing.ipynb file :
        The entire dataset is loaded first from google drive in colab.
        Irrelevant data are removed and NaN values are handled using IterativeImputer!
        Categorical and Numerical values are handled separately. Finally the dataset is saved as FinalVehiclesData.csv

        3.  Run model_training.ipynb file :
        FinalVehicles.csv file is loaded. The categorical data are encoded by LabelEncoder and saved as joblib file. All other features are normalized using their max values in the dataset.
        Finally models like Linear Regression, KNN, RandomForestRegressor and XGBoost are run and the model with lowest RMSE is chosen. In this case, XGBoost made it to the front.

        4.  Run prediction.ipynb :
        There are a couple of features to be inputted by the user.
        The fifth cell contains all the values of the categorical features to choose from. For choosing the feature `region` and `model`, two csv files named - model.csv and region.csv are uploaded. 
        To ease up the process of finding latitude and longitude, a free API is used. Only zip code is needed to be filled.
        Fill up all the details in the 6th cell.
                1.  Continue running the following cells.
                    Mention the model path and run the last cell. It should give you the price in Dollars!


Team Members : 

Mrinmoy Das - SE20UCSE101
Nitya Varshini Gaddala - SE20UCSE117
Rounak Das - SE20UCSE149
Bhavya Chaurasia - SE20UECE011
Likhith Gadde - SE20UECE039