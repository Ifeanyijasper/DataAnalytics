# Loan Form Prosper Data Exploration

## By Okonkwo Ifeanyichukwu

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, 
borrower rate (or interest rate), current loan status, borrower income, and many others. After examining 
the data and perform some data cleaning. The dataset was reduced to 113912 loans with 14 varibable. 
The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv),
with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
BorrowerRate and BorrowerAPR. In similar way there is relationship between 
LoanOriginalAmount and MonthlyLoanPayment. I also discovered that BorrowerRate 
and BorrowerAPR are values are highly close for loans that last 60 means 
compare to the loans that last 36 months. Findings from loans amounts show 
that originalLoanAmount above 7000 dollar has high rate to stay pass the 
payment due day. As expected, majority self-employed workers do not have a 
verifiable income. Also I discovered that IncomeVerifiable has impact 
loanOriginalAmount. The BorrowerRate and BorrowerAPR a high range of value when 
the loan Term is 36 month and lower range of values when the Term is 60 months.


Outside of the main variables of interest, I verified the relationship between
LoanOriginalAmount and MonthlyLoanPayment.Also look into how loan it taken by 
borrowers based on their Monthly income. IncomeVerifaible and EmploymentStatus
also play a role on verifying how likely loan is given out based on their 
employmentStatus. I was able to find relationship between StatedMonthlyIncome
and LoanOriginalAmount this is to find out if Borrower consider their MonthlyIncome
to decied the amount of Loan to take or if the Loan is given out based on 
StatedMonthlyIncome to determine if likely LoanStatus will be completed before 
due days.

## Key Insights for Presentation

For the presentation, I focus on each variable on the dataset to discover how 
they perform or varies on their own without other variable influence After that
I added the other key varible to the plot such as the LoanOriginalAmount on
the LoanStatus, IncomeVerifiable on LoanStatus and then compare all numeric varible
in pairgrid. I also compare BorrowerRate and BorrowerAPR. I also bring in 
LoanStatus into BorrowerRate and BorrowerAPR and verify how varies with addition 
of extra variable like EmploymentStatus.

I use barplot to introduce each of the categorical variables with numerical 
variable. To start,I use the bar plots of LoanStatus and BorrowerRate across 
EmploymentStatus and perform similar action with BorrowerAPR. I also look at
relationship between StatedMonthlyIncome and LoanStatusIncome using scatter plot.
Investigation of influence of IncomeVerifiable on other categorical variables.
