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

### Excel
