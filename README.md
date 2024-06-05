# AB testing for Cookie cats

## Purpose
To perform AB testing on player retention for Cookie Cats where we are comparing the gates at level 30 and 40. A gate signifies a paywall or limit. To remove the gate, the player can either make an in-app purchase or wait a time period.

Data was sourced from [Kaggle](https://www.kaggle.com/datasets/yufengsui/mobile-games-ab-testing/data) which was sourced from [Datacamp](https://www.datacamp.com/projects/184).

## Process
I started by loading the data and checking or any data integrity issues like nulls and duplicates. I also performed some data cleaning/formatting like changing data types and changing booleans to numeric.

I performed EDA next. I looked at each feature by itself and in relation to other features. 

I initially just performed non-parametric tests due to time constraints, but hope to return and transform the data to explore parametric tests

I formulated some hypotheses to test:
- Sum Game rounds
    - H0: There is no difference between the average sum game rounds for the gate_30 and gate_40 versions
    - Ha: There is a difference between the average sum game rounds for the gate_30 and gate_40 versions
    - test to use: Mann-Whitney U

- retention_1
    - H0: There is no difference between the gate_30 and gate_40 versions and the number of users who log on one day after downloading
    - Ha: There is a difference between the gate_30 and gate_40 versions and the number of users who log on one day after downloading
    - Test: Chi-Square

- retention_2
    - H0: There is no difference between the gate_30 and gate_40 versions and the number of users who log on seven day after downloading
    - Ha: There is a difference between the gate_30 and gate_40 versions and the number of users who log on seven day after downloading
    - Test: Chi-square


## Results
