Loan Status Prediction:
Predicting loan status using a neural network model.

Overview
This project aims to predict loan status based on various attributes using a neural network model. The dataset used for training and testing the model contains information such as gender, 
marital status, education, loan amount, loan term, credit history, and property area, among others.

Dataset
The dataset used in this project is stored in a CSV file named loan_data.csv. It contains the following columns:

Gender
Married
Dependents
Education
Self_Employed
ApplicantIncome
CoapplicantIncome
LoanAmount
Loan_Amount_Term
Credit_History
Property_Area
Loan_Status
Preprocessing

Missing values in the dataset were handled using mode imputation.
Categorical variables were converted to numerical using label encoding.
Attributes with low correlation with the target variable were removed.

Model
A neural network model was implemented using TensorFlow's Keras API. The model architecture consists of three dense layers with relu activation for hidden layers and sigmoid activation for 
the output layer since it is a binary classification problem.

Training
The dataset was split into training and testing sets using a 70-30 split.
Min-max scaling was applied to normalize the features.
Early stopping was used to prevent overfitting during training.

Results
The model achieved a f1 score of .90. Unforunately, it was no amazing at predicting who would not recieive a loan, but was perfectin predicting who would recieve a loan.

Additionally, the loss went from loss 0.7336 to 0.4123 to and the validation loss went from 0.7424 to 0.3773.
