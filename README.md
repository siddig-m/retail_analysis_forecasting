# retail_analysis_forecasting
Exploring various features that affect company wide sales as well as looking to forecast sales for the next fiscal quarter. 

## Inspiration
As someone who has always been interested in the applications data analysis can have on businesses and their performance, this [dataset](https://www.kaggle.com/manjeetsingh/retaildataset) struck my eye and I wanted to explore it more. I was interested in what factors play a part in the company's sales performance and this large dataset seemed like a great opportunity to explore and improve my skills! 

## What it does
The first half of the notebook analyses the dataset, looking for patterns and interactions between sales and other regional data such as the consumer price index, temperature, and holidays. The notebook also features internal data such as the size of the company's specific retail store, the type of departments, as well as the markdowns of products for that given week. The second half of the project aims to build an ARIMA time series model to predict a store's sales for each department for the next fiscal quarter. Using this vast amount of data and forecasting, potential insights could be drawn and explored further in order to improve performance from a company's perspective. 

## How I built it
This project was built in a Jupyter Notebook using Python due to Jupyter Notebook's simplicity and markdown capabilities making for a cleaner and informational presentation of the notebook. Throughout the project, various libraries were used to process the data and get it prepped for time series analysis. Once the best model was chosen according to the Alkaline Information Criterion (AIC), the best ARIMA model was trained on two years of the data and then used to predict the next 3 months in the test set.

## Challenges I ran into
With time-series, the formatting of the data is very important and can lead to many problems if not done correctly. Specifically, the formatting of the time data was difficult to work with as data was selected weekly with inconsistent frequencies making grouping difficult. It was challenging to implement the inconsistencies into the time series format properly. In the end, I  was able to group the days into months and successfully use this for my forecasting model. 

## Accomplishments that I'm proud of
I'm proud to have gained more experience in the data science workflow and exploring a project from start to finish. Not only was I able to improve my coding skills, but I was exposed to more libraries and tools at my disposal and how to use them. With a mean absolute error of about 11501 (relative to high sales), the model is not perfect, however, it does a fair job in predicting sales for the next three months and I look forward to exploring more ways to improve it.  

## What I learned
By completing this project I was able to expose myself to the realm of forecasting and how to apply it in a time-series setting. Also, through the process of this project, I learned about the importance of processing your data before using it in your model. As mentioned above, time series models require specific formatting and given the nature of the data, properly processing the data from the beginning would prove useful. Not to mention I was able to explore new python libraries and sharpen my coding skills.

## What's next for Retail Data Analysis and Sales Forecasting
The next step for this project would be to improve the accuracy of the sales forecast. Exploring other techniques and machine learning algorithms that could perhaps incorporate not only time as a feature but other factors as well may contribute to more accurate predictions. The next step is also to automate the process of applying the model to any department and store of choice that would present a more user-friendly use.
