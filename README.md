# Credit Card Approval Prediction with Supervised Machine Learning Models



## 1. Credit Card Approval Dataset Description: 

- Credit Card Approval Prediction: Used machine learning to determine the features that affect the approval of customer credit card!. This dataset is available from the UCI machine learning repository, https://archive.ics.uci.edu/ml/datasets/credit+approval
- This data file concerns credit card applications. All attribute names and values have been changed to meaningless symbols to protect confidentiality of the data. 
- This dataset is interesting because there is a good mix of attributes -- continuous, nominal with small numbers of values, and nominal with larger numbers of values. There are also a few missing values. 


## 2. Overview of Data: 

- The dataset of credit approval contains 690 rows and 16 columns. The following are the variables in the dataset namely 'Gender', 'Age', 'Debt', 'Married', 'BankCustomer', 'EducationLevel', 'Ethnicity', 'YearsEmployed', 'PriorDefault', 'Employed', 'CreditScore', 'DriversLicense', 'Citizen', 'ZipCode', 'Income', 'Approved'
- **Input variables - “features” :** They are based on information of the applicant namely 'Gender', 'Age', 'Debt', 'Married', 'BankCustomer', 'EducationLevel', 'Ethnicity', 'YearsEmployed', 'PriorDefault', 'Employed', 'CreditScore', 'DriversLicense', 'Citizen', 'ZipCode', 'Income'
- **Output variables - “target” :** The variable here is approval status whether applicant's request was approved or denied approved (0 and 1)

## 3. Part I: Data Preprocessing 

*Summary:*

- All the relevant libraries for the project were imported and the data was read into the file
- A basic exploratory data analysis reveals the summary of the data along with the data types and the descriptive statistics
- The dataset was throroughly explored for missing values and they were eliminated using mean, frequency and other relevant imputation methods 
- Used Label encoders for converting some of the data labels in the various variables to numeric form in order for the machine learning models to be applied.
- Obtained Correlation Heat Map to understand correlation of variables and also to extract some important features.
- **Label Encoding in Approval "target" variable:** Approved as "1", Denied as "0" 

## 4. Part II: Machine Learning

*Models:*

(A). LOGISTIC REGRESSION

(B). DECISION TREES

(C). RANDOM FORESTS

(D). SVM

(E). STOCHASTIC GRADIENT DESCENT

(F). KNN

*Top 2 Models for dataset:*

**1. Logistic Regression**
   - Hyperparameters were tuned, and these are the parameters used in the model are Kernel = ‘poly’, Degree = 3, Gamma = 'auto'
   - Accuracy was 86% for this model

   
**2. Random Forest**
   - Hyperparameters were tuned, and these are the parameters used in the model are criterion = ‘entropy’, max_depth = None, 
   min_samples_split = 3
   - Accuracy was 85% for this model

*Variable Importance Plot indicates that **Prior Default** is the most important variable*

## 5. Conclusions:
 
- The credit card approval data was analyzed for quality 
- It was found that approval status of the applicant is mostly correlated to priordefault
- Data was split into training and test set. Machine learning models were trained in training set and tested for accuracy on the test   set.
- Logistic Regression model does the best with an accuracy of 86%
- Machine learning also conclude that “PriorDefault” is the most important variable that determines the approval of credit card

## 6. Future Scope:

- ML models accuracy is not high. A larger datset with more information on the applicants will aid better prediction.
- Lack of information about how the dataset was created may impact the prediction of approval status using only the generalized applicant data as predictors. 