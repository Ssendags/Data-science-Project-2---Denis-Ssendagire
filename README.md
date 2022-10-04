# Data-science-Project-2---Denis-Ssendagire

Individual Income Predictions
Data Science Course Project

Preprocessing of Data and Creation of Income Prediction Model
Author: Denis Ssendagire

Business problem:
An individual’s income is a result of various factors. It is influenced by the individual’s education level, age, gender, occupation, etc. It is a classification problem.

Data:
Acknowledgements This dataset named “adult” is found in the UCI machine learning repository http://www.cs.toronto.edu/~delve/data/adult/desc.html The detailed description on the dataset can be found in the original UCI documentation http://www.cs.toronto.edu/~delve/data/adult/adultDetail.html
The data constitutes of demographics and other features to describe a person. The intention is to explore the possibility of predicting income level based on the individual’s personal information.

Attribute Information:

- age: continuous.
- workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.
- fnlwgt: continuous.
- education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.
- education-num: continuous.
- marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.
- occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, - - Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.
- relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.
- race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.
- sex: Female, Male.
- capital-gain: continuous.
- capital-loss: continuous.
- hours-per-week: continuous.
- native-country: 

Methods
- Data Exploration is done using info(), shape(), unique(), duplicated() methods. Data is checked and addressed for: duplicates, missing values, incorrect data types,    inconsistencies and incorrectiness.

- For duplicates one insitance of duplicated data is retained while the others are dropped.
- Inconsistencies are standardised
- Ordinal data is encoded.
- Train-test split is performed on the data.
- Missing values imputed during preprocessing.
Categorical data converted to numerical data during preprocessing.
Data is prepared (preprocessed) for Machine Learning by using SimpleImputer, OneHotEncoder, Pipelines and Column Transformers.
Models are built and evaluated: Logistic Regression and Decision Tree Classification.

Results
Explanatory Data Analysis:
![image](https://user-images.githubusercontent.com/109603891/193822965-35c3e2f2-93e8-4733-9109-79605c051b07.png)

Img 1: Number of Peole Per Income Group.

![image](https://user-images.githubusercontent.com/109603891/193823325-cfdd39c9-9468-46b6-9ae6-7b1fe74741ec.png)

Number of People per Race.

![image](https://user-images.githubusercontent.com/109603891/193824189-cbe815cb-9eae-46a4-b522-49d1112839aa.png)

Distribution of Gender

![image](https://user-images.githubusercontent.com/109603891/193825197-20798d85-33e1-404f-8e8c-adbf513b122b.png)

Visualisation of one of the Logistic Regression model

From the above visualisations:
- It is evident most people are married or never married (Img 1).
- Img 2 shows that most people belong to the white race.
- Img 3 shows gender distribution per income group.

Best Fitting Model:
Decision Tree Classification Model gave an accuracy of 81.55% but with overfitting. Decision tree classification model achieved 86.07% accuracy with Logistic Regression model achieving: L1 tuning at 85.19% and with L2 tuning at 85.07%.

In this case the Decision Tree Classification model is most suitable to be deployed.

Recommendations:
In this case the Decision Tree Classification model is most suitable to be deployed.

Limitations & Next Steps
Given that the best fit attained is 86%, it is in consideration to develop and evaluate other models until the highest best fit is achieved.

For further information
For any additional questions, please contact ssendags@gmail.coml
