# Explore visual tools for machine learning

## Use Automated Machine Learning in Azure Machine Learning
1. An automobile dealership wants to use historic car sales data to train a machine learning model. The model should predict the price of a pre-owned car based on its make, model, engine size, and mileage. What kind of machine learning model should the dealership use automated machine learning to create?
- [ ] Classification
- [ ] Regression
- [ ] Time series forecasting
 
<details>
  <summary>Check your answer</summary>

- [ ] Classification
- [x] Regression: Correct. To predict a numeric value, use a regression model.
- [ ] Time series forecasting 
</details>

2. A bank wants to use historic loan repayment records to categorize loan applications as low-risk or high-risk based on characteristics like the loan amount, the income of the borrower, and the loan period. What kind of machine learning model should the bank use automated machine learning to create?
- [ ] Classification
- [ ] Regression
- [ ] Time series forecasting

<details>
  <summary>Check your answer</summary>

- [x] Classification: Correct. To predict a category, or class, use a classification model.
- [ ] Regression
- [ ] Time series forecasting
</details>

3. You want to use automated machine learning to train a regression model with the best possible R2 score. How should you configure the automated machine learning experiment?
- [ ] Set the Primary metric to R2 score
- [ ] Block all algorithms other than GradientBoosting
- [ ] Enable featurization

<details>
  <summary>Check your answer</summary>

- [ ] Set the Primary metric to R2 score: Correct. The primary metric determines the metric used to evaluate the best performing model.
- [ ] Block all algorithms other than GradientBoosting
- [ ] Enable featurization
</details>

4. What is machine learning?
- [ ] An automated test tool that can be used in CI/CD pipelines to ensure quality before a software release.
- [ ] A technique that uses mathematics and statistics to create a model that can predict unknown values.
- [ ] A monitoring service that provides visibility f your security posture across all of you services, both on Azure and on-premise.

<details>
  <summary>Check your answer</summary>

- [ ] Azure Test Plans is an automated test tool that can be used in CI/CD pipelines to ensure quality before a software release.
- [X] Machine learning is a technique that uses mathematics and statistics to create a model that can predict unknown values.
- [ ] Azure Security Center is a monitoring service that provides visibility f your security posture across all of you services, both on Azure and on-premise.
</details>

