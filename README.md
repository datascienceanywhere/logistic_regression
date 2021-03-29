![image](https://user-images.githubusercontent.com/75901421/112805389-27f6a580-9093-11eb-8658-a6ee7d93df54.png)
# Building A Logistic Regression in Python, Step by Step

  **Logistic Regression** is supervised classification algorithm where we will used to classify the categories. In logistic regression the output of the estimator is discrete or categorical. The idea of Logistic regression is started from the intuition of Linear regression. For example as from the figure -1 suppose there are two classes, class 0 and class 1 and we need to estimate the classes using independent variable X. For that we can start with the idea of simple linear regression where we fit a line for the samples independent variable and dependent variable (class). Now with the simple linear regression (solid yellow line) we can estimate the probability. Lower the probability we can estimate as class 0 and higher the probability we can estimate as class 0.

Now the question is what is the threshold probability that we need set to class of the sample. By default we can consider 0.5 is the threshold probability and estimate the class. Now here there is problem for default threshold probability = 0.5. Suppose that there are extreme values (not outliers) of X, by common sense we can say that these are also belongs to class 1.

Now when you build a linear regression with the extreme values the linear regression will looks like yellow doted line. And for now default threshold value 0.5 is not approximation for selection or estimation of classification. This phenomenon occurs because, linear regression fit the based on least square regression and hence least square is not appropriate for this problem. To tackle this problem Logistic regression use Maximum Likelihood Estimation (MLE).
In MLE, the Goal is to maximize likelihood.
In most Data Science optimizations, the goal is to find minima using calculus (minimize sum of squared errors in linear regression, and so on) or numerical techniques like Gradient Descent (minimize deviance in logistic regression, and so on)
Maximum Likelihood => Minimum of Negative Log-Likelihood.

## Logistic Regression in Python

### Step-1: Develop transformed linear regression and computer probability of each data point

*Output of Probability Using Linear Regression*

![image](https://user-images.githubusercontent.com/75901421/112804962-a6067c80-9092-11eb-8790-7ebf5f5b6028.png)

### Step-2: Find the best odd ratio using MLE.
*Output of Maximum Likehood Estimation*

![image](https://user-images.githubusercontent.com/75901421/112804874-8a02db00-9092-11eb-8a70-50477889753a.png)

### Combining Linear Regresision and Odds Ratio = Logistic Regression

![image](https://user-images.githubusercontent.com/75901421/112805200-ea921800-9092-11eb-8841-f8fc337f3a3a.png)

---
by *[datascienceanywhere](http://datascienceanywhere.com)*
