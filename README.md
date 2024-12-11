# Assignement

It is an assignement of Training a classifier to predict the class: 0 or 1.

in this Assignement we compare 3 differenet models 

__1-Random Forest Classifier:__

Random Decision Forest is a supervised Machine learning algorithm used for classification, regression, and other tasks using decision trees.

__2-K-Nearest Neighbor:__

The K-Nearest Neighbors (KNN) algorithm is a supervised machine learning method employed to tackle classification and regression problem

__3-Logistic Regression:__

Logistic regression is a supervised machine learning algorithm widely used for binary classification tasks.


__Using F1 score as evaluation metric:__

F1 score is a measure of the harmonic mean of precision and recall. Commonly used as an evaluation metric in binary and multi-class classification and LLM evaluation, the F1 score integrates precision and recall into a single metric to gain a better understanding of model performance.  

## Data Pre-Processing

### Showing the first five rows of our data

![image](https://github.com/user-attachments/assets/00022713-5055-4c59-b609-5cdeb15de078)

### Checking the presence of Missing Values

![image](https://github.com/user-attachments/assets/7b290390-29c8-4a09-9b72-ee2e3aefd51d)

### Generates descriptive statistics that summarize the central tendency, dispersion and shape of our dataset distribution, excluding NaN values:

![image](https://github.com/user-attachments/assets/7ef5f7a6-4729-4b77-bd67-fb8974b72578)

### Defining input Varibles-Features

![image](https://github.com/user-attachments/assets/6b573ceb-3f96-4ca3-aa32-466a724a1dcc)

### Defining Target Variable (Class)

![image](https://github.com/user-attachments/assets/b86a2255-2a8a-443c-b717-151de693e102)

### Split the data into training and test dataset

![image](https://github.com/user-attachments/assets/a16a0b77-6379-4543-a58e-4474d233599a)

### Impute Missing Values

![image](https://github.com/user-attachments/assets/a5132b1e-e004-40a3-9487-4ba89b273cca)

__Imputation Strategy:__ We're using the median of each column in the training data, which is often a good strategy for numerical features when there are missing values (especially if the data is skewed).

__Data Leakage Prevention:__ The median is calculated only on the training data, which avoids the issue of data leakage from the test set.

### Scaling the Data

![image](https://github.com/user-attachments/assets/a66247ff-4493-493b-acdf-e808fab97942)

__StandardScaler:__ This scaler standardizes the data by removing the mean and scaling to unit variance.

__Fit and Transform:__
fit_transform(X_train): This fits the scaler on the training set and transforms it (scaling).
transform(X_test): After fitting on the training data, you apply the same scaling transformation to the test set, ensuring consistency between train and test data.

## Training The Model:

![image](https://github.com/user-attachments/assets/78a530aa-e950-425f-98a7-80e9c90256e2)

![image](https://github.com/user-attachments/assets/c6b0c835-2b67-4994-afc9-1de834a174c6)

![image](https://github.com/user-attachments/assets/8a698e02-ddae-4a93-ae08-784d97676a07)


### Prediction 


__Random Forest Classifier__

![image](https://github.com/user-attachments/assets/b00d7d6e-df23-4519-ba16-34913345032f)

__Logistic Regression Model__

![image](https://github.com/user-attachments/assets/611e6429-ad82-44ff-9fab-057c9be1fbd6)

__K-Nearest Neighbors__

![image](https://github.com/user-attachments/assets/4d6bd0d7-d851-4c33-8fc9-b0209ca91d2f)

## Results

the comparison between the 3 models have shown the best performance related to Random Forest Classifier with F1-scoere=0.96
and then we get F1-score=0.93 when using Logisitic Regression Model.The pporest Performance among the Three models was K-Neares Neighbors with F1-score=0.83


    
