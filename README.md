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
fnlwgt: continuous.
education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.
education-num: continuous.
marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.
occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.
relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.
race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.
sex: Female, Male.
capital-gain: continuous.
capital-loss: continuous.
hours-per-week: continuous.
native-country: 
Methods
Data Exploration is done using info(), shape(), unique(), duplicated() methods. Data is checked and addressed for: duplicates, missing values, incorrect data types, inconsistencies and incorrectiness.

For duplicates one insitance of duplicated data is retained while the others are dropped.
Inconsistencies are standardised
Ordinal data is encoded.
Train-test split is performed on the data.
Missing values imputed during preprocessing.
Categorical data converted to numerical data during preprocessing.
Data is prepared (preprocessed) for Machine Learning by using SimpleImputer, OneHotEncoder, Pipelines and Column Transformers.
Models are built and evaluated: Linear Regression and Regression Tree.
Results
Explanatory Data Analysis:
image

Outlet Sales by Outlet Type.

image

Outlet Sales by Outlet Location Type.

From the above visualisations it is evident that Outlet sales have a pattern with each of Outlet Type and Outlet Location Type.

Best Fitting Model:
image image

Visualisation of tuning using max_depths values and what R^2 values they give giving the best fit at max_depth 5.

Model
From the 3 models considered above the regression tree model has given better values (training = 60% and testing = 60%) making it the best fit, this as compared to R^2 which was found to be too low (Training = 1 and Testing = 0.00022) and RMSE which was found to be too high (Training = 8.32 and testing = 72.39x10**12).

Recommendations:
In this case the tuned (max_depth = 5) regression tree model shall be considered for deployment.

Limitations & Next Steps
Given that the best fit attained is 60%, it is in consideration to develop and evaluate other models until the highest best fit is achieved.

For further information
For any additional questions, please contact ssendags@gmail.coml
