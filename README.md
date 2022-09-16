# Interested in Knowing What Factors are Causing Traffic Crashes on the Roads of Chicago?

## Background
The Chicago Police Department (CPD) records every traffic crash taking place on its roads in an electronic crash reporting system (E-Crash). Records are added to the data portal when a crash report is finalized or when amendments are made to an existing report in E-Crash.
We are working with two datasets here which are sourced from CPD’s official website:
### Dataset 1: Traffic Crashes Data (https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if)
The traffic crash data contains all information about the crash, number of injuries in the crash, weather conditions at the time of crash, etc. Note: Our focus in the dataset is towards analysis crashes which result to injuries, hence we are excluding unfatal crashes out of our analysis.

### Dataset 2: Traffic Crashes People (https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d)
The dataset records details of the people who were involved in the above traffic crashes we have earlier analysed. The datasets are threaded together through 'Crash_Record_Id' variable which is a unique identifier for each crash incident. Through this dataset we have some attributes about the people, their demographics, license status and all

## Objective of the Study
We are analysing the traffic crashes data at first to understand what variables are playing role in traffic crashes happening in the City of Chicago. Our focus of research is accidents leading to fatal injuries (at least 1) which will enable us to prioritize those crashes first. The analysis would open our view towards what could be possible reasons behind common crashes leading to injuries.

## Methodology Adopted
-In order to have a general view of the situation, we have sampled 10,000 crashes from the whole data to perform our analysis. This helps us in two ways: 1) Optimizing and making the analysis efficient 2) Randomised distribution of events 
-Moreover, to make the analysis more meaningful, we picked up data which leads to at least 1 injury in the crash. 


## Observations
Roads with no controls devices are more prone to fatal accidents
Rear end collisions are most frequent occuring type of crash.  West and South bound directions have the most crashes amongs all the categories.
Analysing the reason for the crash, we found a lot of data is tagged as 'Unable to Determine' as a primary cause of the crash. While, apart from that we see that 'Failing to Yield Right of the Way' is the most common cause of the crash and comprising close to 20% of the all the crashes under study.




