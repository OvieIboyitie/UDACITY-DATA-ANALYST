# Prosper Loan Data - What Loans should be Approved or Declined
## by Ovie Iboyitie


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

## Summary of Findings

Of 113,937 loan listings, 49.65% are current, 33.42% of the loans are completed, 10.53% and 4.40% are chargedoff and defaulted respectively with 1.81% percent past due with less than 0.2% accounting for Cancelled and Final Payment in progress listings. Giving out loans could be for a lot of different reasons - improving the socioeconomic life of the borrower, saving the life of the borrower, imporiving the economy of a state  by funding business and investments, but sometimes, or rather most of the times, its to make profit and/or a combo of making profits and other reasons. 

*The objective of this analysis is to identify and understand patterns responsible for Defaulted, Chargedoff, and past due loans and to improve the percentage of completed loans. To make data driven decisions on whether a loan should be approved.* 

A loan listing could either be a 12-month loans, or a 36-month or 60-month loan. 77.04% of the loan listings have a term of 36 months, with 60-months and 12-months loans accounting for 21.54% and 1.42% of the loan listings.

each loan listing has a corresponding listing category, which gives an idea about "What is the loan for". The data had 21 listing categories, but the top 11 most occured categores which accounts for 96.33% of the loan listings. A whooping 51.18% of the loans are for Debt consolidation. The top 11 categories are 

- Debt Consolidation
- Not Available
- Other
- Home Improvement    
- Business              
- Auto                   
- Personal Loan          
- Household Expenses     
- Medical/Dental         
- Taxes                 
- Large Purchases   

37.75% of the borrowers are from California(13.57%), Texas, New york, Florida and Illinois. These are the top 5(out of 51) states with the highest loan listings. 

60.28% of the Borrowers are Employed. This is followed by Full-time (23.6%), self-employed, Not available and Other. Partime, Not Employed and Retired only account for about 2.5% of the loans lsitings


The Original Loan amounts are majorly multiple of 5000s ranging from 5000 - 35000, But 95% of the original loan amount are less than or equal to 20,000.  The stated monthly income has an outlier, 1750000 and 99.5% of the stated monthly income are less than or equal to 25000, which is 10000 less the maximum Original loan amount. 
95% of the Monthly loan payments are less than or equal to 634.91, which is more than triple the mode and median of the monthly loan payments. The 95th percentile of monthly loan payments is greater than 1/36 of the 95th percentile of the Original loan amount. *This implies, that a 25000 loan would be completed in less than or 36 months if a borrower makes a monthly payment greater than or equal to 556 which is less than the 92nd percentile of the monthly loan paymets.*

The distribution of the DebtToIncomeRatio is skewed to the right. 99% of the borrowers have a DebtToIncomeRatio less than 0.86 with only 5% of the borrowers having a DebtToIncomeRatio less than 0.06. 

Inline with the objective of the analysis - identifying and understanding patterns responsible for Defaulted, Chargedoff, and past due loans and to improve the percentage of completed loans in To make data driven decisions on whether a loan should be approved,  loans that are Current, Cancelled, and  FinalPaymentInProgress were exluded or filtered out. 

1 year loans are good for business, but they only account for 1.42% of the loan listing. They have a whooping 94% completion rate. The Chargedoff 1 year loans have low stated monthly income. Only 66.8% of the 3 year loans were completed. Not high enough. 21.2% and 9.4% of the 3 year loans were Chargedoff and defaulted respectively. Now that's bad for business. but it doesn't just end there. 5 year loans are just as bad or worse. With a completion rate of only 55.3%. 24.8% and 15.6% of these loans are charged off and Past due resepctively. 4.3% of the loans are also defaulted. Is there something responsible for thes. Is there someting the can be done to turn this over?

Focusing on Chargedoff, defaulted and past due loans, Loans collected for Medical/Dental, household expenses, Not Available, Large Purchases have relatively low completion rates compared to the other listing categories. These categories of loans also had high pecentages of Chargedoff and Past due loans with a minimum Chargeoff percentage of 18.8% and Past due percentage of 10.8%. 

Breaking it down. The followig categories that the least completion rate in ascending order:
- Medical/Dental
- Household Expenses
- Not available
- Large Purchases
- Business
- Taxes

The followig categories have the highest Chargeoff percentage in descending order:
- Household Expenses
- Medical/Dental
- Business
- Personal Loan
- Not available
- Taxes

