# Bank_Marketing

### Intro

An important source of income for banks is term deposits, i.e., deposits made by customers at a fixed rate for a fixed time. This capital can be used to disburse loans at a higher interest rate. Therefore, banks use various marketing techniques to encourage customers to save via term deposits. These techniques include email, advertisement, phone, and digital marketing. Telephonic marketing (i.e., phone calls) is particularly effective in acquiring term deposit customers, especially when guided by quality estimates of customers’ inclinations to save via term deposits. Banks might use data and machine learning-informed alert models to identify customers who are more likely to save via term deposits and inform a telephonic marketing campaign accordingly.

The dataset is related to the direct telemarketing campaigns (phone calls) of a European banking institution.

The goal is to use machine learning techniques to predict if the customer will subscribe to a term deposit (Term Deposit = 1).

### Part 1:
In this part, I explore the dataset, prepare it for analysis, and plot some basic graphs to understand the relationship between variables.

### Part 2:
#### Part 2a:
Here, I fit a logistic regression model on the dataset to assign an observation to the Term Deposit = 1 class. I evaluate its performance given probability thresholds of 10%, 20%, 35%, and 50%, and compute a confusion matrix for each threshold to compare the models.

#### Part 2b:
Next, I evaluate the predictive power of the logistic model by splitting the data into a 70% training set and a 30% test set. I perform 5-fold cross-validation on the training set.

### Part 3:
In this section, I repeat the same process as in Part 2b but use a random forest classifier, decision tree, and bagging classifier. Then, I compare their predictive power to that of the logistic model.

### Part 4:
In the last section, I explore whether unsupervised ML models can increase predictive power. I use principal component analysis and K-means clustering. Spoiler! It turns out that roughly 90% of the data can be explained by the first three principal components (PCs). I proceed by using the 3 PCs as the input variables for the four supervised ML models used throughout (Part 2b). Lastly, I use K-means clustering on the 3 PCs and find that k=6 is the optimal number of clusters. Then, I run the four ML models with the 3 PCs and the clustering categories as input variables and compare their results (Part 2b).
