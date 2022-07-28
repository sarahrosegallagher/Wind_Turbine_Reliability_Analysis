# Wind Turbine Reliability Analysis

## Forward 

* This repository has an associated Heroku web application: <wind-turbine-reliability.herokuapp.com>
* The visualization tab exceeds Heroku's RAM allowance, but launching app.py locally will build the necessary files to run the application on a local server. 

## Background

* Selected topic and reason


Wind turbine reliability. Decrease cost and increase reliability. The intent is to build a machine learning algorithm to predict wind turbine failure. A major component failure occurs on average annually on a wind turbine. With high repair costs for catostrophic failures, predicting these failures would lead to a much lower cost in maintainence. 

* Data source description

Real time monitoring data for 29 wind turbines on 66 features from 2019 to 2020. Measurements averaged and recorded every 10 minutes. 10 million records for 19 features of interest for gearbox performance. 

* Questions we hope to answer with data 

Which features that are measured can give a leading indicator on gearbox failure?

Can we predict wind turbine gearbox failure with sensor data?

## Communication Protocols 

* GitHub

* Slack

* Google Drive

* Zoom Meetings 


## Models Plan
After preliminary data cleaning and transformation we intend to investigate the data descriptive statistics, histograms, and feature correlations to the targets. After which, some features may be dropped or merged depending on results. 

#### Unsupervised Learning
Next we intend to conduct a K-Means unsupervised Machine learning analysis to further investigate grouping within the data to inform the analysis design. Then, we intend to use a Random Forest supervised learning model to predict turbine failure withing a target window. 

#### Supervised Learning
We intend to conduct a preliminary evaluation several models increasing in power/complexity with each iteration. Each model will be evaluated for performance. After preliminary evaluation, we will optimize performance through feature reduction/elimination, bagging/boosting, activation changes or neural network configuration changes depending on the model choice and optimization options available. 

Test order:
  * Logistic regression
  * Support Vector Machine
  * Random Forest with feature importance testing
  * Neural Network (still investigating which one to use for this case)

 
 ## Presentation Plan
 Potential Outline:
   * Could start with a full exec summary like an abstract, i.e. super short summary of all elements
   * Background, problem description, business case
   * Summary of  Approach
       * Raw data investigation
       * Subject matter expert interviews
       * Wide web and textbook search for best practices
   * Description of data
       * What is in it, where it comes from, 
       * a few descriptive images
   * Description of database architecture and preprocessing (probably a chart like the one mocked up in the google slides)
   * Description of exploratory analyes (high level overview of maybe individual turbine tests)
   * Description of overall database analysis 
   * Results
   * Summary
       * Review Approach
       * report what we found (or didn't find)
       * Describe limitations (data itself, approach, algorithms and optimization, generalizability, etc.)
       * Highlight improvements that could be done to improve approach or work to be dont to implement in real world
