# Project Portfolio
#### Yichen Wang
#### Analytics Consultant at SVDC | Analytics Consultant at Air Transat | McGill University | Master of Management in Analytics(MMA) '22
https://www.linkedin.com/in/yichenwang1114/

# Table of Content <br>
## Topics (with links to corresponding repositories):
1. [MySQL dbms](#mysql-dbms)
2. [R Programming](#r-programming)
3. [Python](#python)
4. [Excel](#excel)

## [MySQL dbms](https://github.com/Yichen-Wang-666/MySQL-dbms)
### 1. [Bumble Database Simulation](https://github.com/Yichen-Wang-666/MySQL-dbms/tree/main/Bumble%20Database%20Simulation)
A dating app database is inspired by the functionality of Bumble, a free dating app that rapidly got popular recently. We aim to build a **subscription-based model database** that enables us to create value from the data, i.e. to perform:
- user targeting/user analytics
- financial metrics
- performance metrics <br>

**The ERD of the database is shown below**
![image](https://user-images.githubusercontent.com/59845928/184709915-4a170d12-bf6e-47cf-82ad-d624d764daab.png)
20 queries are generated to explore both functionalities of the app and various metrics. These queries are divied into 5 different themes, with examples shown below:
#### 1.  App Features <br> 2. Feature exploration <br>3. Matching Metrics<br> 4. Performance Metrics<br> 5. User Targeting

_Example Query:_<Br>
<img src="https://user-images.githubusercontent.com/59845928/184714056-a0774211-c522-4c97-80ed-bda4cef3c260.png" width="500" height="200"><br>
<img src="https://user-images.githubusercontent.com/59845928/184714277-c0a2284a-3a3a-450d-b4e7-f65e8af64c5e.png" width="500" height="350"><br>

For more details, please visit Bumble Database Simulation Folder to see the report and files.
  
### 2. [La Ronde Analysis](https://github.com/Yichen-Wang-666/MySQL-dbms/tree/main/La%20Ronde%20Analysis)
Several datasets including the ride history, ticket, customer, facility and so on of La Ronde, one of the famous amusement part in Montreal, are provided. This project aims to create a database to store all the datasets and come up with different queries to exploit values from the massive amount of data.

**The ERD of the database is shown below**<br>
<img src= "https://user-images.githubusercontent.com/59845928/184717931-d8995621-ceb5-4afb-80c3-176d38759965.png" width="700" height="500">

_Example Query:_<br>
<img src= "https://user-images.githubusercontent.com/59845928/184719095-910394fc-acdd-4b9d-8dbf-504fa56f0b6d.png" width="600" height="400"><br>
<img src= "https://user-images.githubusercontent.com/59845928/184719249-1a448936-7b65-4bd4-9ec5-85486421bf6f.png" width="600" height="360"><br>

## [R Programming](https://github.com/Yichen-Wang-666/R-Programming-Projects)
### 1. [Artea Case Analysis](https://github.com/Yichen-Wang-666/R-Programming-Projects/tree/main/Artea%20Case%20Analysis)
In the Artea Case Analysis, they ran the A/B testing to test the coupon promotion strategy because the proportion of those who actually made a purchase is much lower than they expected even the engagement metrics indicate nothing wrong. By doing analysis using R, we mainly focus on several key problems:
#### 1. Does the discount coupons work? <br>
To examine whether the discount coupons work, we ran a **descriptive analysis** on the indicative variables, trans_after, and revenue_after, for the effectiveness of coupons and compared the result across two groups. The result is listed in the following table:
  
<img src="https://user-images.githubusercontent.com/59845928/184964481-c1e92247-3fb8-466d-8d9e-69d42231ce3a.png" width="600" height="100"><br>
Based on the result above, we observed that the percentage of customers who made a ransfer after receiving coupons is 12.39% while the percentage of customers who ade a transfer without a coupon is 10.69%. The difference is not substantial. Moreover, we conducted **hypothesis testing** with the null hypothesis being: the revenue is not significantly different between two groups of customers, customers with coupons and customers without coupons. Based on the T-test, the test statistic is contained in the 95% confidence interval, thus we **cannot reject the null hypothesis**. There is no significant evidence that customers with coupons generate more revenue than customers without coupons.

#### 2. Which customers should be targeted
Considering the several models and tests we’ve performed, we think in general, Artea should focus on loyal customers and stimulating those potential customers with non-empty shopping carts to make the purchase. Besides, gender, minority, and
browsing record are also noteworthy attributes that Artea can include in their targeting strategy based on different purposes to maximize the effect of such marketing campaigns.
  
#### 3. Does demographics data influence the recommendation?
<img src="https://user-images.githubusercontent.com/59845928/184966151-c98f1684-1498-44fa-baad-b01471319acc.png" width="600" height="200"><br>
For the Artea case, after the comparison from the **ANOVA test**, we find that combining both gender and minority into our recommendation strategy has **the lowest AIC score**, which means both will influence our expected outcome and we should not ignore either of them.

### 2. [Facebook Analysis](https://github.com/Yichen-Wang-666/R-Programming-Projects/tree/main/Facebook%20Analysis)
#### Purpose of analyzing social media content engagement:<br>
Most common marketing problem for brands can be targeting and attracting the wrong customer. By analyzing the engagement with social media contents, brands can increase the accuracy of conveying the market information and can improve the marketing strategy. And for those people who show interest on social media but are not ready to purchase, by analyzing the hints on social media engagement, companies can also adjust their strategy and solve the pain points.

#### Methodology<br>
1. To find out which predictors are mroe reliable at predicting engagement with digital content, a linear regression model is constructed. Instead of using the total interactions as the target variable, we use the sum of **the number of shares**, **likes** and **comments** because it is more representative. By setting up a threshold of feature importance > 0.01, 13 predictors are filtered as shown below: <br>
<img src="https://user-images.githubusercontent.com/59845928/185002159-8e1bdc55-fe3d-4233-b54f-6c9096970d8d.png" width="400" height="500"><br>
2. To find out whether engagement mostly a function of factors extrinsic to the post (who posted it/ when they did it), or mostly due to intrinsic factors (languages it uses), feature importances are examined. Although the top 3 factors can be grouped into a function of extrinsic factors, the remaining ones are more intrinsic, meaning when people see a post, they will firstly pay attention to who posts it and the time when it post (extrinsic), if the person they are interested or familiar with, then they will take a good look at the details of the post (intrinsic)<br>

We also have analyzed the coefficients of each predictor to understand how they affect the overall interaction. Here we only analyze predictors with high significance. For example, posts with live videos have positive coefficients, indicating more interactions with users. This explains the increasing popularity of live streaming as users feel more involved.<br>
<img src="https://user-images.githubusercontent.com/59845928/185003680-d3308540-4c09-4b88-80c2-0bf428ad4d1b.png" width="400" height="500"><br>

### 3. [Heart Disease Prediction](https://github.com/Yichen-Wang-666/R-Programming-Projects/tree/main/Heart%20Disease%20Prediction)
This project is aiming to predict the occurrence of the heart disease based on different clinical features such as age, sex, blood pressure and so on based on a dataset provided on Kaggle, which includes over 11 common features, making it the largest heart disease dataset available so far for research purposes.

The whole process contains:
#### 1. Data Visualization:<br>
Data exploration is performed, using histograms of ggplot() for numerical and categorical variables.
<img src="https://user-images.githubusercontent.com/59845928/185035578-7c80f7fd-2c57-4499-a639-05222d0fdc22.png" width="400" height="500">
<img src="https://user-images.githubusercontent.com/59845928/185035679-2b900ea2-ab0d-4f3d-a2f1-ac1b427029ea.png" width="400" height="500"><br>

#### 2. Data cleaning and feature selection:<br>
To check relationship between each variable, a collinearity matrix is generated, as shown below:
<img src="https://user-images.githubusercontent.com/59845928/185036953-233a176d-8709-4c69-923b-d4dc49cb3ac5.png" width="500" height="400"><br>
According to the matrix, Sex_F and ExerciseAngina_N will be dropped to avoid collinearity problem.<br>

To select the most representative predictor, feature importance is measured using random forest model, visualized using varImpPlot(), shown below:<br>
<img src="https://user-images.githubusercontent.com/59845928/185038279-558a6a5d-fb0c-4d3e-964b-d0eb80a34f26.png" width="600" height="400"><br>
While a 2-dimensional plot of PCA can also be used to reduce dimensions and select important features. The detailed selection process could be seen in the report. The final choice is [ChestPainType_ASY, FastingBS , ST_Slope_Flat, Oldpeak, Cholesterol, ExerciseAngina_Y].<br>
<img src="https://user-images.githubusercontent.com/59845928/185038961-73796e7a-7682-46ed-ae51-31ce25f0cf98.png" width="600" height="400"><br>

#### 3. Data modelling:<br>
For predicting models, both regular logistic model and boosted forest model are used, with outcome table shown below:<br>
<img src="https://user-images.githubusercontent.com/59845928/185040928-01999946-7764-4c91-9e78-f481a96ba312.png" width="350" height="200">
<img src="https://user-images.githubusercontent.com/59845928/185040943-0a3960f0-557b-4e74-96ae-64a94196c16f.png" width="450" height="200"><br>
The main improvement is due to the boosting, as each tree grows sequentially, and learns from the previous one. This mechanism helps to build a forest of weak predictors. However, this model may tend to be a bit overfitting over this particular dataset. But the good performance provided by both models indicates the reliability of the features chosen previously.

#### Conclusion:<br>
The conclusion could help improve the efficiency of current diagnosis of heart disease, which includes mainly three parts: first category is history check, asking about whether having heart disease history or other symptoms in the past; the second category examines the heart rate abnormality, sound of possible lung crackles, wheezing or third heart sound, while the third category will check the chest radiography.

### 4. [IMDB Review Analysis](https://github.com/Yichen-Wang-666/R-Programming-Projects/tree/main/IMDB%20Review%20Analysis)
The purpose of this project is to develop a predictive model that projects the critic rating (variable name: imdb_score) of the movie based on the IMDb (an online database for all film-related information) dataset. The dataset, with 46 predictors, contains various movie attributes such as the budget of the movie, its duration, and genre, allowing for data analysis and model building. At the completion of the project, the team will use the final model to predict the IMDb rating of 40 blockbusters with the expectation of testing the accuracy and usefulness of the model.

**1. Distribution Visualization:<br>**
<img src="https://user-images.githubusercontent.com/59845928/185045520-54674904-8368-44a2-8be8-0d1395e9a50b.png" width="450" height="500"><br>
When we look at the distribution of total number of actors in a movie, it becomes clear that the data is heavily skewed
to the left and there are many outliers that will have to be eliminated for us to build a good model. This helps us understand the data and identify any possible issues.
  
**2. Non-linearity check:<br>**
After checking all the residual plots, we found that most of our numerical predictors (year_of_release, budget_in_millions, duration_in_hours, and total_number_of_actors) are nonlinear, and this indicates that we should adopt non-linear regression model instead of the simple linear regression to improve reliability.<br>
<img src="https://user-images.githubusercontent.com/59845928/185045638-13a5ccde-a921-4a8b-a05c-f602191e4394.png" width="550" height="400"><br>

**3. Collinearity check:<br>**
When we consider the rule of thumb to handle the collinearity problem, it can be problematic only the absolute value of coefficients exceeds 0.8. As a result, our team concluded that the collinearity problem does not exist in the given dataset, so no further fix is required.<br>
<img src="https://user-images.githubusercontent.com/59845928/185045722-cde4198f-b9d0-4236-b628-aa5a23616d88.png" width="500" height="500"><br>

**4. Feature Selection:<br>**
To identify irrelevant features, we utilized the Recursive Feature Elimination tactic. It works by defining ‘incremental R-squared’ per each predictor by starting with all features in the dataset and removing one predicter from the initial model by one iteration.<br>
<img src="https://user-images.githubusercontent.com/59845928/185046106-2e7ab392-a990-400c-b3a8-224be6692f36.png" width="500" height="300"><br>

**5. Model Selection:<br>**
From the residual plots, we detected **non-linearity of 4 numerical variables** (year_of_release, budget_in_millions, duration_in_hours, and total_number_of_actors) that are all features with predictive powers as suggested by the feature selection section. Therefore, the dataset reveals the need to use polynomial regression to increase the predictive power of the model. The 4 numerical predictors are transferred into non-linear terms.
  
To determine the best degree for each predictor, we decided to apply **ANOVA test**. To ensure the efficiency and accuracy of the ANOVA test, 18 polynomial regression models with various degrees were constructed in order to minimize the effect brought by variable change. We first kept all predictors at degree = 1, and then increment the degree for each numerical predictor. The degrees of other numerical predictors are kept the same and these models were included in the ANOVA function. By checking the decreasing pattern in RSS while keeping our Pr(>F) smaller than 0.05, we could observe the desired degree for our polynomials.<br>
<img src="https://user-images.githubusercontent.com/59845928/185046248-09aaecea-9021-41a7-bc2c-87703656ec3a.png" width="450" height="500"><br>

In the future, if given more time to work on this project, we would recommend looking into interaction terms before predictors to determine whether the factors that make a highly scored movie successful are constant across genres. For example, does increasing duration have the same effect on the critic score for action movies that it does on comedy movies? Increasing the level of granularity using interaction terms is an interesting next step for this project.
  
## Python
## [Python-Optimization](https://github.com/Yichen-Wang-666/Python-Optimization)
### 1. [Police Patrol Route Optimization](https://github.com/Yichen-Wang-666/Python-Optimization/tree/main/Police%20Patrol%20Route%20Optimization)<br>
In this project, we set an eye on Toronto, a city that has demonstrated 78 homicides, 373 shootings, and 5,268 breaks and enters in 2021 till December 2nd (Toronto Crime Incidences, 2021), highlighting the necessity of police patrol for crime prevention and improving citizens’ feeling of safety. Based on a simplified simulation of the Toronto police system and public safety conditions, we built a model to minimize the budget spent on police patrolling among divisions in downtown Toronto via optimizing the patrolling routes and determining the number of police cars.

#### Data Collection:<br>
For our data source, we've assumed a complete police patrol route as a closed loop that can be broken into different line segments connected together by checkpoints. Each checkpoint represents the location of the police headquarters in each division, with Division 53 being the Central Field, shown below:<br>
<img src="https://user-images.githubusercontent.com/59845928/185223594-d5bda931-06f1-4304-9c29-7e420584659e.png" width="800" height="300"><br>

The time required to travel between each police divisions is collected using Google Map, where data is entered into a Route Time Matrix, shown below. We also acquired data on the per-hour utilization cost of a police patrolling vehicle, which we found to be 37.38 CAD/hour for Toronto.<br>
<img src="https://user-images.githubusercontent.com/59845928/185224312-8099b790-06a5-4a86-9acc-d43cf1a37c2d.png" width="800" height="150"><br>

#### Optimization Model (Gurobi Formulation)<br>
- Import Gurobipy, Pandas and relevant libraries
- Load datasets
- Declare model (using Gurobipy.model("Model Name") functionality)
- Create all decision variables (shown below)
<img src="https://user-images.githubusercontent.com/59845928/185224922-0e36324e-5cbd-4079-a660-eeaea2788c83.png" width="600" height="200"><br>
- Add Constraints (8 constraints in total, such as **subtour elimination**, **Arriving/Leaving a division**, details in report in folder)
- Define objective functions (using model.setObjectivN()):<br>
1. **First priority**: Minimize the total travel time, which is the sum of travel time for each police car.
2. **Second priority**: Minimize the maximum travel time, which is the time for all police cars to complete patrol.
3. **Third priority**: Minimize the number of police cars used.

#### Solution<br>
The optimization model will give us the number of cars used for patrolling, their individual routes and the time taken for them to
complete those routes as well as the total cost of travel for the advised routes.<br>
<img src="https://user-images.githubusercontent.com/59845928/185225867-3b29523b-54d6-41a4-b16b-f42dc5ed9d79.png" width="600" height="200"><br>
<img src="https://user-images.githubusercontent.com/59845928/185226069-a065d981-6180-4970-b9b8-1285f416fc0a.png" width="500" height="300"><br>

#### Problem Extension:<br>
If police needs to patrol areas with high crime rate twice, then the model would suggest the following route, with heatmap showing the crime rate.<br>
<img src="https://user-images.githubusercontent.com/59845928/185226483-29b8ecac-b7b2-4752-8165-bf38c1cc0559.png" width="550" height="650"><br>

#### Conclusion:<br>
In this project we have learnt how to solve a real-life problem by using concepts from Travelling Salesman Problem, incorporated with other techniques such as categorizing data by using the heatmap package from python to highlight high crime-rate regions. We have also implemented a multi-objective model, with different weights assigned to each objective function. This technique really helps our model as we need to consider many different goals to help the Toronto police design the best patrol route.

### 2. [Retail Markdown Game](https://github.com/Yichen-Wang-666/Python-Optimization/tree/main/Retail%20Markdown%20Game)<br>
#### Introduction<br>
In the retailer game, each round starts with 2000 items and the sales season is 15 weeks. One needs to choose their strategy during the 15 weeks sale time. One has 4 possible strategy: $60, $54, $48 and $36. Each time after the price decreases, one cannot choose to increase the price. For example, if at week 6 one changes the sale price from $60 to $54, they cannot change back to $60 anymore. The only options left are to maintain the price at $54, or decrease the price further to $48 or $36. 

In this assignment, we aimed to develop a strategy to achieve a good performance in the retail markdown game under different random circumstances.

#### Data Processing<br>
To model this problem using optimization solver, we first utilized the original dataset to generalize the increment in demnad after decreasing the price. Based on the calculation, the average increments in sales when one decrease the price from $60 to several price options ($54,$48,$36) are calculated (1.306, 1.629, 2.647 respectively). These coefficients will be used for forecasting the increment in sales. <br>
<img src="https://user-images.githubusercontent.com/59845928/185230334-1dc983ca-914d-4ae5-bc44-1ffc153f2cc9.png" width="700" height="300"><br>

#### Optimization Model (Gurobi Formulation)<br>
For variables, we have D_60 representing the weekly demand at $60, where demand at different prices can be represented with coefficients * D_60. (E.g. D_54 = 1.306*D_60). Other variables are x_60, x_54, x_48 and x_36 representing the number of weeks the item is sold at a specific price (x_60 refers to the number of weeks the item is sold at $60 and the rest are defined similarly). The lower bound is set to be 0 and the upper bound is set to 60 as it is the length of the trial.
  
The **objective function** is shown below:<br>
<img src="https://user-images.githubusercontent.com/59845928/185236362-f2f1944f-3012-4c2b-86eb-2fb06f035a25.png" width="650" height="50"><br>  

The Final result is shown below, indicating that at a demand of 105 at price = $60, price level at $60 should be maintained for two weeks and the remaining weeks should be maintained at the price of $54.<br>
<img src="https://user-images.githubusercontent.com/59845928/185236877-88a55b1d-605b-400d-b037-31a69f22cad9.png" width="350" height="200"><br>  

### 3. [SVDC algae harvesting](https://github.com/Yichen-Wang-666/Python-Optimization/tree/main/SVDC%20algae%20harvesting%20optimization)<br>
#### project description
SVDC R&D department has a major pain point that at what level of cell density, what frequency, as well as harvest amount would result in the maximum yield. This project uses various optimization and visualization methods to deliver the optimum harvesting scheme. 

#### Use Case Pain Points (pp):
1. SVDC only has un-cleaned data recorded by sensors, which cannot be transferred into usable information.
2. Three factors during the harvesting process (density level at harvesting, volume extracted for each harvest, and time interval between each harvest) require optimization to reach theoretically highest possible yield.

#### Solution:
**Solution for pp1**: Data preprocessing and winsorization are performed to detect and eliminate outliers in original dataset. Only data without external interference are kept for further modelling.

**Solution for pp2**: Growth versus Density plot is obtained from daily record of density. This relationship simulates a piecewise function between density and time, leading to a Monte Carlo optimization of the harvesting procedure. The best combination of harvesting conditions (density level at harvesting, volume extracted for each harvest, and time interval between each harvest) are obtained from a 3d heatmap.

#### General Architecture:<br>
<img src="https://user-images.githubusercontent.com/59845928/185246043-63a57f82-4b62-48c1-8f5f-c1963bff6c84.png" width="800" height="400"><br>  

#### Data Processing:<br>
Data processing includes several procedures, such as:
#### 1. data cleaning and plotting
Most of the data will be removed as it is irrelavant to the analysis, all the null records have been dropped<br>
<img src="https://user-images.githubusercontent.com/59845928/185247326-ea4e1c28-eb5f-475c-93ba-2222c8dfb9a4.png" width="800" height="170"><br>  

#### 2. data selection
![image](https://user-images.githubusercontent.com/59845928/185247686-e55936f6-7534-4f6c-86ec-174a8bd3430d.png)

#### 3. growth rate calculation
![image](https://user-images.githubusercontent.com/59845928/185247815-ccdbb00f-f19f-4c82-bb40-e705fd3cac31.png)

#### 4. Simplification of the growth rate plot
![image](https://user-images.githubusercontent.com/59845928/185247911-38cb81a7-aa56-4007-aa22-b7c2411a7fcb.png)

#### 5. Final Function simulation
![image](https://user-images.githubusercontent.com/59845928/185247947-ec7596a0-529e-4a77-90f7-67f0b624a4f2.png)

#### Optimization model<br>
![image](https://user-images.githubusercontent.com/59845928/185248443-47840c47-88b2-4bc5-b0db-63c4305521ab.png)<br>
![image](https://user-images.githubusercontent.com/59845928/185248475-35e31646-1e76-493f-94bc-f70f26a2fd44.png)
![image](https://user-images.githubusercontent.com/59845928/185248550-1ab3978d-b89c-4811-b032-b691c41673e6.png)


## [Python-Machine Learning](https://github.com/Yichen-Wang-666/Python-Machine-Learning)
1. [NLP](#nlp)
2. [Python ML](#python_ml)
3. [Neural Network](#neural_network)

### NLP
### 1. [Airline Customer Experience Analysis](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/Airline%20Customer%20Experience%20Analysis)<br>
In this project, in order to compare airlines in terms of customer experience, we collect and analyze related **user-generated content** (UGCs) rather than trusting polished news articles or advertisements produced by airlines themselves. More specifically, we aim to 
1. Analyze popular airlines and understand whether people show positive or negative sentiments about each one of them 
2. providing customized recommendations of airlines to segmented customers based on their preferences by leveraging sentiment analysis and airlines segmentation
3. providing advice to airlines about which attributes to improve to effectively alleviate customer experience.

#### Revew Scraping:
All the data is scrapted from two famous airline review websites, namely Consumer Affairs and Skytrax. By scraping reviews from different sources, we reduce the bias on a specific platform and we are able to get the true consumer point of views and generalize our analysis. We focus our analysis on 10 different well-known airlines in the world, shown below:<br>
![image](https://user-images.githubusercontent.com/59845928/185257099-68b83d0f-2b3c-4542-9188-9b41b760ecaf.png)

#### Pre-processing and word analysis:
To pre-process the scraped reviews, we did the following two steps:
1. Tokenizing the reviews by the **nltk** package
2. Replace confusing tokenized words such as "American","Airlines" into "American_Airlines".<br>
3. Filter out most frequently mentioned nouns, adjectives and adverbs across all reviews.<br>
And a word cloud and counting histogram have been generated:<br>
![image](https://user-images.githubusercontent.com/59845928/185257788-67ed0067-9a5a-4541-9328-7e6753e8a003.png)
![image](https://user-images.githubusercontent.com/59845928/185257794-2a9b940e-9e4a-4663-ba1e-a314af30727d.png)

Words have been manually grouped into seven major attribute categories, shown below:
<img src="https://user-images.githubusercontent.com/59845928/185262530-c613b2da-aae6-44c7-9c53-1af7407f509c.png" width="650" height="400"><br> 
All the word counts have been summarized by a histogram, describing the distribution of all 7 attribute categories.<br>
![image](https://user-images.githubusercontent.com/59845928/185262723-2abd5f98-5760-4ca8-a071-543926887842.png)

#### Sentiment Analysis
With the help of vader package that examines both polarity and inensity of emotions reflected by sentences, sentiment scores are generated and a coupound score is calculated. The dataset is transformed into an interactive dashboard shown below:<br>
![image](https://user-images.githubusercontent.com/59845928/185262872-5030e7bd-2df6-4f3a-b3bc-78af77e38db4.png)
#### Regression
By performing regression, we could predict the sentiment score for a particular airline, and investigate the relationship between the sentiment score and its various component. For example, American Airline has a coefficient of -0.1746, meaning reviews mentioning American Airline usually tend to be negative. The detailed results shown below:<br>
![image](https://user-images.githubusercontent.com/59845928/185263229-885e4d8d-db53-46c0-9aa0-27535fe02480.png)

### 2. [Ice Bucket Challenge Analysis on Twitter](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/Ice%20Bucket%20Challenge%20Analysis%20on%20Twitter)<br>
In this project, we will explore what role the social media (Twitter) played during the famous Ice Bucket Challenge campaign in 2014 and how it influenced the trend of this charity movement from two perspectives: 
1. We will apply methods such as topic modelling and sentiment analysis to investigate the thoughts and attitudes of Twitter users had towards this campaign. By integrating scores generated with time labels, we could come up with detailed trend plots to gain a deeper understanding. 
2. Network analysis will be used to examine how the ALS association and other influencers/ celebrities contributed to this campaign.
#### Data Acquisition
Data scraping is performed over Twitter, both on related tweets and user info of all mentioned users using Twitter Developer API.
#### Constraints:
1. All tweets mention **#IceBucketChallenge** are collected, where data ranges from July 2014 to December 2014 since this campaign
achieved its popularity peak during this period according to the tweet summary statistics.
2. To reduce the data scraping time cost, we only chose the 1st, 15th and 30th of each month to represent important milestones to reduce dataset size.
3. There’s a limit of 5000 tweets per day due to the possibility of having an enormous amount of related tweets posted on that day

#### Topic & Sentiment Analysis
To reveal the popularity change of the campaign on Twitter over time, we first extract the dates of each tweet we collected and then plot the number of postings to visualize the trend<br>. We see that #icebucketchallenge has comparatively high popularity, with #icebucketchallenge embodying a similar trend as the tweets posts’ trend obtained from the previous step. The popularity of #als also increases at the beginning of our observed period but dropped significantly after a month.
![image](https://user-images.githubusercontent.com/59845928/185265752-c11f1bfd-25fc-429f-9120-d338ea986051.png)
With the vader package, we calculate the compound sentiment scores for each of the tweets. We classified each tweet’s sentiment into these three categories: positive, neutral and negative. Then, we plot out a line graph denoting the change of sentiment over time.
![image](https://user-images.githubusercontent.com/59845928/185265999-c10f3360-a3f3-48ec-a4cb-28163c4c87b5.png)

#### Topic Modelling
To further extract the hidden structure behind this collection of tweets, we used the Latent Dirichlet Allocation model (referred to as LDA). Given the number of documents and number of words, we determined the number of topics and ran the model. The output includes both the distribution of words for each topic and the distribution of topics for each document. In our case, each document refers to a tweet post. Utilizing Python packages such as **gensim, nltk, pprint, pyLDAvis and pickle**, as well as a for loop on the number of topics, we were able to find the optimal number of topics and generate a dashboard for our topic modelling result, shown as below:
![image](https://user-images.githubusercontent.com/59845928/185268717-68361306-4bdf-4d90-90bb-67b6d9124d99.png)
For Sub-topic analysis, the number of users mentioned of tweets under different topics is shown as well:<br>
![image](https://user-images.githubusercontent.com/59845928/185269921-36540332-7400-4acb-9374-6211fe7d16c5.png)

#### Network Analysis
To better understand the results, we created a visualization for networks of the top 10 influencers that we identified in the ice bucket challenge, using the Pyvis library. According to the network visualization shown below, the big circular cluster is the network of youtube. As a popular media platform, YouTube was mentioned the most when users posted tweets regarding the ice bucket challenge, and thus had the largest network. This is reasonable because many people are either watching or posting ice bucket challenge videos on YouTube.
<img src="https://user-images.githubusercontent.com/59845928/185270110-5d9834da-bc4b-4906-9f3a-597b7eb353b3.png" width="650" height="500"><br> 

#### Recommendation:
![image](https://user-images.githubusercontent.com/59845928/185270188-39b9942b-85eb-4857-8d7b-aba0d2ca79f7.png)

### 3. [Name Origin Classification using Character-level RNN](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/Name%20Origin%20Classification%20using%20Character-level%20RNN)<br>
An rnn-based model is developed to perform classification. The goal is threefold:

1. Preprocessing procedures required for performing text classification from A to Z.
2. Use embeddings and RNNs in conjunction at the character level to perform classification.
3. Write a function that takes as input a string, and outputs the name of the predicted class.

#### Dataset
Dataset includes 2.88 million names corresponding to their origin, shown below:
![image](https://user-images.githubusercontent.com/59845928/185271027-83383886-8924-4936-8fab-6681be32f85b.png)
#### Modelling:
1. Map the corresponding origins into one-hot vectors, so could be fitted for classification.
2. Use the Keras tokenizer at the character level tokenize the name input into integar sequences.
![image](https://user-images.githubusercontent.com/59845928/185273583-bf17f729-7ed3-4adc-b25b-0a45407e759f.png)
3. Pad the sequences using the Keras preprocessing tools.
4. Train the Sequential RNN model
![image](https://user-images.githubusercontent.com/59845928/185273632-9da551b3-f4d4-4352-b425-3a8e3bfcd07b.png)
5. The most probable origin will be returned, example shown below:<br>
![image](https://user-images.githubusercontent.com/59845928/185273745-97d50e91-1060-4220-bd20-abfabca14c6a.png)

### Python ML
### 1. [KickStarter Data Analysis](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/KickStarter%20Data%20Analysis%20(Classification%20%26%20Clustering%20Model))<br>
The goals of this project are:
1. Developed a classification model that predicts whether the variable “state” will take the value “successful” or “failure.” 
2. Develop a clustering model to group projects together.

#### Data Description
The dataset in this project is scraped from Kickstarter, which is a popular crowdfunding platform. There are 45 variables in total. Variables include **Number of backers**, **Status of the Project** and so on.<br>

#### Classification model
A classification model is built to predict whether the variable "State" will take the value "successful" or "failure".
1. **Clean the data**: drop null values and columns with unique values (such as id, which cannot contribute to classification). Other columns with high collinearity will be dropped as well.
2. **Feature Selection**: for feature selection, **RandomForestClassifier** is used to fit the current data and indicates feature importance. Top 5 features are selected to be predictors.

According to the feature importance provided by the RandomForestClassifier, the goal amount set is the most important factor to the success of the project. It could be deduced that an unreasonable goal may scare away backers, while a good and realistic goal may give backers confidence. Other factors such as “name_len_clean” and ”create_to_launch_days” also contribute a lot, meaning that a clear and intuitive name and a suitable preparation period for the project launch will likely indicates success.

#### Clustering model
A clustering model is used to group projects together. Before clustering, all features are standardized. The clustering method I used is **KMeans** so a pre-determined number of clusters is required. This could be determined by using the **elbow method**. Since adding another cluster almost always reduce the variance, a number k that improves little should be our target k. In this case, k=5 is a good choice. To test whether the cluster assignment’s performance, the **silhouette method** is used, and the silhouette score is equal to 0.856, much greater than 0.5, meaning it provides good evidence of the reality of the clusters in the data. Results shown below<br>
  
![image](https://user-images.githubusercontent.com/59845928/185299229-3f09cd0b-f0e3-4480-814b-a06dd3461778.png)
We can obtain a lot of insight from these results, especially about how the several features affect the rate of success. Since the data has been normalized, value equals to 0 meaning is among average. For example:<br>
- For cluster 1, it has an astonishing high value for staff_pick, meaning if the project has been promoted and highlighted on the site, there will be a great chance of achieving success.

### 2. [Salary Prediction from Job Description](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/Salary%20Prediction%20from%20Job%20Description)<br>
This assignment involves building and testing classification models to predict salaries from the text contained in the job descriptions. The data for this assignment can be found at http://www.kaggle.com/c/job-salary-prediction.

2500 data points were randomly selected from the training dataset (“Train_rev1.csv”) for ease of analysis. Naïve Bayes classifier models were created to predict high (75th percentile and above) or low (below 75th percentile) salary from the text contained in the job descriptions.

#### Model Construction
1. For the **Salary** column, the value is normalized to improve training results. And the "high" and "low" standard can be calculated using 75th percentile. 
2. A new binary attribute is added, 0 meaning lower than the standard, and 1 meaning higher than the standard.
![image](https://user-images.githubusercontent.com/59845928/185302667-b1116a61-987d-480a-9f91-644d2cd4e83b.png)
3. Setting up stopwords to choose only nouns and adjectives from tokenized words.
4. Features are selected from top 2000 most frequent words appeared in the description
5. The **Naive Bayes Classifier is used to train the model**


#### Results
The confusion matrix is shown below, showing the accuracy of the model (0.784) and a high recall value.<br>
![image](https://user-images.githubusercontent.com/59845928/185303666-6a511a28-58d8-4ea3-950d-a17eb6cb2cc1.png)<br>
The top ten words that are most indicative of high/low salary are shown below as well:<br>
![image](https://user-images.githubusercontent.com/59845928/185304074-734e6db7-e70a-4274-a299-53e9f1a0c17e.png)
![image](https://user-images.githubusercontent.com/59845928/185304090-c30b9da8-fc32-4771-9534-a045ab84821e.png)

### 3. [Spotify Analysis](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/Spotify%20Analysis)<br>
Improve functionality of Spotify by adding "Mystery Box", which allow users to choose the number of songs desired, genre & mood, and mood level. A playlist will generated according to the parameters entered.
  
#### Dataset
This project is conducted using Spotify dataset on Kaggle. We also build a front-end web app of our project, to use it, please refer to this URL (https://8potify.netlify.app/). Variables include numerical ones such as **Acousticness (ranges from 0 to 1)**, **tempo (ranges from 50 to 200)**, and so on. Categorical variables include **key**, **artists**, and so on.

#### Clustering model
Each song has been clustered into one cluster and given a gnere, the graph is shown below:<br>
![image](https://user-images.githubusercontent.com/59845928/185318927-9ac615d4-f2a8-42b1-9a23-f7b42d40eba5.png)

The clustering using **K Nearest Neighborhood (KNN)**, which is a non-parametric learning method. KNN will calculate the distance between the target song and every other song in its database.

#### New Features
3 new features are added, which mainly result in certain filters available.<br>
1. **By Song**: Users can enter a song title, the artists of the song, and the number of recommended songs they want. The algorithm will generate a list of recommended songs based on the inputed song.
2. **By mood**: we create a list of moods based on the music features. For example, enegy will be energetic and danceability will be willing to dance. Users can enter the mood, select the percentage of mood and number of recommenations. A sample entry will be: want to dance, 70%, 5 songs. The algorithm will then generate 5 songs based on the song that is the nearest to the 70% quantile of danceability attribute.

#### Demo
A front-end web app is built to simulate the result of the project (https://8potify.netlify.app/), shown below:
![image](https://user-images.githubusercontent.com/59845928/185322927-b8c651e0-f9a2-4a35-b003-f01d754770f1.png)

### Neural_Network
### 1. [CIFAR100 Dataset Classification using AlexNet](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/CIFAR100%20Dataset%20Classification%20using%20AlexNet)<br>
An AlexNet Architecture is built and trained on the CIFAR100 dataset. Kernel sizes are resized and the number of kernels are changed because CIFAR100 is a smaller dataset than ImageNet, as well as lower-resolution (32x32 vs 224x224).

#### 1. Preprocessing
The primary preprocessing transformations that will be imposed on the data presented to the network are: Normalizing and standardizing the images. Resizing of the images from 32x32 to 227x227. The AlexNet network input expects a 227x227 image.<br>
#### 2. Pipeline
Implement mapping, shuffle and batching at size of 32.
#### 3. Model Implementation
![image](https://user-images.githubusercontent.com/59845928/185326534-f5d3864b-8b32-4868-8106-8b393c0eb30e.png)<br>

For evaluation, the result is shown below:
![image](https://user-images.githubusercontent.com/59845928/185327040-f6d3ac75-7821-4831-bd14-b53c01632999.png)

### 2. [MNIST Autoencoder](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/MNIST%20Autoencoder)<br>
Autoencoders using the funcitonal API are create with the following topology:<br>
1. Stacked 784 - 392 - 196 - 392 - 784 (tied weights or not)
2. Convolutional Encoder (conv, maxpool, conv, maxpool, conv, maxpool). Decoder (conv, upsample2d, conv, upsample2d, conv, upsample2d, conv)
![image](https://user-images.githubusercontent.com/59845928/185329195-c1abbe45-ada6-401d-8d91-db50195a3d94.png)

The result is shown below:
![image](https://user-images.githubusercontent.com/59845928/185329430-efda0c9b-170e-4df6-86ef-a73a775aea73.png)

### 3. [Reinforcement Learning (CartPole-v0)](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/Reinforcement%20Learning%20(CartPole-v0))<br>
1. Setting up initialization (Learning-rate, discount, runs)
2. Exploration settings (epsilon, decay value)
3. Create bins and Q tables to store every state

If pole fell, given negative rewards; The formula to calculate Q values:<br>
![image](https://user-images.githubusercontent.com/59845928/185332458-d0e0d2aa-86ba-4905-a483-bd24c8b14330.png)

The plot for the learning process is shown below, with three different reward type:<br>
![image](https://user-images.githubusercontent.com/59845928/185332931-92e9540b-70fa-4a0d-a109-bfa49d02b200.png)
  
### 4. [Time Series Prediction](https://github.com/Yichen-Wang-666/Python-Machine-Learning/tree/main/Time%20Series%20Prediction%20using%20Tensorflow)<br>
## Code Description
Time series prediction using datasets from:
https://storage.googleapis.com/nicksdemobucket/sunspots.csv

Three different machine learning models are used: RNN seq-to-seq, LSTM and GRU. Results are shown below:
#### RNN SEQ-TO-SEQ:
![image](https://user-images.githubusercontent.com/59845928/184555841-f8013ff9-611e-4d0e-9ff7-006b248af370.png)
#### LSTM:
![image](https://user-images.githubusercontent.com/59845928/184555849-3a2eaa60-4747-441c-981f-3094aa49f5e7.png)
#### GRU:
![image](https://user-images.githubusercontent.com/59845928/184555858-9a68c986-b7fe-476a-8872-3852a587016f.png)


### Excel

