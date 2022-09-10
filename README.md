# Chicago-Traffic-Crashes-Analysis

Crash data shows information about each traffic crash on city streets within the City of Chicago limits and under the jurisdiction of Chicago Police Department (CPD). Data are shown as is from the electronic crash reporting system (E-Crash) at CPD, excluding any personally identifiable information. Records are added to the data portal when a crash report is finalized or when amendments are made to an existing report in E-Crash.

# Methodology Adopted:
-In order to have a general view of the situation, we have sampled 10,000 crashes from the whole data to perform our analysis. This helps us in two ways: 1) Optimizing and making the analysis efficient 2) Randomised distribution of events 
-Moreover to make the analysis more meaningful, we picked up data which leads to atleast 1 injury in the crash. 

# Background of the Data:

## Dataset 1: Traffic Crashes Data
We are analyzing the traffic crashes data at first to understand what variables are playing role in traffic crashes happening in the City of Chicago.
 The analysis opens our view towards what could be possible reasons behind common crashes leading to injuries.
Our focus in the dataset is towards analysis crashes which result to injuries, hence we are excluding unfatal crashes out of our analysis.

Observations:
Roads with no controls devices are more prone to fatal accidents
Rear end collisions are most frequent occuring type of crash.  West and South bound directions have the most crashes amongs all the categories.
Analysing the reason for the crash, we found a lot of data is tagged as 'Unable to Determine' as a primary cause of the crash. While, apart from that we see that 'Failing to Yield Right of the Way' is the most common cause of the crash and comprising close to 20% of the all the crashes under study.

## Dataset 2: Traffic Crashes People
The dataset records details of the people who were involved in the above traffic crashes we have earlier analysed. The dataset are threaded together through 'Crash_Record_Id' variable which is a unique identifier for each crash incident.
Through this dataset we have some attributes about the people, their demographics, license status and all

# DataSource:
https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if
https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d

