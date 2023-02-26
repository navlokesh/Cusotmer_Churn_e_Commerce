# Cusotmer_Churn_e_Commerce
# Problem Statement:
The data set belongs to a leading online E-Commerce company. An online retail (E commerce) company wants to know the customers who are going to churn, so accordingly they can approach customer to offer some promos.
### Need for Solving it:
Customer retention: It is one of the very important aspect for business. Once a customer goes to an e-Commerce website and order something there is a possibility that the customer would come back and buy more things (If they are happy with the experience). Customer retention helps in generating higher customer lifetime value and hence the revenue. It is good to have new customers, but existing customers bring more revenue than the new ones.

There are many ways to achieve customer retention but the most commonly used model is- Churn Model. Churn Model helps identifying customers who are most likely to switch to different e-Commerce website. Once identified the company can take actions in order to keep its existing customers. Now the question is, how does Churn model identify these customers? The model can be used to calculate the churn rate and depending on the nature of business, different metrics can be used. Few common metrics are - • Number of customers lost • Percent of customers lost

### Business/Social Opportunity:
The Churn Model provides opportunities to the businesses in many ways. Few advantages of implementing Churn Model in e-Commerce are - • Churn rate can help identifying churn customers and accordingly businesses can run retention campaigns. • It will help in the keeping the revenue flowing. • Churn Model can help business to maintain customer lifetime value. • It helps businesses to track the progress. • The inputs received from Churn Model can be very helpful for BI activities.

# EDA and Business Implication:
Uni-variate, Bi-variate and Multi-variate analysis to understand relationship between variables.
Checked skewness of the data, histogram of all the features, Boxplots, Bar graphs, pie charts, pairplots, heatmaps, correlation, etc.

### Analysis => Business Impact
A customer churning out doesn’t mean he/she stopped buying products online. They might have just moved to a different e-commerce company.
This will directly impact the revenue of the business.
The market share of other companies will increase, and the market share of our company will decrease.
Saving the churns will help us keep the revenue flowing and giving better customer experience by collecting feedbacks.

### Both visual and non-visual understanding of the data.
There are 16.8% of the total customers who are churning
Male and Female customers show similar behavior in churning
21.3% of total customers present in Tier 3 cities are churning which is greater than the overall churn percentage

# Data Pre-processing:
Missing value treatment, outlier identification and treatment, variable transformations, feature scaling by bringing all the features on the same dimension level.

# Model Building:
Performed model training on most of the classification Machine Learning Algorithms, such as:
Decision Tree Classifier, Random Forest Classifier, Artificial Neural Networks, Logistic Regression, Linear Discriminant Analysis, Naïve Bayes Classifier, Support Vector Machines, ADA Boost and XG Boost.

# Model Evaluation:
Checked model performance for all the models trained above using accuracy_score, Precision, Recall, F1 scores, roc_auc_scores using confusion matrix, classification report and roc_curve.

# Interpretation of Model performance:
Considering that we are working on a customer churn problem, recall will be one of the most important factors for us to decide on which model is giving the best results.
Checking on the Recall and Accuracy of all the models:
### Tree algorithms:
Decision Tree Classifier has a better recall when compared with Random Forest Classifier. Random Forest Classifier has a slightly better accuracy when compared with Decision Tree Classifier.
### Artificial Neural Network:
The algorithm has similar performance compared to the other tree algorithms.
The accuracy of test data is slightly better than train data
### Logistic Regression:
The algorithm has least recall value when compared with all of the other algorithms.
The accuracy score seems to be same when compared with above algorithms.
### Linear Discriminant Analysis:
The metrics show that this algorithm has one of the least recall when compared with all other algorithms.
But the accuracy score looks similar to the model built on Logistic Regression.
### K-Nearest Neighbors:
This model has one of the highest recall value when compared with other algorithms.
However, the accuracy score looks similar as most of the other algorithms.
### Naïve Bayes:
The model has the highest recall value when compared with other algorithms.
However, the accuracy score looks similar as most of the other algorithms.
### Support Vector Machine:
The recall value is the least when compared with other algorithms.
The accuracy score also is very low when compared with other algorithms.
### Boosting algorithms:
ADA Boost and XG Boost have better model performance considering the metrics and compared to other models above.
XG Boost seem to been performing slightly better compared to ADA Boost both in terms of accuracy and recall factor.

## From the above comparison, we can see that Naïve Bayes model is best performing for our data followed by K-Nearest Neighbors model.

# Model Optimization:
Further scaling of data was done and selected models were re-trained.
Tuned the models using automated hyperparameter tuning using grid search and param grid techniques.

However, the results did not change much. The metrics are almost same as the model built on non-scaled data.

# Further Optimization:
The data is very imbalanced. There are only 16% of ones and rest are of 0 class. This shows that the data is very imbalanced.

Used SMOTE technique to achieve balance in the data.
Re-trained the models on new balanced data.
Applying SMOTE technique on the scaled dataset helped in better results.

# Model Validation:
Accuracy of the model will not completely tell us the model performance.
Recall meaning – What percentage of churners are captured correctly by the model.
In our project, the recall factor is important since it is customer churn analysis and we do not want to miss out on the potential churners
Hence, a combination of Accuracy and recall factor is chosen for model validation

# Final interpretation / recommendation
### Interpretation:
The analysis was made after applying multiple algorithms on normal data, scaled data and after applying SMOTE technique to balance the data after scaling.
The performance metrics of original data and scaled data seem to be similar.
The performance metrics for models built on the balanced data show way better results when compared with the other models.
From the above analysis, we can see that the model built on XG Boost looks to be performing the best for us.
The best results are seen when the model is built using the scaled and balanced data.
XGBoost has in-built L1 (Lasso Regression) and L2 (Ridge Regression) regularization which prevents the model from overfitting.
This model will be one of the best to use for our analysis of customer churn for this business due the metrics such as Recall and Accuracy being the best when compared with others. This is also better considering the below:
We can consider XG Boost model for our further analysis as this model shows the best metrics during the model evaluation.
The XG Boost model is advantageous as well. It does non-greedy tree pruning, built-in cross-validation and handling the missing values.

### Recommendation:
The Company can consider starting to collect the feedbacks to understand what makes customers unhappy which can cause their churning
The company can consider promotional offers in the area where churning rate is seen to be high
#### Few ways to stop churning:
Giving cashbacks and free promotional cash to lure them to buy from our company.
Start a payback card and actively communicating the offers and discounts they can avail.
