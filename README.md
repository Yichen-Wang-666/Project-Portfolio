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
<img src="https://user-images.githubusercontent.com/59845928/184714277-c0a2284a-3a3a-450d-b4e7-f65e8af64c5e.png" width="500" height="350">

For more details, please visit Bumble Database Simulation Folder to see the report and files.

### 2. [La Ronde Analysis](https://github.com/Yichen-Wang-666/MySQL-dbms/tree/main/La%20Ronde%20Analysis)
Several datasets including the ride history, ticket, customer, facility and so on of La Ronde, one of the famous amusement part in Montreal, are provided. This project aims to create a database to store all the datasets and come up with different queries to exploit values from the massive amount of data.

**The ERD of the database is shown below**<br>
<img src= "https://user-images.githubusercontent.com/59845928/184717931-d8995621-ceb5-4afb-80c3-176d38759965.png" width="700" height="500">

_Example Query:_<br>
<img src= "https://user-images.githubusercontent.com/59845928/184719095-910394fc-acdd-4b9d-8dbf-504fa56f0b6d.png" width="600" height="400"><br>
<img src= "https://user-images.githubusercontent.com/59845928/184719249-1a448936-7b65-4bd4-9ec5-85486421bf6f.png" width="600" height="360"><br>

### [R Programming](https://github.com/Yichen-Wang-666/R-Programming-Projects)
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
For the Artea case, after the comparison from the** ANOVA test**, we find that combining both gender and minority into our recommendation strategy has **the lowest AIC score**, which means both will influence our expected outcome and we should not ignore either of them.

### 2. [Facebook Analysis](https://github.com/Yichen-Wang-666/R-Programming-Projects/tree/main/Facebook%20Analysis)



### Python
### Excel
