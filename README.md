# ⚕️ Heart Disease Classification
## Project Overview
* Created a tool that predicts (with an accuracy ~ 84.46%) if someone has heart disease to help medical professionals diagnose potential dangers based on a patient's clinical parameters.
* Trained models on a sample of 242 patient records and tested them on a testing set of 61 records.
* Experimented with LogisticRegression, KNeighborsClassifier and RandomForestClassifier. Based on baseline models, optimizations were done for LogisticRegression and RandomForestClassifier using RandomizedSearchCV and GridSearchCV in order to reach the best model.
## Code and Resources Used
* **Python Version**: 3.8.8
* **Packages**: pandas, numpy, sklearn, matplotlib, seaborn
* **Data Source**: https://archive.ics.uci.edu/ml/datasets/heart+Disease
## EDA
I looked at the relationships between certain features found in our data. Below are a few highlights from the analysis made.

![download](https://user-images.githubusercontent.com/79250297/187205473-dfd0ab87-01ee-438e-a4d7-e16c2a1b7fec.png)
![download](https://user-images.githubusercontent.com/79250297/187205571-80406248-3512-4163-99dc-d113208cfe2c.png)
![download](https://user-images.githubusercontent.com/79250297/187205592-8e0acbda-af37-4630-8527-f2824001d5df.png)
## Model Building
I split the data into train and tests sets with a test size of 20%.

I tried three different models and evaluated them using accuracy. I chose accuracy because it is relatively easy to interpret and shows how many prediction our models got right. 

* **Logistic Regression**
* **K Neighbors Classifier**
* **Random Forest Classifier**

## Model Performance
The Logistic Regression model far outperformed the K Neighbors Classifier and slightly outperformed the Random Forest Classifier

* Logistic Regression: 0.885%
* K Neighbors Classifier: 0.688%
* Random Forest Classifier: 0.836%

![download](https://user-images.githubusercontent.com/79250297/187207300-9fcf74b8-a06a-4d02-9655-ae10bd223087.png)

After hyperparameters tuning and cross validation, Logistic Regression had an accuracy of 0.844%. Other metrics are shown below.

![download](https://user-images.githubusercontent.com/79250297/187207798-8cd63454-48fd-43dd-9533-99177fb742e2.png)
