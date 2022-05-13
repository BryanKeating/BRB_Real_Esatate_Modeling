# BRB Reality Modeling
## Overview
For this project, you will use multiple linear regression modeling to analyze house sales in a northwestern county.
    

    
## Business Understanding
At BRB reality, our job is to find solutions to your Real Estate Goals.  We created mamathematical models which predict Real Estate data, allowing us to give you calculated recommendations with calculated risk. 


## Data Understanding and Analysis
For this project, we utilized the following sources of data:
    
    1. KCSO Offense Reports 2020-Present 
    This data set gave us criminal offenses based on each Zip Code. We created a rating sytem and rated them from 0-5 based on the number of crimes             in each Zip Code. The higher our saftey rating-the lower the crime.  (55,000 Crimes)
    2. KC_Hosusing_Data
    This data set gave us various factors in predicting the price of a house. From this data, we used price, square foot living, number of bedrooms,  and the age of each house. We nemoved the outlier house that contained 33 bedroom inorder to better visualize our data. (21,500 homes)
    3. WA State School District Rankings 2020
    This data set gives us School District Ranking tied to each house's zip code. We used this data set to group each house into School Districts by           zip code and then compared our results to the school districts rating. (250 School Rankings)

Final Data Set-20,632

## Modeling
1. Linear Regression Model - Our data showed that Sqft Living was the most important feature. 

![regression_plots](https://user-images.githubusercontent.com/103067635/168381942-1e6b0982-3c15-4583-b2c0-bcba6fbac29b.png)


2. School District Rating vs. Price - This showed us that a school district rating with 4 or 5 stars commanded a higher home price. 

![SCHOOL_DISTRICTS](https://user-images.githubusercontent.com/103067635/168381493-28ce54e6-22de-4e75-96c4-e8a7391ed1f3.png)


3. Saftey Rating vs. Price - Neighborhood Crime Rate does now show any impact but please see limitations for more info. 

![safety_rating_plot](https://user-images.githubusercontent.com/103067635/168381424-0ea11683-f762-44e1-9181-5c82ca008868.png)

4. Age of Home vs. Price - Individually Age of Home didn't show an impact when compared to Price but it added to our overall model. 

![home_age_v_price](https://user-images.githubusercontent.com/103067635/168381400-4b86b7c0-907d-47a9-b3f7-99999a063483.png)




Limitations:Saftey Rating. We would like more data that tell us what type of crime happend.
No linear Data
## Regression Results

![final_model](https://user-images.githubusercontent.com/103067635/168381153-defec933-0e10-4cfa-af93-f3021d46dcf0.png)



## Recomendations
We concluded that in addition to Sqaure foot living, the most important features to include are School Rating, Saftey Rating, and Home age. We bleive that with further exploration, we recomneded that focusing on the data points under out profit line, especially those with high saftey rating, high school ratings, and high grade scores. Further, with continued exploration, we recommend focusing on the data points under our profit line - especially those with High Safety Rating, High School Rating, and High Grade scores.


## Limitations and Next Steps

**Limitations
    We weren’t able to tie in pop data to crime, so highly populated areas are going to seem more dangerous, and we did not distinguish between types of crime (petty theft v assault for example)
    Our data was outdated (2014-2015) and does not properly accoutn for currrent market trends
    To make this model more accurate, we would need at least 5-10 years worth of data
**Normality
    Does a good job at explaining price within 2 std of the mean, so homes priced between 655. You can see as the price increases, so does variance
**Next Steps
    Compare linear Data
    Further Investigate Safety Data
    Consider the cost of construction/ renovation vs. current value
    Explore Date of construction with cost of construction vs. current value
