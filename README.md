# AWS Machine Learning Specialty Certification
# Fundamentals of Machine Learning on AWS
### Overview
* Artificial Intelligence != Machine Learning != Deep Learning
* Machine Learning - Learning from Data is = Identifying Patterns. Machine Learning Identifies Patterns in the existing data to make predications about new data.
* Deep Learning - Subset of ML.
![image](https://user-images.githubusercontent.com/13011167/103115848-254a7580-468a-11eb-8ede-04f5aefc56e3.png)

#### When to use the Machine Learning?
* When its too difficult to code logic the "old fashioned way"using if-else statements. E.g Analyze Sentiments on the social Media data or websites.
* When its not cost effective to do it manually.
* When there is ample training data available.
* When Business problem can be stated as the ML Problem.

#### When not to use Machine Learning?
* When don't have the enough data available. E.g If we trying to predict sales for the new product.
* When Data can't be labelled.  Is the histrotical data fraud or not, will particular customer churn or not. We need to make the sense of data.
* When we need to launch quickly.
* When there is no room for error. For mission critical applications that cannot tolerate errors, ML can't be applied. 

### Defining Machine Learning Problems (Different types of problems)
![image](https://user-images.githubusercontent.com/13011167/103083778-45832180-4603-11eb-89a4-2c87cbd5a01e.png)

### How to define the Machine Learning Problems
###  Example - Customer's Churn Problem (What Questions to ask)
#### 1. Whats the current pain point?
* Customer Churn rate last year was 14.5%.
* We have no way to predict who will leave so that we can incentivize then to stay.
#### 2. How are we currently solving this problem?
* If a customer gets angry during the service call and threatens to leave, a customer agent can offer them the incentive.
#### 3. What data do we have?
#### 4. Is the data Labelled?
#### 5. How will we define success?
* Customer Churn rate to be dropped to 4%.
* Customer retension incentives not to exceed $750,000.
#### 6. What are the trade-offs?
* Some Customers will be given incentives even if they are not Churn risks.
* Some Customers given the incentives will leave anyway.
#### 7. What is out of scope?
* Deactivaiton or downgrade of the service or features.
* Sales Experience and performance of the Customer service agents.

# AWS SAGEMAKER 
* Getting data into Sagemaker. 
![image](https://user-images.githubusercontent.com/13011167/103111676-a8ad9c00-4675-11eb-85c1-dc2ebe460f5b.png)

### FETCH, CLEAN and PREPARE DATA
#### FETCHING
* Two type of Data Ingestion Techniques - Batch Processing or Stream Processing.
* Batch Processing - Prediocally collect and send Data. Used when there is no need for real time processing. 
* AWS Services used for Batch Processing:
![image](https://user-images.githubusercontent.com/13011167/103111758-5f118100-4676-11eb-95fb-539c14e74398.png)
* Stream Processing - Real Time Processing. Data is loaded and maniplated as it is recognized. Used when real-time data is required (e.g Stock Prices). More Expensive.
* AWS Services used for Stream Processing (AWS Kinesis):
![image](https://user-images.githubusercontent.com/13011167/103114014-1a401700-4683-11eb-8343-5b4f3214e0fa.png)

#### CLEANING
* Data is Messay. Taking care of Missing Data, Inconsistent Data values( Male, M), Inconsistant Abbreviations, Duplicates etc.
#### DATA VISUALIZATION AND ANALYSIS
* Analysize descriptive Statistics of Data. Mean, SD, correlation and Outliers etc. 
* USe Scatter Plots, Correlation Matrix, Histrogram and Box Plots. 
#### FEATURE ENGINEERING
* Goals is to increae the predictive power of the data. 
* Dimentional Reduction - Which features are not related and can be Dropped.
* Handling Scales (Inches, Meters etc). Age can be in Years and months.
* Converting Categorical Values to Binary. Categorical Data can be of two type - Norminal Data (Oder does not matter) and Ordinal Data (Order Does matter). Norminal e.g Yes, No, Red Blue Yellow. Ordinal- Small, Medium, Large or Hot, Hotter and Hottest. 
* ONE-HOT ENCODING (Ordinal Data - Generally not recomanded the encode numerical Value). Solution is ONE-HOT-ENCODING.
![image](https://user-images.githubusercontent.com/13011167/103112229-047a2400-467a-11eb-8218-2e378f59c41f.png)

### TRAINING AND EVALUATING THE MODEL
* Train the models using different algorithms and evauate it using Hyperparameter tuning.
* Goal of ML is to generalize he model. Taking care of Overfitting or Underfitting. 
* Tuning the Model:
![image](https://user-images.githubusercontent.com/13011167/103115898-54f97d80-468a-11eb-9197-2cdae7113f86.png)

* Confusion Matrix for the following predictioned values.
![image](https://user-images.githubusercontent.com/13011167/103114735-e2869e80-4685-11eb-8fb2-f663a2f30db0.png)
![image](https://user-images.githubusercontent.com/13011167/103121032-59309580-46a0-11eb-9c5e-61f2cde12310.png)

* Metrics for Classification Problems:
![image](https://user-images.githubusercontent.com/13011167/103114603-54aab380-4685-11eb-8ec5-ad794e6a64f1.png)

### DEPLOY AND MONITORING MODELS
* Deploying the model - Need to take care of security and best practices and Monitoring the Model - CloudWatch(Performance Metrix) and CloudTrail (Auditing API Activity), Sagemaker Model Monitor
* IAM Role based Access for Amazon Sagemaker for security.

# AWS MACHINE LEARNING STACK
![image](https://user-images.githubusercontent.com/13011167/103115779-ee745f80-4689-11eb-907f-a12c33cd5202.png)

# DATA ENGINEERING WITH AWS MACHINE LEARNING


###Important Links
* Amazon SageMaker Examples: git clone https://github.com/awslabs/amazon-sagemaker-examples.git
* SageMaker Developer Guide (Important)
* SageMaker Blog 
* Amazon ReInvent - SageMaker.




