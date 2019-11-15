# LoadData by Prosper
## by Abdullah Mustafa


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, 
borrower rate (or interest rate), current loan status, borrower income, and many others.
To ease the analysis process, only 11 variables were chosen. The data was overall clean; 
however, wrangling was conducted to remove outliers and outstanding peaks as well as filling in 
the missing values.
The data is obtained through this URL: https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv.
A brief description of the variables can be found here: https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0


## Summary of Findings

> As for the 'LoanStatus' feature, it was possible to compare the loan completion ratio 
for different features and the following relations were found: 

1. Term: Shorter loan terms (12) have higher completion rations than longer ones (60).
2. IncomeRange: Those with higher income are more likely to complete their loan payment.
3. EmploymentStatus: Employed persons are more capable of completing their loan than unemployed ones.
4. IsBorrowerHomeowner: Owning a home gives a slightly higher probablity of completing the loan.
5. BorrowerAPR: Loans with lower APR are more likely to be completed.
6. BorrowerRate: Loans with lower interest rate are more likely to be completed.
7. AvailableBankcardcredit: The larger the credit, the higher the completion rate.
8. StatedMonthlyIncome: Overall, we can suggest that higher monthly income suggests higher completion ratios.
9. LoanOriginalAmount: The larger the loan, the lower the completion ratio.
10. MonthlyLoanPayment: Lower monthly loan payments have higher completion ratios.

> A strong corrolation between the "BorrowerAPR" and the "BorrowerRate" was found.

> The "BorrowerAPR" was found to have dependance on other features as follows:

1. LoanStatus: Incompleted loans have higher APRs.
2. Term: Short term periods have higher APRs
3. IncomeRange: Higher incomes have lower APRs
4. EmploymentStatus: Employed status has a lower APR
5. IsBorrowerHomeowner: Home owners get lower APRs.
6. AvaliableBankcardcredit: Low credit has a higher APR.
7. LoanOriginalAmount: Lower loans have higher APRs.
8. MonthlyLoanPayment: Lower payments have higher APRs.
9. StatedMonthlyIncome: The relation isn't clear.

> The dependancy of MonthlyLoanPayment on the "LoanOriginalAmount" is found to be strong and
is influnced by the Term periond as well as the BorrowerAPR.

> Higher incomerange increase the chances of getting larger loans at lower APRs.

## Key Insights for Presentation

> The presentation summarized all of the previously-stated findings except for the APR and the interest rate relation.
The visualiztions used are
1. barplots for the LoanStatus dependance
2. point plots and heatmaps for the BorrowerAPR relations
3. heatmap and faceted scatter plot for the monthly payment and loan amount relation.
4. point plots for the incomerange relations.