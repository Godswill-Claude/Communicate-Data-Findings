# Communicate-Data-Findings - Prosper Loan Data Exploration

## Dataset
> This project is concerned with the exploration and visualization of the loan data from Prosper (a registered, legitimate loan-lending company in the United States). 

> The dataset contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income and many others. However, this project does not attempt to explore all of the variables in the dataset; we will focus our exploration on about 10-15 of them.

> The dataset can be found in the following address: [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), while the data dictionary to understand the various variables contained within can be acccessed via the address: [here](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554486256024000)

> The python programming language, along with libraries such as pandas, numpy, matplotlib, seaborn and scipy, was used for the explorations and visualizations contained in this work. 

## Key Insights for Presentation
  I decided to explore and discovered the following insights
  
> INSIGHT #1: Which features affect the borrower’s APR or interest rate?

> I chose this because the annual percentage rate (APR) of a loan also has a bearing on the loan status at the end of the day, so it is a very important variable in the dataset, in my view.

> To explore this, first I checked BorrowerAPR against LenderYield and then LoanOriginalAmount using a heatmap in both cases. Next, I checked the relationship between BorrowerAPR and ListingCategory_numeric using a barplot. I then went on to investigate the BorrowerAPR vs Occupation using a pointplot. Again, I examined BorrowerAPR vs MonthlyLoanPayment using a scatterplot.

> INSIGHT #2: What factors affect a loan’s outcome status?

> I chose this insight as a natural follow up to my first insight, and also because the LoanStatus variable is a key variable of my interest

> I took the following steps to obtain the required insight: LoanStatus vs EmploymentStatus using a heatmap, LoanStatus vs BorrowerRate using a boxplot and LoanStatus vs CurrentCreditLines using a violinplot; I also ensured to look at the describe statistics in both cases.

> INSIGHT #3: If a customer is both employed and is a homeowner, does this affect the amount of loan he can be given by Prosper? Would Prosper company consider him more eligible to pay back the loan completely?
> I employed the help of the faceting technique to examine the relationship multivariately between the three variables EmploymentStatus, IsBorrowerHomeowner and LoanOriginalAmount.

## Summary of Findings

>  From the entire exploration process, I discovered some two factors that affect the borrower's annual percentage rate: 
    (1) The expected yield of the company/investors 
    (2) The original amount of the loan.

> More so, lower income earners tend to go for lower amounts of loans. Again, the reason why a loan is applied for also determines the amount of loan the customer obtains. Customers tend to take huge amounts of loans only for major and necessary expenses, and also only occasionally, than for everday expenses.

> The employment status and occupation of a customer and the borrower rate or APR of a loan are major factors determining if Prosper company would be able to successfully recover their loans.
