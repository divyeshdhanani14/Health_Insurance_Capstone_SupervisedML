# Health_Insurance_Capstone_SupervisedML


![Untitled](https://user-images.githubusercontent.com/107920120/211268678-e3a60bb1-c381-4a64-b6e0-9061874a5fe8.png)


Our client is an insurance company that has provided Health Insurance to its
customers. Now they need your help in building a model to predict whether the
policyholders (customers) from the past year will also be interested in Vehicle
Insurance provided by the company. In this Supervised Machine Learning
Classification Project, we will be building a model to predict whether a customer
would be interested in Vehicle Insurance. This will be extremely helpful for the
company because it can then accordingly plan its communication strategy to reach
out to those customers and optimize its business model and revenue.
In order to predict whether the customer would be interested in Vehicle insurance,
we will consider the following information about the customers which includes
demographics (gender, age, region code type), and Vehicle, we checked the
duplicate values, null values, outliers, and feature scaled the outliers for further
analysis.

In the Exploratory data analysis, we visualized the distribution of the data for age,
region, and policy channel variables, categorizing Age features as young_age,
middle_age, and old age, and Region_Code as Region_A, Region_B, Region_C. We
also categorized the Policy_Sales_Channel into channel_A, channel_B, and
channel_C. Further, explored the categorical variables and Annual Premium relation
with all other features of the dataset. Checked the correlation of the dataset using
the Kendall method and feature importance of categorical variables. Our EDA gave
us the results that customers belonging to the young_age are more interested in
Vehicle response whereas Customers having a vehicle for more than 2 years are
more likely to be interested in Vehicle Insurance. Similarly, Customers owning
damaged vehicles were also more inclined toward Vehicle Insurance.


As a first step before starting machine learning modeling, we encoded the
categorical features in our dataset using One hot encoding. For Hyper-parameter
training, the HalvingRandomizedSearchCV method was used as other methods
turned out to be more time-consuming. Created a function for the machine
learning algorithms and model implementation. We have used Logistic Regression,
Gaussian Naive Bayes, Decision Tree, Gradient Boosting, and Bagging Classifier
models for training the dataset of which Bagging classifier gave an acceptable
accuracy score of around 85% in comparison to other models without underfitting
or overfitting the data. For Gaussian Naïve Bayes Classification Algorithm, we got an
accuracy score of 68% and for the Decision Tree, Gradient Boosting and Bagging
Classifier accuracy score was around 82-87%. We select our best model as Bagging
Classifier considering precision and recall, as we have an unequal number of
observations in each class in our dataset, so accuracy alone can be misleading.