5. You can define machine learning using a mathematical term as f(x) = y. What does each part of the term represent?
- [ ] _f_ is a function definition that operates on one or more features of something (which we'll call _x_) to calculate a predicted label (_y_)
- [ ] _y_ is a function definition that operates on one or more features of something (which we'll call _f_) to calculate a predicted label (_x_)
- [ ] _x_ is a function definition that operates on one or more features of something (which we'll call _y_) to calculate a predicted label (_f_)

<details>
  <summary>Check your answer</summary>

- [x] _f_ is a function definition that operates on one or more features of something (which we'll call _x_) to calculate a predicted label (_y_)
- [ ] _y_ is a function definition that operates on one or more features of something (which we'll call _f_) to calculate a predicted label (_x_)
- [ ] _x_ is a function definition that operates on one or more features of something (which we'll call _y_) to calculate a predicted label (_f_)
</details>

6. There are two general approaches to machine learning. These are ...... and ...... .
- [ ] regression and clustering
- [ ] supervised and unsupervised machine learning
- [ ] classification and clustering

<details>
  <summary>Check your answer</summary>

- [ ] regression and clustering
- [x] supervised and unsupervised machine learning
- [ ] classification and clustering
</details>

7. The ...... machine learning approach starts with a dataset without known label values.
- [ ] unsupervised
- [ ] supervised
- [ ] regression

<details>
  <summary>Check your answer</summary>

- [x] unsupervised
- [ ] supervised
- [ ] regression 
</details>

8. The ...... machine learning approach requires you to start with a dataset with known label values.
- [ ] unsupervised
- [ ] supervised
- [ ] regression

<details>
  <summary>Check your answer</summary>

- [ ] unsupervised
- [x] supervised
- [ ] regression 
</details>

9. The unsupervised machine learning task ...... is used to determine labels by grouping similar information into label groups; like grouping measurements from birds into species.
- [ ] Regression
- [ ] Clustering
- [ ] Classification

<details>
  <summary>Check your answer</summary>

- [ ] Regression
- [x] Clustering
- [ ] Classification
</details>

10. Two types of supervised machine learning tasks include ...... and ...... .
- [ ] Regression
- [ ] Clustering
- [ ] Classification

<details>
  <summary>Check your answer</summary>

- [x] Regression: used to predict a continuous value; like a price, a sales total, or some other measure.
- [ ] Clustering: used to determine labels by grouping similar information into label groups; like grouping measurements from birds into species.
- [x] Classification: used to determine a binary class label; like whether a patient has diabetes or not.
</details>

## Create a regression model with Azure Machine Learning designer

11. In Azure Machine Learning studio, what can you use to author regression machine learning pipelines using a drag-and-drop interface?
- [ ] Notebooks
- [ ] Automated machine learning
- [ ] Designer

<details>
  <summary>Check your answer</summary>

- [ ] Notebooks: Incorrect. You can use Notebooks to author machine learning projects with code.
- [ ] Automated machine learning: Incorrect. You can use AutoML to author regression pipelines with a click-through wizard.
- [x] Designer: Correct. You can use Designer to author regression pipelines with a drag-and-drop interface.
</details>

12. You are creating a training pipeline for a regression model. You use a dataset that has multiple numeric columns in which the values are on different scales. You want to transform the numeric columns so that the values are all on a similar scale. You also want the transformation to scale relative to the minimum and maximum values in each column. Which module should you add to the pipeline?
- [ ] Select Columns in a Dataset
- [ ] Clean Missing Data
- [ ] Normalize Data

<details>
  <summary>Check your answer</summary>

- [ ] Select Columns in a Dataset
- [ ] Clean Missing Data
- [x] Normalize Data Correct. When you transform numeric data to be on a similar scale, use a Normalize Data module.
</details>

13. Why do you split data into training and validation sets?
- [ ] Data is split into two sets in order to create two models, one model with the training set and a different model with the validation set.
- [ ] Splitting data into two sets enables you to compare the labels that the model predicts with the actual known labels in the original dataset.
- [ ] Only split data when you use the Azure Machine Learning Designer, not in other machine learning scenarios.

<details>
  <summary>Check your answer</summary>

- [ ] Data is split into two sets in order to create two models, one model with the training set and a different model with the validation set.
  - Incorrect. The validation set is used to test the model created with the training set.
- [x] Splitting data into two sets enables you to compare the labels that the model predicts with the actual known labels in the original dataset.
  - Correct. You want to test the model created with training data on validation data to see how well the model performs with data it was not trained on.
- [ ] Only split data when you use the Azure Machine Learning Designer, not in other machine learning scenarios. 
  - Incorrect. Splitting data into training and validation sets is an important part of all machine learning scenarios.
</details>

## Create a clustering model with Azure Machine Learning designer

14. You are using an Azure Machine Learning designer pipeline to train and test a K-Means clustering model. You want your model to assign items to one of three clusters. Which configuration property of the K-Means Clustering module should you set to accomplish this?
- [ ] Set Number of Centroids to 3
- [ ] Set Random number seed to 3
- [ ] Set Iterations to 3

<details>
  <summary>Check your answer</summary>

- [x] Set Number of Centroids to 3: That is correct. To create K clusters, you must set the number of centroids to K
- [ ] Set Random number seed to 3
- [ ] Set Iterations to 3
</details>

15. You use Azure Machine Learning designer to create a training pipeline for a clustering model. Now you want to use the model in an inference pipeline. Which module should you use to infer cluster predictions from the model?
- [ ] Score Model
- [ ] Assign Data to Clusters
- [ ] Train Clustering Model

<details>
  <summary>Check your answer</summary>

- [ ] Score Model
- [x] Assign Data to Clusters: That is correct. use the Assign Data to Clusters module to generate cluster predictions from a trained clustering model
- [ ] Train Clustering Model
</details>

## Create a classification model with Azure Machine Learning designer

16. You're using Azure Machine Learning designer to create a training pipeline for a binary classification model. You've added a dataset containing features and labels, a Two-Class Decision Forest module, and a Train Model module. You plan to use Score Model and Evaluate Model modules to test the trained model with a subset of the dataset that wasn't used for training. What's another module should you add?
- [ ] Join Data
- [ ] Split Data
- [ ] Select Columns in Dataset

<details>
  <summary>Check your answer</summary>

- [ ] Join Data
- [x] Split Data: Correct. Use a Split Data module to randomly split a dataset into training and validation subsets.
- [ ] Select Columns in Dataset
</details>

17. You use an Azure Machine Learning designer pipeline to train and test a binary classification model. You review the model's performance metrics in an Evaluate Model module, and note that it has an AUC score of 0.3. What can you conclude about the model?
- [ ] The model can explain 30% of the variance between true and predicted labels.
- [ ] The model predicts accurately for 70% of test cases.
- [ ] The model performs worse than random guessing.

<details>
  <summary>Check your answer</summary>

- [ ] The model can explain 30% of the variance between true and predicted labels.
- [ ] The model predicts accurately for 70% of test cases.
- [x] The model performs worse than random guessing. - Correct. An AUC of 0.5 is what you'd expect with random prediction of a binary model.
</details>

18. You use Azure Machine Learning designer to create a training pipeline for a classification model. What must you do before deploying the model as a service?
- [ ] Create an inference pipeline from the training pipeline
- [ ] Add an Evaluate Model module to the training pipeline
- [ ] Clone the training pipeline with a different name

<details>
  <summary>Check your answer</summary>

- [x] Create an inference pipeline from the training pipeline - Correct. You must create an inference pipeline to deploy as a service.
- [ ] Add an Evaluate Model module to the training pipeline
- [ ] Clone the training pipeline with a different name
</details>