# Company-Bankruptcy-Prediction

**1. Business problem and motivation**
The ability to predict corporate bankruptcy would be beneficial for several
stakeholders, including:
- Investors
- Creditors
- Financial service institutions such as banks, insurance companies, etc
- Corporation themselves so that they can change their financial structure
- Employees
The prediction of bankruptcy in companies is a problem that has concerned
entrepreneurs, researchers and even governments for years, since detecting early
signs that a company is going to enter bankruptcy involuntarily and being able to
save it from that process, can help reduce the economic losses that bankruptcy
entails, both in quantitative and qualitative terms.

**2. Dataset:**
https://www.kaggle.com/fedesoriano/company-bankruptcy-prediction
The data were collected from the Taiwan Economic Journal for the years 1999 to
2009. Company bankruptcy was defined based on the business regulations of the
Taiwan Stock Exchange.

**3. Aims of the study**
The aim of the study is to narrow down the variables that could potentially predict a
company's bankruptcy and to know the value of these variables at which it is likely
that the company will bankrupt.

**4. Research Questions**

This project is an exploratory study that identifies the relevant indicators for the classification of corporate bankruptcy in Taiwan from 1999 to 2000. The research questions are determined as follows:
- Which variables play the most important roles in company bankruptcy?
- How unbalanced data affect the prediction result?
- Which model is the best for predicting bankruptcy? Why?


**5. Methods**

To highlight the positive effect of rebalancing, we first train a model on the original, unbalanced data set.
Next, we will use SMOTE (Synthetic Minority Oversampling Technique) to rebalance the training data.
Finally, we train the actual model (that we expect to perform better) using the rebalanced data.
In order to compare models, we apply these steps to train three different models: Logistics Regression, Decision Tree and SVM
To evaluate models, we will use the following evaluation methods:
- Confusion matrix
- AUC (Area Under the Curve) and ROC curve

**6. Conclusion**

- The project focused on decision trees, SVM, and logistic regression. The full potential of other models for predictions in the data set at hand should be explored in future research endeavors.
- Rebalancing significantly improves the results
- Features like Fixed Assets to Assets, Operating Expense Rate could provide policy implications for all of the involved stakeholders in early bankruptcy detection.
- As for bankruptcy prediction, the balanced decision tree model is able to predict a few bankruptcy, albeit with large amount of false positive.

**7. Limitations and Future work**

- The current max depth of Decision Tree model is 3, which could make the model underfitting. Therefore, we will try to find the best max depth
- We could try different methods of feature selection in order to deal with multicollinearity such as PCA or partial least squares regression
- We could also explore other models for prediction in the dataset such as Logistics regression model with L1 and L2
- With model evaluation, we can use K-fold and Gain Charts to aid model evaluation process. In addition, we will consider using expected benefit from confusion matrix to further understand the true implications of each model especially regarding the cost/benefit of false positives and false negatives.
