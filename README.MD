# Titanic : Machine Learning From Disaster

## Predict survival on the Titanic

<img src="https://static1.squarespace.com/static/5006453fe4b09ef2252ba068/5095eabce4b06cb305058603/5095eabce4b02d37bef4c24c/1352002236895/100_anniversary_titanic_sinking_by_esai8mellows-d4xbme8.jpg" alt="Titanic Disaster" style="width: 720px;"/>

<p style="text-align: center;">
  <small>
    [See <a href="https://www.kaggle.com/c/titanic/overview">Titanic - Machine Learning from Disaster (Kaggle URL)</a>]
  </small>
</p>

## Introduction

<br>

### Object

<br>

This competition can make you dive into ML competitions and familiarize your self with how to solve Kaggle problem.

<br>

This competition's object is so simple : Create Machine Learning algorithm that predicts which passenegers survived in the ship.

On April 15, 1912, Titanic sank after colliding with an iceberg. Unfortunately, there weren't enough lifeboats for everyone onboard, resulting in the death of 1,502 out of 2,224 passengers and crew. (The lifeboat has s capacity of only 1,178 people only. So, only 706 people were rescued.)

<br>

### Data Fields from Titanic)

<br>

- Survived : 0 = died, 1 = survived

<br>

- Pclass : Ticket class for passengers
  - 1st = Upper
  - 2nd = Middle
  - 3rd = Lower

<br>

- Sex : gender of passengers (composed of male and female)

<br>

- Age : Passenger's age (if age less than 1, it's fractional)

<br>

- Sibsp : The sibsp defines family relations in this way.
  - Sibling = brother, sister, stepbrother, stepsister
  - Spouse = husband, wife

<br>

- Parch : The parch defines family relations
  - Parent = mother, father
  - Child = daughter, son, stepdaughter, stepson

<br>

- Ticket : Number of ticket

 <br>
 
 * Fare : Fare fee of Titanic
 
 <br>
 
 * cabin : Cabin number
 
 <br>
 
 * embarked : Port of Embarkation 
   - C = Cherbourg
   - Q = Queenstown
   - S = Southampton
   
   <br>
   
### Evaluation

<br>

Our goal is to predict whether the passengers in test.csv have died or not individually. (Use Classifier)

 <br>

Your score is the percentage of passengers you correctly predict. This is known as accuracy.

 <br>

$$ Accuracy = \frac{TP + TN}{TP + TN + FP + FN} $$

 <br>

TP = True positive; FP = False positive; TN = True negative; FN = False negative

### Precedure [[See link]](https://github.com/ChaHoHyun/Bike-Sharing-Demand_score_0.3794/blob/main/Bike%20Sharing%20Demand_registered_Score_.ipynb)

There will be follow steps for how to solve this problem. [[See link]](https://github.com/ChaHoHyun/Titanic_score_0.811/blob/main/Titanic_0.811.ipynb)

1. Import CSV file by using Pandas (Collecting Data)
2. Exploratory Data Analysis (EDA)
3. Explore (Preprocessing)

4. Training (For Machine Learing - **Decision Tree**)

5. Visualization

![image](./Visualiztion_of_DecisionTree.png)

6. Submit

   Through the fit and predict of the decision tree, we predicted whether or not the passenger in the test data was survived. Now all we have left to do is to organize them according to the submission format recommended by Kaggle ([kaggle](http://kaggle.com/)) and save them as a file.

   Kaggle's Titanic Competition ([Titanic: Machine Learning from Disaster] (https://www.kaggle.com/c/titanic)) offers a submission format called **gender_submission.csv**. ([Download Link](https://www.kaggle.com/c/titanic/data)) We will insert and store our predicted values in this submission format.
