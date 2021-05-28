# Titanic-Dataset-Analysis
A data-based approach to uncover what sorts of people were more likely to survive in one of the most infamous shipwrecks.
Read detailed blog [here](https://medium.com/@garvitkataria/would-you-have-survived-on-sinking-titanic-e534d4acef33).
## CRISP-DM approach
#### Business Understanding
We will be trying to answer the following questions - 
1. Were the rich given priority while assigning lifeboats?
2. Were women evacuated first?
3. How did family size impact the chance of survival?
4. How important were boarding point and cabin location?
#### Data Understanding
1. The dataset has information on 1309 passengers who boarded the ship. It comprises 12 attributes of passenger information like name, age, gender, socio-economic class.
2. Roughly 20 percent of the Age data is missing. The proportion of Age missing is likely small enough for reasonable replacement with some form of imputation. Looking at the Cabin column, it looks like we are just missing too much of that data to do something useful with at a basic level. We'll probably drop this later, or change it to another feature like "Cabin Known: 1 or 0"
3. Sex and Embarked are categorical features which we'll need to convert to dummy variables using pandas! Otherwise our machine learning algorithm won't be able to directly take in those features as inputs.
#### Prepare Data
1. Imputed passenger age according to average age in Passenger class as wealthier passengers in the higher classes were found to be older.
2. Handled the categorical variables like Sex and Embarked
3. Extracted cabin distribution and level of cabin from 20% of available fields.
#### Data Modeling
Used logistic regression to for prediction and got 81% accuracy.
#### Evaluate the Results
Conclusions made after exploring the Titanic dataset
1. Women and children were given priority during the evacuation process and had much higher chances of surviving.
2. The wealthy first-class people had a good chance to survive irrespective of their boarding location.
3. Midsize families had a higher chance of surviving than lone individuals and large families.
4. Finally, we looked into the location of rooms in the Titanic and found out that people in upper blocks, nearer to the deck, were better off in comparison to mid and lower blocks (towards the bottom of ship and farther from the deck).


### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using Titanic Dataset to better understand:

1. How was evacuation prioritized when ship was sinking?
2. Were the rich given priority while assigning lifeboats?
3. Were women and evacuated first?
4. How did family size impact the chance of survival?
5. How important were boarding point and cabin location?

## File Descriptions <a name="files"></a>

There are three files available here to showcase work related to the above questions. The notebooks is exploratory in searching through the data pertaining to the questions showcased by the notebook title.  Markdown cells were used to assist in walking through the thought process for individual steps.  

At the end of the notebook, there is necessary code to obtain the final model used to predict whether person will survive or not.

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@garvitkataria/would-you-have-survived-on-sinking-titanic-e534d4acef33).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

You can find the Licensing for the data and other descriptive information at the Kaggle link available [here](https://www.kaggle.com/c/titanic).  Otherwise, feel free to use the code here as you would like! 