Recall Employed, Full-time (45.59%), Employed (33.18%), Not available (9.74%), Self-employed (5.54%) and Part-time (1.93%) accounts for 96% of the loan listings(excluding current, cancelled and FinalPaymentInProgress loans). Of these Employments status, Self-Employed has the highest Chargedoff loans (29.51%), followed by Full-time (21.34%).  Loans with a Borrower Employment status of "Not Available", which accounts for accounts for 9.74% of the loan listings (excluding current, cancelled and FinalPaymentInProgress loans), had the least completion loans (57.6%), with 22.5% defaulted loans and 19.9& of Chargedoff loans.  Other, Retired, and Not employed, whilst accounting for a small percetage of the loan listings, have High chargedoff and defaulted loans. With Other and Not Employed having over 32% chargedoff loans, and other having 13% Defaulted loans. Past time, Full time and Self employed have the highest number of completed loans.

Defaulted and Chargedoff loans have a low median for StatedMonthlyIncome as compared to Past due, Completed loans
Transactions that are past due have higher Loan Original amount, followed by loans that were charged off. But a larger proportion of Defaulted loans have Loan Original amount greater than 15000. This is closely followed by Past due and defaulted loans. There is weak negative linear correlation between Stated Monthly income and debt-to-income ratio. Higher values for Stated Monthly income have a lower debt-to-income ratio.  There is weak positive correlation between between Stated Monthly Income and Monthly Loan Payment and  between Stated Monthly Income and Loan Original Amount
There is no linear correlation between Loan Original Amount and Debt-to-Income ratio and between Monthly Loan Payment and Debt-to-Income, but lower values of Debt to income ratio had higher values for monthly loan payment.

There is a strong linear correlation between Monthly Loan Payment and Loan Original Amount, higher values of Loan Original Amount had higher values for monthly loan payment and vice versa.

There is a strong linear correlation between Loan Original Amount and Monthly Loan Payment. Defaulted, Chargedoff, Past due loans have higher Loan Original amount and slightly higher monthly loan payment.The opposite is the case for completed loans.
Defaulted Loans and Past due loans had relatively lower StatedMonthlyIncome and a higher DebtToIncomeRatio and compromised majorly of 3 year loans. Completed Loans have a lower DebtToIncomeRatio and higher StatedMonthlyIncome. Defaulted and charged off loans have lower stated monthly income and relatively a larger pecentage of low Loan original amount as opposed to Completed and Current loans

## Key Insights for Presentation

- Of 113,937 loan listings, Majority(49.65%) of the loans are current, 33.42% of the loans are completed, 10.53% and 4.40% are chargedoff and defaulted respectively with 1.81% percent Past due

- 14.89% of the loans that had a listing category of "Not Avialable", a whooping 51.18% of the loans were listed for Debt Consolidation, 6.53% and 6.31% were listed as Home improvement and business respectively. The top 10 listings excluding the "Not available" category are
    - Debt Consolidation
    - Other
    - Home Improvement    
    - Business              
    - Auto                   
    - Personal Loan          
    - Household Expenses     
    - Medical/Dental         
    - Taxes                 
    - Large Purchases
    
- The Original Loan amounts are majorly multiple of 5000s ranging from 5000 - 35000, But 95% of the original loan amount are less than or equal to 20,000 and the 95th percentile of monthly loan payments is greater than 1/36 of the 95th percentile of the Original loan amount. ***This implies, that a 25000 loan would be completed in less than or 36 months if a borrower makes a monthly payment greater than or equal to 556 which is less than the 92nd percentile of the monthly loan paymets.***

- 1 year loans are good for business, but they only account for 1.42% of the loan listing. They have a whooping 94% completion rate. The Chargedoff 1 year loans have low stated monthly income. Only 66.8% of the 3 year loans were completed. Not high enough. 21.2% and 9.4% of the 3 year loans were Chargedoff and defaulted respectively. Now that's bad for business. but it doesn't just end there. 5 year loans are just as bad or worse. With a completion rate of only 55.3%. 24.8% and 15.6% of these loans are charged off and Past due resepctively. 4.3% of the loans are also defaulted. Is there something responsible for thes. Is there someting the can be done to turn this over?

- Self-Employed has the highest Chargedoff loans (29.51%), followed by Full-time (21.34%). 
- Loans with a Borrower Employment status of "Not Available", which accounts for accounts for 9.74% of the loan listings (excluding current, cancelled and FinalPaymentInProgress loans), had the least completion loans (57.6%), with 22.5% defaulted loans and 19.9& of Chargedoff loans. Other, Retired
- Not employed, whilst accounting for a small percetage of the loan listings, have High chargedoff and defaulted loans. 
- With Other and Not Employed having over 32% chargedoff loans, and other having 13% Defaulted loans. Past time, Full time and Self employed have the highest number of completed loans.

- Defaulted Loans and Past due loans had relatively lower StatedMonthlyIncome and a higher DebtToIncomeRatio and compromised majorly of 3 year loans. Completed Loans have a lower DebtToIncomeRatio and higher StatedMonthlyIncome. Defaulted and charged off loans have lower stated monthly income and relatively a larger pecentage of low Loan original amount as opposed to Completed and Current loans

