## <h1><b>Compare Classifiers</b></h1>

## <h3>Overview:</h3>
<p>
In this practical application, our goal is to compare the performance of the classifiers we encountered in this section, namely K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines. We will utilize a dataset related to marketing bank products over the telephone.
</p>

## <h3>Repo Structure</h3>
* The compare_classifiers.ipynb file contains python code related to data analysis, visualization.
* The data folder has bank-additional-full.csv file that contains sample data used in this application.

## <h3>Business Objective</h3>
<p>
The objective of this project is to compare different classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) using the bank marketing dataset from the UCI Machine Learning Repository. The goal is to determine the most accurate and reliable model for predicting the success of a marketing campaign for a bank.

The dataset contains information about client attributes, campaign details, and outcome variables related to bank marketing campaigns. By evaluating the performance of different classifiers on this dataset, the objective is to assess their accuracy, precision, recall, and F1-score in predicting whether a client will subscribe to a term deposit or not.

The aim is to identify the classifier that performs best in terms of these metrics, which will provide valuable insights for the bank's marketing campaign.

Thank you UCI Machine Learning repository for allowing us to use your dataset https://archive.ics.uci.edu/dataset/222/bank+marketing.
</p>

## Key Highlights
*  Decision Tree model performs the best in terms of accuracy and training time (8 seconds).
*  Decision Tree model has the best accuracy, recall, and F1-Score metrics among all four models.
*  Logistic Regression model has the best precision and ROC-AUC Curve metrics among all four models.
*  SVM model (SVC classifier) has the highest training time (1000+ seconds) and is computationally expensive.
*  Bank Marketing dataset is impbalanced because distribution is not similar within dataset.
*  The highest positive correlation between numerical independent variables is between "emp.var.rate" and "euribor3m" with a value of 0.97.
*  The highest negative correlation between numerical independent variables is between "pdays" and "previous" with a value of -0.59.
*  Decision Tree model predicted the highest True Positives, while SVM (SVC Classifier) predicted the highest True Negatives, followed by the Logistic Regression model on the Test Data.
*  The "Day_of_Week" feature has a similar success rate among all categorical values, so it is not an important feature for the given model dataset.
*  The "nr.employed" & "euribor3m" are higher importance features since they have higher influence towards model predictions.
*  The "month", "cons.price.idx" and "duration" features have higher coefficient and they contribute higher towards predicting the target variable.
*   Overall, the **Decision Tree** model is the best performing model among all four models followed by **Logistic Regression** model.

## Next steps and Recommendations
Evaluate and identify non-important categorical features in a group (with other feature variable) rather than single to determine whether there exist combination of categorical features which can be disgarded.
*  Continue to add samples from new marketing campaign and evaluate the different classifier models.  
*  Imbalanced dataset: Since the bank marketing dataset is imbalanced, consider using techniques such as resampling, SMOTE, or cost-sensitive learning to address the class imbalance and improve model performance.
*  Feature importance: Focus on the "nr.employed", "euribor3m", "month", "cons.price.idx", and "duration" features, as they have higher coefficients or importance towards predicting the target variable. Consider further analyzing these features and their relationships with the target variable to gain deeper insights.
* Training time and computational expense: Given that the SVM model (SVC classifier) has the highest training time and is computationally expensive, consider optimizing the model or exploring alternative models that can provide similar performance with lower training time.
*  Performance metrics: While the Decision Tree model performs the best in terms of accuracy, recall, and F1-Score, and the Logistic Regression model has the best precision and ROC-AUC Curve metrics, it is important to consider the specific requirements of the problem at hand. Evaluate the trade-offs between different metrics and select the model that aligns best with the desired outcome.
*  Correlation analysis: Take note of the highest positive correlation between "emp.var.rate" and "euribor3m" and the highest negative correlation between "pdays" and "previous". These insights can help in understanding the relationships between variables and potentially identifying multicollinearity issues.  
* Overall, continue to refine and optimize the Decision Tree model and consider the recommendations mentioned above to further enhance model performance and interpretability.

[Compare_Classifiers_Report.docx](https://github.com/hardikszaveri/CompareClassifiers/blob/main/Compare_Classifiers_Report.docx)
