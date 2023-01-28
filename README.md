# ML_Regression_Retails_Sales_Prediction

The main objective of this project was to build a predictive model to forecast the daily sales for 1115 Rossmann stores in Germany using historical sales data for 6 weeks in advance. The data provided consisted of 2 datasets, one with store information, sales, customers, and other details, and the other with store type, competition distance, and promotion information. 
# **Evaluation Criteria:**
The evaluation criteria was based on the Root Mean Square Percentage Error (RMSPE). Lower the score better will be the prediction

# **Problem Statement**:
The main objective is to build a predictive Model,the task was to forecast the daily sales for Rossmann stores in Europe using historical sales data for 1,115 stores.

# **Approach:**
After loading the dataset and importing the libraries, first step was to clean the data and Replacing the Null values with it's suitable Mean,Meadian or Mode.
Then we Merged the two dataset & We extract the Month,Year,WeekofYear from Date columns and also Understand each and every Variables After cleaning the data, EDA was performed In EDA We done Univariant ,Bivariant and Multivariant Comparision.We used many graphs like bar chart,pie chart,line chart,facegrid etc to show diffrent kind of relationship between variables.
It included statistical analyzes in which specific trends,relationships and factors have been identified that had some impact on our dependent variable.We have done Year of Year ,Month of Month and Day of Day comparision & plot correlation matrics to see the relationship of every columns.
the next step was feature engineering where competition and promotion columns were combined and unnecessary columns were dropped,
Then we had worked on OneHotEncoding and encoded 'DayOfWeek','StoreType'&'Assortment' columns . The next step was to check for distribution and outliers and replace them with suitable values by doing Capping we used methods like z-score for Sales

The final step was to experiment with various machine learning algorithms in the separate and suspended data. Following algorithms have been used viz. Linear regression,Decision Tree, Random Forest Regressor & hyperparameter tuning was performed and evaluated the performance of each model using
a variety of metrics. And also implemented feature importance technique to understand which features were important for the prediction purpose.
Linear Regression Model RMSPE and R2 score for train test:
**Linear Regression**
RMSPE Train:0.05688450820238183

RMSPE Test: 0.055890281246762465

R2 Train: 0.751786052900501

R2 Test: 0.7464744699494363

Linear Regression didn't gave such good score so we tried Random Forest,

Random Forest: **bold text**

RMSPE Train: 0.0068497492138425665

RMPSE Test: 0.021876457462720905

R2 Train: 0.996400953086413

R2 Test: 0.9611578642172859

if R-squared score was the best for random forest, it means that the random forest model fits the data well and it explains a large portion of the variability in the target variable.

then for betterment we tried Decision Train and Also got the best score but less accurate then RF

**Decision Tree:**

RMSPE Train: 0.00013284138986048634

RMPSE Test: 0.031322119805353356

R2 Train: 0.9999986463543659

R2 Test: 0.9203746412500768

To compare the Accuracy among different regression models, RMSE is a better option as it is simple to calculate and differentiable.So, after comparing RMSE and RMSPE values it is evident that Random Forest Regressor is the best performer. 
