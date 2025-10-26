## Project Title: The Oguri Model

## Authors: Ryan Duong, Andrei Duque

## Description of Question and Research Topic (5 Sentences)

## Project Outline/Plan

### Data Collection Plan (two parts, one for each author)

Hong Kong Race Horses (Ryan):
If allowed: https://www.kaggle.com/datasets/deltaromeo/horse-racing-results-ukireland-2015-2025/data
If these kaggle datasets are allowed, then the topic would change from comparing Japanese Race Horses and Hong Kong Race Horses to Japan Race Horses and European Race Horses.

Otherwise (more preferred): https://racing.hkjc.com/racing/information/english/Horse/SelectHorse.aspx

Using the data from the Hong Kong Jockey Club database, we will individually select 100 (or more, if desired) horses and record the necessary attributes. It is important to choose attributes that also exist in the JBIS database, so that comparisons can be made.

The following attributes would be scraped from the database and used to train the models:
Date
RC/Track/Course (Race Condition, Track)
Dist. (Distance)
Length Behind Winner (LBW)
Finish Time
Declar. Horse Wt. (Weight) / Act. Wt.
Pla. (Placed)
Sex

Example page from Hong Kong Jockey Club database:

[hkdbimage](hkracehorse.png)

Margin and Finish Time will also be the predicted values for the multiple linear regression models.

### Model Plans (two parts, one for each author)

Model Plans (Ryan):
Mini model 2 (multiple linear regression model): To measure how dominant a horse is in a race (raises likeliness to win a race), we want to use the predicted horse’s time, race grade, distance, condition, field strength (turf or dirt?), and use it to predict the margin (distance between the winning horse and second place).

Model Plans (Andrei/ Ryan):
Main model (logistic regression): Using the predicted values, and the horse attributes (these are also used in mini models, nothing new introduced), we want to predict whether a horse will win. The weights for this model will also likely include race attributes such as distance and condition which are needed since races have different conditions.

### Project Timeline

Project Timeline:

10/26 - Submit Proposal for Problem of the Week

11/2 Find Appropriate Datasets/Gather Relevant Data

11/9 Finish Data Preprocessing

11/16 Test first iterations of models 

11/23 Continue tuning hyperparameters

11/30 Write conclusions on results + finish presentation slides

12/2 - Presentations

12/11 - Final Submission
