# Project 4 Proposal

## Project Title - Machine Learning and US Housing Market Analysis

### Team Members

* [Jhazmine Billups](https://www.linkedin.com/in/jhazmine-billups/)
* [Jason Dugger](https://www.linkedin.com/in/jason-dugger-5277982a/)
* [Megan Goode](https://www.linkedin.com/in/megan-goode-0b419a60/)
* [Bruce Ly](https://www.linkedin.com/in/bruce-ly-8b8295151/)

### Project Description/Outline

We will be using machine learning to predict the price index(Jan 2000=100) of houses in the US housing market using a random forest regression model from sklearn as well as a time series model using PyAF. PyAF is an Open Source Python library for Automatic Forecasting built on top of popular data science python modules: NumPy, SciPy, Pandas and scikit-learn.

As part of our analysis, we will be looking at the following:

* How well does the model predict the price index of houses in the US housing market?
* What are the most important features in predicting the price index of houses in the US housing market?
* How well does the time series model predict the price index of houses in the US housing market?
* Compare the results of the random forest regression model and the time series model.

#### Data Sets to be Used

* [US Housing Market Analysis: Supply-Demand Dynamics | Kaggle](https://www.kaggle.com/datasets/utkarshx27/factors-influence-house-price-in-us)
* [New Privately-Owned Housing Units Completed: Total Units (COMPUTSA) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/COMPUTSA)
* [S&P/Case-Shiller U.S. National Home Price Index (CSUSHPINSA) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/CSUSHPINSA)
* [Housing Inventory Estimate: Vacant Housing Units in the United States (EVACANTUSQ176N) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/EVACANTUSQ176N)
* [Gross Domestic Product (GDP) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/GDP)
* [New Privately-Owned Housing Units Started: Total Units (HOUST) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/HOUST)
* [Interest Rates, Discount Rate for United States (INTDSRUSM193N) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/INTDSRUSM193N)
* [30-Year Fixed Rate Mortgage Average in the United States (MORTGAGE30US) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/MORTGAGE30US)
* [Monthly Supply of New Houses in the United States (MSACSR) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/MSACSR)
* [Median Sales Price of Houses Sold for the United States (MSPUS) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/MSPUS)
* [NASDAQ Composite Index (NASDAQCOM) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/NASDAQCOM)
* [Chicago Fed National Financial Conditions Index (NFCI) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/NFCI)
* [New Privately-Owned Housing Units Authorized in Permit-Issuing Places: Total Units (PERMIT) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/PERMIT)
* [S&P/Case-Shiller 10-City Home Price Sales Pair Counts (SPCS10RPSNSA) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/SPCS10RPSNSA)
* [Total Construction Spending: Residential in the United States (TLRESCONS) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/TLRESCONS)
* [University of Michigan: Consumer Sentiment (UMCSENT) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/UMCSENT)
* [New Privately-Owned Housing Units Under Construction: Total Units (UNDCONTSA) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/UNDCONTSA)
* [Producer Price Index by Commodity: Lumber and Wood Products (WPU08) | FRED | St. Louis Fed](https://fred.stlouisfed.org/series/WPU08)
* [Consumer Price Index for all Urban Consumers | Alpha Vantage API](https://www.alphavantage.co/query?function=CPI&interval=monthly&apikey=demo)
* [Effective Federal Funds Rate | Alpha Vantage API](https://www.alphavantage.co/query?function=FEDERAL_FUNDS_RATE&interval=monthly&apikey=demo)

#### Rough Breakdown of Tasks

* Data Cleaning
* Data Exploration
* Data Analysis
* Data Visualization
* Machine Learning
* Time Series Analysis
* Presentation

#### Machine Learning Model

* Random Forest Regression Model
* Time Series Model

#### Communication Protocol

* Slack
* Zoom
* Google Docs
* Github

#### Project Timeline

* Week 1 - Data Cleaning, Data Exploration, Data Analysis, Data Visualization
* Week 2 - Machine Learning, Time Series Analysis, Presentation

#### Questions for Instructor

* What are the best ways to handle missing data?
* What are the best ways to handle categorical data?
* What are the best ways to handle outliers?
* What are the best ways to handle skewed data?
* What are the best ways to handle overfitting?
* What are the best ways to handle underfitting?

#### Our Findings

The project was a success. We were able to predict the price index of houses in the US housing market with an accuracy of 99.9% using a random forest regression model from sklearn. The most important features in predicting the price index of houses in the US housing market were the following:

* `Mortgage Rate`
* `Oil Price`
* `NASDAQ`
* `Lumber Price Index`
* `Construction`
* `Fed Funds Rate`

We initially used the dataset from Kaggle and were not satisfied with the number of predictions so we increased the resolution by adjusting and imuting missing data. Later, we created a custom dataset by combining data from FRED and Alpha Vantage. The custom dataset provided a much higher resolution and during the testing phase were able to output 108 predictions. Our model predictions were fantastic and we were able to predict the price index of houses in the US housing market with an accuracy of 99%.

After we were satisfied with the RandomForestRegression model we wanted to target future predictions. We used a time series model to predict the price index of houses in the US housing market. Though the time series model was probably not the best model for this data set, it still performed well. After we were satisfied with the time series model we wanted to target future predictions using the RandomForestRegression model. To do this, we implemented a shifted target technique to predict the price index of houses in the US housing market. Upon training the model on our custom dataset we were left with different features in the top 6 most important features. The most important features in predicting the price index of houses in the US housing market were the following:

* `Price Index`
* `CPI`
* `Sales Price`
* `NASDAQ`
* `Lumber Price Index`
* `Construction`

The shifted target technique performed well and we were able to predict the price index of houses in the US housing market 6 months in advance with an accuracy of 99%.

#### Future Considerations

* Try our shifted target technique for a years worth of data and see its performance
* Try a different model for time series analysis
* Explore other data sets

#### Final Project Report

* [Final Project Report](https://docs.google.com/presentation/d/1_d7BWpvVJStsAObi0IUtoNzGzz51GVUMTdhjJULH8NU/edit#slide=id.g35f391192_00)
