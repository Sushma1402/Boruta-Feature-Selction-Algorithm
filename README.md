# Boruta-Feature-Selction-Algorithm
#- Problem Statement : In this project we will build Boruta algorithm to recognize which are important independent features for the model building. #- Boruta is a Feature Selection technique. With this technique we can categorize the independent features into 3 categories, which are:

Confirmed
Tentative
Rejected Boruta categorizes a certain feature into "Confirmed" if the independent feature is important for the prediction of the output. If a certain feature is not importent for the model building, then Boruta categorizes the certain feature into "Rejected" and if the Boruta is not sure wheather a certain feature is important or not, then it categorizes the feature as "Tentative".
#- Credit loan approval prediction: We have a dataset of credit loan approval. We have 11 dependent features in this dataset, such as: 'Gender' : Male or Female (Categorical data type) 'Married' : Yes or No (Categorical data type) 'Dependents': Number of dependent persons on the applicant (Integer data type) 'Education': Education of the applicant. "Graduate" or "not Graduate" 'Self_Employed': Yes or No(Categorical data type) 'ApplicantIncome': Income of the applicant(Float Type) 'CoapplicantIncome': Income of co-applicant(Float type) 'LoanAmount': Required Loan Amount (Float data type) 'Loan_Amount_Term': Tenure of the loan (Float data type) 'Credit_History': 1 or 0 ( Good or Bad,Categorical data type) 'Property_Area': Urban ir Rural (Categorical data type) 'Loan_Status': Yes or No, loan approved por not (Categorical data type)

#- From a technical point of view, the main aspects of python covered throughout the notebook are:

data manipulation: pandas, numpy, modeling: Boruta class definition: Random Forest Classifier

#-Exploratory Data Analysis We have performed EDA by dropping the rows which have missing values. Then we have converted the categorical data into numeric form. The input of Boruta Must be an Array, hence we have converted the data frame into array.

#- Model Building After EDA, we have built Boruta on Random Forest Classifier with maximum iterations of 25. #- Output: The Boruta has indicated that there are 2 confirmed important features and 9 not importanrt features. "Credit_History" and "ApplicantIncome" these are the three important features. Rest of the features, such as "Gender", are least important. With this observation we can say that there is no Gender Bias followed for loan approval.
