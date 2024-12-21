# Project Name
> EDA - Landing Club case study


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.
- What is the background of your project?
- What is the business probem that your project is trying to solve?
- ## Problem Statement:
> Conduct a comprehensive analysis of a dataset containing consumer attributes and loan attributes. Our goal is to gain insights into the factors influencing loan default rates and to develop strategies to mitigate risks associated with lending.
- What is the dataset that is being used?

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Conclusion 1 from the analysis 1
This visualization can help us understand the distribution of loan amounts in the dataset. We can see that most loans fall in the range of $5,000 to $15,000

![alt text](image.png)
- Conclusion 2 from the analysis 1
This visualization can help us understand the distribution of loans in the dataset. We can see that most loans issued in year 20011

![alt text](image-1.png)
- Conclusion from the analysis 2
![alt text](image-2.png)
- Conclusion from the analysis 3
![alt text](image-3.png)

- Conclusion from the analysis 4
**High-Risk Grades (E, F, G):**

**Key Indicators:**

>High median interest rates, reflecting the high likelihood of default.

>Wider IQR and more outliers, signaling a significant variability in risk levels.

>Risk Profile:

>These grades represent borrowers with poor credit histories or unstable incomes.

>Lenders face a high risk of non-payment, which is offset by charging much higher interest rates.

![alt text](interestGradeBox.png)

![alt text](interestSubgrade.png)
- Conclusion from the analysis 6

![alt text](image-4.png)

- Conclusion from the analysis 7


![alt text](image-5.png)
- Conclusion from the analysis 8
![alt text](image-6.png)
- Conclusion from the analysis 9

> **Debt-to-Income Ratio (DTI) and Risk:**

> Negative correlation between DTI and annual income (-0.11): 

> As income increases, the DTI ratio tends to decrease. A high DTI is a strong indicator of higher risk because it implies the borrower is already carrying a significant debt load relative to their income, which increases the likelihood of loan default.

> The weak positive correlation with loan amount (0.15) and revolving balance (0.26) also shows that higher loan amounts and higher balances tend to go hand-in-hand with a higher DTI, which is a risk factor for default.


> **Correlation between loan_amnt and other variables:**

> The loan amount (loan_amnt) has a moderate positive correlation with the interest rate (int_rate) at 0.30 and a slightly higher positive correlation with annual income (annual_inc) at 0.41.
> It also has moderate positive correlations with revolving balance (revol_bal) and total accounts (total_acc).
Interest rate correlations:

> The interest rate (int_rate) has a low positive correlation with loan amount (loan_amnt), but it has very low correlations with other variables like annual income (annual_inc) and revolving balance (revol_bal).

![alt text](image-7.png)
- Conclusion from the analysis 10

**Risk Implication:**

Debt consolidation loans are often used by individuals facing financial stress or managing existing debt. Therefore, loan grades D and E, with their high frequencies for debt consolidation, may reflect higher financial distress and a higher risk of default.

Credit card loans also seem to be somewhat common in these grades, further suggesting that borrowers in these grades may have challenges managing credit and could be at risk.

**Risk Insights:**
Debt consolidation is strongly associated with higher-risk borrowers (grades D, E, F, G and sub-grades D4, D5). Borrowers in these groups are likely facing financial struggles, making them higher-risk for loan defaults.

Home improvement and small business loans, while somewhat common across sub-grades, show lower frequencies in riskier grades. These loan purposes may still indicate a level of financial planning or stability, but they are less prominent in the high-risk groups.

Credit card loans show a mixed frequency across grades and sub-grades. This could suggest that some borrowers in lower grades are using loans for credit-related needs, which can indicate over-reliance on credit, adding to the default risk.

![alt text](image-8.png)
- Conclusion from the analysis 11

**As the loan grade decreases (from A to G), the revolving utilization increases for each loan status category.**

There is variation within each grade and sub-grade, with some sub-grades showing significantly higher utilization rates, especially in the "Charged Off" and "Fully Paid" categories.

![alt text](image-9.png)

- Conclusion from the analysis 12

**Fully Paid Loans:**

Median revolving utilization is lower compared to the other statuses.

Indicates that borrowers who fully repay loans tend to have more conservative credit usage.

The interquartile range (IQR) shows a narrower spread, suggesting more consistent credit behavior.
Charged Off Loans:

**Charged Off Loans:**

Median utilization is higher than Fully Paid loans, suggesting riskier credit behavior.

The IQR is wider, indicating a higher variability in credit usage among borrowers whose loans are charged off.

Borrowers in this group often have high utilization, hinting at financial stress or over-leverage.
Current Loans:

**Current Loans:**

Median utilization is slightly below Charged Off loans but above Fully Paid loans.

Reflects borrowers who are actively paying loans but may have higher revolving credit balances.

IQR suggests a moderate spread, showing variability in usage but less than Charged Off loans.

![alt text](revolvingBox.png)
- Conclusion from the analysis 13
![alt text](image-10.png)
- Conclusion from the analysis 14

Insights:
**Risk Assessment:**

Borrowers with sub-grades in the F and G categories represent high-risk groups due to their high revolving utilization. These borrowers are more likely to default or struggle with repayments.

**Borrower Behavior by Sub-Grade:**

Borrowers with lower sub-grades (e.g., A and B) tend to use credit sparingly, making them safer for lenders.

Higher sub-grade borrowers (E, F, G) exhibit risky behavior with higher utilization, potentially signaling over-leverage or poor financial management.


**Custom Lending Criteria:**

Offer better terms (e.g., lower interest rates) to A and B borrowers to encourage safe credit usage.

Consider stricter repayment schedules or additional guarantees for F and G borrowers.

![alt text](image-11.png)
- Conclusion from the analysis 15

**Risk Differentiation:**

Sub-grades F and G consistently display high utilization across all loan statuses, indicating they are the riskiest borrowers regardless of their loan outcome.

**Loan Status Analysis:**

Charged Off loans have significantly higher utilization compared to fully paid loans across all sub-grades, confirming that revolving utilization is a key risk indicator for defaults.

Current loans are intermediate, showing higher utilization than fully paid loans but lower than charged off loans, reflecting their ongoing risk exposure.
Credit Behavior by Sub-Grade:

Lower sub-grades (A and B categories) demonstrate strong financial discipline, with consistently low utilization, even for charged-off loans.
Borrowers in sub-grades G2, G3, and G4 are outliers with dangerously high utilization, particularly for charged-off and current loans.

![alt text](image-13.png)
- Conclusion from the analysis 16
![alt text](image-12.png)
- Conclusion from the analysis 15
![alt text](image-14.png)
- Conclusion from the analysis 15
![alt text](image-15.png)
- Conclusion from the analysis 15
![alt text](image-16.png)
- Conclusion from the analysis 20
![alt text](image-17.png)
- Conclusion from the analysis 21


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- python - version 3.12.4
- pandas - version 2.2.2
- matplotlib - version 3.8.4
- seaborn - version 0.13.2
- Plotly 5.22.0
- Jupyter Notebook
- Anaconda Navigator 2.6.3
- Visual Studio Code 1.96.0


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->