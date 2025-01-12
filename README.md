# FlightFinalApproachAnomalyDetection

## Team 1 AAI-540: Machine Learning Operations

**Project Title:** Flight Final Approach Anomaly Detection and Classification

**Project Status:** Active

## Project Intro/Objective

 The model will use time series data from 99,000 flights to predict either a nominal landing or one of three types of anomalies. During aircraft events and incidents, time is of the essence. If the anomaly can be detected automatically or ideally predicted earlier than alarms would typically trigger, this facilitates an earlier intervention which can be of pivotal importance for safety.


### Goals:

- Accurately predict the class for the time series of the flights
- Evaluate feasibility of prediction of the class prior to completion of the time series, or with a moving window
- Find patterns that generalize well across all flights, not just for particular arrival airports or runways


## Contributors

- **Elan Wilkinson**
- **Melissa Short**
- **Nick Short**

## Methods Used

- Data Preprocessing
- Train Test Split
- Model Training
- Metrics

- - **Programming Language:** Python
- **Models and Libraries:** 
  - Numpy
 
  - ## Project Description

The model will be generating predictions for a multiclass multivariate time series classification problem with four exclusive labels. During development, the model will be evaluated on a holdout subset of the available training data. Later phases at greater levels of maturation will involve incorporating data from additional flights over time.

 Standard classification metrics will be used for evaluation including recall, precision and F1 scores, but much higher priority will be given to recall for anomaly classes, as false positives are much more acceptable than false negatives in the given context. The model would be continuously monitored as more flights occur over time and additional data become available, either validating existing performance or showing drift. While automatic notifications could be set to trigger at certain performance values or failures, manual human review could be conducted as part of regular safety maintenance. For training, the datasource comes nasa.gov from Bryan Matthews (https://c3.ndc.nasa.gov/dashlink/resources/1018/Links to an external site.), a member of the intelligent data understanding group at NASA. The samples come from approximately 99,000 flights on final approach when the flights are crossing 1,000 ft before touchdown. There are 20 different measures of aircraft readings for each of the 160 seconds leading up to touchdown. 

Our thanks and appreciation go to our professor **Jules Malin**.
