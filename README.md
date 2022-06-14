# kickstarter-analysis
## Performing analysis on Kickstarater data to uncover trends
####  An Analysis of the Kickstarter Campaign through multiple media. 

Example: Seasonality and influence of campaign funding in Theater
![image](https://user-images.githubusercontent.com/95913722/173016794-8bbae271-0d5a-4374-a95d-15e979771179.png)

Examples of past success and failures in multiple industries:
![image](https://user-images.githubusercontent.com/95913722/173017514-8a7de6a7-f42b-4e99-80bc-4386d474ca59.png)

A large factor influencing success or failure based on statistical data on campaign goals and pledges.

![image](https://user-images.githubusercontent.com/95913722/173018337-e2e54a82-f8e2-4e60-87e1-357fcceb9d92.png)

# Kickstarter Challenge – Written Analysis of Results

## Overview of Project

### Purpose: 
The purpose of this project is to help Louise compare her play’s fundraising goal’s performance to other project performances based on their plays’ launch date and financial goals.  Louise’s play “Fever” was created in 2016 but she barely met her project goal. The review and analysis of the data set of over 4000 plays in different categories gives an insight on this analysis. The three-year historical analysis helped us to compare performance from industries and helped to narrow down to a specific industry.


## Analysis and Challenges: 
Based on the data set provided, we converted the UNIX timestamp provided in the data set into a more readable format using the formula =(((J4110/60)/60)/24) +DATE (1970,1,1). Once a more recognizable date format was obtained, we used the excel formula “=Year ()” to extract the year. We also used the Pivot table to extract the number of plays categorized under the year and month they were produced. Between 2014 and 2016 there were a total of 1,369 project lunch in the Theater category. 

### Analysis of Outcomes Based on Launch Date: 
From running the pivot and analysis, we identified 
a pattern for success, failures, cancellation. The most successful projects launched in the month of May and began to decline in June, while from October through December there was a steep decline in projects’ success rate. October also recorded the highest number of failures throughout the year. 


### Analysis of Outcomes Based on Goals: 
The data set fund was grouped into twelve goal ranges and four categories - successful, failed, live, and cancelled.  Using the “COUNTIFS” function, (COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,"<1000",Kickstarter!$R:$R,"plays") we categorized project outcome goals under these categories. The most successful project had goals between $1,000 to $4,999 while plays with goals between $45,000 and $49,999 recorded the highest failure.  Also, the SUM(B2:D2) function helped to derive the project totals under each group and the percentage of totals.

### Challenges and Difficulties Encountered: 
The most challenging part of the analysis was correctly using the correct “COUNTIFS” criteria. The correct result from one cell was copied to the other cells and modified according to their various categories. There was no difficulty in performing this task.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?: The two conclusions I can draw about the Outcomes based on Launch Date are:
i.	The most successful projects launched in the month of May and began to decline in June. So, this will be the best time to launch a new play base on the 3year historical data.
ii.	December and January are not active periods under the Theater category and plays are likely to not be as successful as those in May or June. 

- What can you conclude about the Outcomes based on Goals?: i.	The most successful project had goals between $1,000 to $4,999 while plays with goals between $45,000 and $49,999 recorded the highest failure. So, you do need to raise so much funding to run a successful play in a theater.

- What are some limitations of this dataset?: The data set is a sample size from across the world and may not be a true representation of the entire population. Also, there are several outliers in the data set that may have skewed the statistic far to the left.

- What are some other possible tables and/or graphs that we could create? Other possible tables and/or graphs that we could create include an Area chart that shows the concentration of successes, etc. a Bar Chat or a histogram that could easily represent the skewness of the population mean. 
