# Loan Approval Prediction

# Predicting Approval of the loan using machine learning
![Loan Defaults Picture](https://github.com/KelvinJulius/loan-approval-prediction/assets/108222785/4de788ae-76df-450e-8675-9af21c6b076e)

This notebook using python for machine learning and data science in attempt to predict the approval of the loan based on the attributes.

We're going to take the following approach:
1. Problem definition
2. Data
3. Evaluation
4. Features
5. Modelling
6. Experimentation


## 1. Problem definition
We assume as a loan officer who is deciding whether to approve a loan to a small business. In this case, we predict the approval (**Approved** or **not approved**) based on the attributes.

## 2. Data
This dataset can be looked at this link: https://www.kaggle.com/datasets/mirbektoktogaraev/should-this-loan-be-approved-or-denied

## 3. Evaluation

Evaluation metrics are:
* Accuracy (90%)
* ROC curve and AUC score
* Confusion matrix
* Precision
* Recall
* Classification report
* F1-score
* Cross-validation

## 4. Features

Information about the description of features

**Create data dictionary:**
* LoanNr_ChkDgt = Identifier Primary key
* Name = Borrower name
* City = Borrower city
* State = Borrower state
* Zip	= Borrower zip code
* Bank = Bank name
* BankState = Bank state
* NAICS = North American industry classification system code
* ApprovalDate = Date SBA commitment issued
* ApprovalFY = Fiscal year of commitment
* Term = Loan term in months
* NoEmp = Number of business employees
* NewExist  -  1 = Existing business (0) , 2 = New business (1)
* CreateJob = Number of jobs created
* RetainedJob	= Number of jobs retained
* FranchiseCode =Franchise code, (00000 or 00001) = No * franchise
* UrbanRural - 1 = Urban, 2 = rural, 0 = undefined
* RevLineCr = Revolving line of credit: Y = Yes, N = No
* LowDoc = LowDoc Loan Program: Y = Yes, N = No
* ChgOffDate = The date when a loan is declared to be in * default
* DisbursementDate = Disbursement date
* DisbursementGross = Amount disbursed
* BalanceGross = Gross amount outstanding
* MIS_Status - Loan status charged off = CHGOFF (1) , Paid in full = PIF (0) (Target)
* ChgOffPrinGr = Charged-off amount
* GrAppv = Gross amount of loan approved by bank
* SBA_Appv = SBA’s guaranteed amount of approved loan


## Preparing the tools
We're going to use pandas, Matplotlib , seaborn, and NumPy for data analysis and manipulation. We're using scikit-learn for machine learning
