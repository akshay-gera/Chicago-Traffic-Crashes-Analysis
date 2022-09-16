# Interested in Knowing What Factors are Causing Traffic Crashes on the Roads of Chicago?

## Background
The Chicago Police Department (CPD) records every traffic crash taking place on its roads in an electronic crash reporting system (E-Crash). Records are added to the data portal when a crash report is finalized or when amendments are made to an existing report in E-Crash.
We are working with two datasets here which are sourced from CPD’s official website:
### Dataset 1: Traffic Crashes Data
(https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if)

The traffic crash data contains all information about the crash, number of injuries in the crash, weather conditions at the time of crash, etc. Note: Our focus in the dataset is towards analysis crashes which result to injuries, hence we are excluding unfatal crashes out of our analysis.

### Dataset 2: Traffic Crashes People 
(https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d)

The dataset records details of the people who were involved in the above traffic crashes we have earlier analysed. The datasets are threaded together through 'Crash_Record_Id' variable which is a unique identifier for each crash incident. Through this dataset we have some attributes about the people, their demographics, license status and all

## Objective of the Study
We are analysing the traffic crashes data at first to understand what variables are playing role in traffic crashes happening in the City of Chicago. Our focus of research is accidents leading to fatal injuries (at least 1) which will enable us to prioritize those crashes first. The analysis would open our view towards what could be possible reasons behind common crashes leading to injuries.

## Methodology Adopted
-In order to have a general view of the situation, we have sampled 10,000 crashes from the whole data to perform our analysis. This helps us in two ways: 1) Optimizing and making the analysis efficient 2) Randomised distribution of events 
-Moreover, to make the analysis more meaningful, we picked up data which leads to at least 1 injury in the crash. 


## Facts Discovery

### How are number of injuries in a crash related to Posted speed limit of the street 
![image](https://user-images.githubusercontent.com/98545133/190727548-a290b4f2-b426-4b03-b0d4-fc079c9ab863.png)

#### Observation
This is a scatterplot between posted speed limit on the road where crash took place and the number of injuries suffered in the crash.
There seems to be no relation between posted speed limit on a road and number of injuries suffered in the traffic crashes.
This shows that accidents are spread accross all varieties of roads and not particular to certain speed limit roads
Though the maximum that we observe is for speed limit 30


### What weather conditions are crashes happening in?
![image](https://user-images.githubusercontent.com/98545133/190727841-7f858b13-11ec-4553-ae98-40956bf25b80.png)

#### Observation
This graphs plot the count of crashes for every Weather Condition of the location when the crash took place.
The majority of traffic crashes (approx 80%) take place in clear weather condition and there is drasatic uneven distribution of values among all the categories of weather condition.


### How do crashes look like over the weekdays and at what time doe they happen?
![image](https://user-images.githubusercontent.com/98545133/190728175-1c7c59b0-6e98-4d44-8e55-9365c139dd86.png)

#### Observation
In this graph we have plotted count of traffic crashes per day and for each hour in the day.
Through the countplot we are able to plot the number of records (or traffic crashes) we have for each day and each hour We are obervering that Friday has the maximum number of traffic crashes in the whole week.
Also with time perspective we witness that the plot for all days peaks in the middle which shows that the traffic crashes are happening in noon (between 1100 hrs and 1300 hrs, ie: 11am and 1pm)

### What kind traffic control devices are installed where crash took place
![image](https://user-images.githubusercontent.com/98545133/190730085-7579b68c-f5bc-43be-a5e3-69988bd4a1f1.png)

#### Observation
We have plotted the type of control device installed on the road where the crash took place.
We witness here that near about 4000 traffic crashes had no traffic control device installed on the road which could be a major reason for crashes

### What is the primary cause of the crash?
![image](https://user-images.githubusercontent.com/98545133/190730254-943c8537-482b-4e51-bbd8-5ad0ad1178dc.png)

#### Observation
We are visualizing frequency distribution of the primary cause of the crash as reported by the field officer.
A lot of data is tagged as Unable to Determine as a primary cause of the crash. While, apart from that we see that 'Failing to Yield Right of the Way' is the most common cause of the crash and comprising close to 20% of the all the crashes under study.

### How does the impact of crashes look like?
#### Created a variable Injuries_to_Vehicles_Ratio which is calculated by total number of injuries in a crash over number of vehicles invlved in the crash

![image](https://user-images.githubusercontent.com/98545133/190791759-7f1c764f-2140-49da-b8a3-ff0e44026a7c.png)

#### Observation
The variable measures the ratio of number injuries suffered to number of vehicles involved in the crash.
The plot shows distribution of major values between 0 to 3.
The ratio could be useful in judging the impact of the crash. The higher the ratio value means low number of vehicles leading to higher number of injuries and vice-versa.
This ratio could also add meanig to geo-spatial analysis where we could oberve what locations are having higher Injuries_to_Vehicles ratio.

## Concluding Remarks
Roads with no controls devices are more prone to fatal accidents
Rear end collisions are most frequent occuring type of crash.  West and South bound directions have the most crashes amongs all the categories.
Analysing the reason for the crash, we found a lot of data is tagged as 'Unable to Determine' as a primary cause of the crash. While, apart from that we see that 'Failing to Yield Right of the Way' is the most common cause of the crash and comprising close to 20% of the all the crashes under study.




