This project showcases the development of a tool designed to predict car prices with a Mean Absolute Error (MAE) of approximately ₦1.8 million, aimed at assisting both buyers and sellers in understanding fair market values. It involved collecting over 2,000 car listings from [cars45](https://www.cars45.com/) and [autochek.africa](https://autochek.africa/ng/cars-for-sale) using Python and Playwright for web scraping. The data underwent thorough cleaning and preparation, including the removal of extraneous characters, standardization of text data, and outlier elimination. Exploratory Data Analysis (EDA) was conducted to identify trends and factors influencing car prices in the target region. 

To predict prices accurately, machine learning models such as Ridge, Decision Tree, and Random Forest Regressors were fine-tuned using GridsearchCV. The project also features a Tableau dashboard for interactive data visualization and a Flask-based web application for end-users to get price estimates. The Random Forest model demonstrated superior performance compared to the other models, achieving the lowest MAE on test and validation datasets. This initiative not only provides a practical solution for pricing cars but also encapsulates the entire data science workflow from data acquisition to model deployment. 


<div style='display:flex;'>
<img src="https://user-images.githubusercontent.com/57121852/213569749-1485cf09-d250-4dcc-8eff-6ede1418aa4b.png">
<img src="https://user-images.githubusercontent.com/57121852/213570571-0afc261a-d7d1-4184-92fe-4366a37aa98c.png" >
</div>

### Dashboard
<img src="https://user-images.githubusercontent.com/57121852/213936600-c760ea7f-321c-4254-a88d-1ecc208e90e5.png" >

##  Model Building
  Firstly, due to the sheer numbers of car models and brands present, **target mean encoding** was used to encode them, while for the remaining categorical features, ordinal and one hot encoding was used as required.  
  Three different models were created and evaluated using Mean Absolute Error.

## Model Performance

The Random Forest model far outperformed the other approaches on the test and validation sets.

Random Forest : MAE = 1.8M  
Decision Tree: MAE =  2.0M  
Ridge Regression: MAE = 2.2M  
  
 ## Productionalization
This step involved creating a Flask web application and API that was hosted on a local webserver. Users can enter and submit information about the vehicle they want to estimate, and the application will return the estimated price.


![image](https://user-images.githubusercontent.com/57121852/213565832-915b6d87-0084-4135-864d-546e8035691c.png)
