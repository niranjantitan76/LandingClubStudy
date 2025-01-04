# Project Name
> EDA - Landing Club case study


# Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

# General Information
- Provide general information about your project here.

    This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 
- What is the background of your project?

    Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.  

    If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

    This project is  a Data Exploration project and tries to find as much findings as possible without the use of any Machine Learning and just simple plain EDA and Data Visualization.

- What is the business probem that your project is trying to solve?

    Understanding the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.
# Problem Statement:
    Conduct a comprehensive analysis of a dataset containing consumer attributes and loan attributes. 
    Our goal is to gain insights into the factors influencing loan default rates and to develop strategies to mitigate risks associated with lending.

    Lending loans to "risky" applicants is the leading cause of financial loss, commonly referred to as credit loss, for banks and lending companies. By identifying these high-risk loan applicants, lenders can reduce the approval of such loans, thereby minimizing credit loss. This case study aims to leverage data analysis to identify and understand the characteristics of these risky applicants.
    By gaining insights into these factors, the company can enhance its portfolio management and risk assessment processes.

    There are two key risks associated with the bank's loan approval decisions:

    Loss of Business: If an applicant is likely to repay the loan, but the loan is not approved, it results in a missed business opportunity.
    
    Financial Loss: If an applicant is unlikely to repay the loan (i.e., is likely to default), approving the loan may lead to significant financial losses.
    
    This study aims to balance these risks by identifying patterns in the data to improve decision-making in loan approvals.

- What is the dataset that is being used?

    The dataset contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

    **Key Columns**

    The provided columns represent crucial predictors of loan outcomes. These attributes, collected during the loan application process, play a vital role in determining the likelihood of loan approval or rejection. By analyzing these factors, lenders can assess borrower risk and make informed lending decisions.

   **Borrower Characteristics**

   **Annual Income (annual_inc):** A key factor in creditworthiness, reflecting the borrower's earning capacity. Higher income generally increases loan approval likelihood.

    **Home Ownership (home_ownership):** Indicates ownership status (e.g., mortgage, rent, own). Homeownership often signals stability and can improve loan approval chances.

    **Employment Length (emp_length):** Represents the duration of the borrower's current employment. Longer tenures suggest greater financial stability and reduce loan risk.

    **Debt-to-Income Ratio (dti):** Measures the proportion of monthly income used for debt repayment. Lower DTI indicates lower financial burden and increases approval likelihood.

    **State (addr_state):** Represents the borrower's location, enabling regional analysis of delinquency and default rates.

    **revol_util:** Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
    
    **Loan Characteristics**

    **Loan Amount (loan_amt):** The amount of money borrowed, impacting both risk and potential return for the lender.

    **Grade (grade):** A creditworthiness rating assigned to the loan, reflecting the perceived level of risk. Higher grades generally indicate lower risk.

    **Sub Grade (sb_grade):** A creditworthiness sub rating assigned to the loan, reflecting the perceived level of risk. Higher sub grades generally indicate lower risk.

    **Verification Status (verification_status):** Indicates the level of income and employment verification conducted by the lender, influencing trust and risk assessment.

    **Term (term): **The loan's duration in months, influencing both interest payments and overall repayment burden.

    **Issue Date (issue_d):** The date the loan was originated, allowing for time-series analysis of loan performance.

    **Interest Rate (int_rate):** The annual percentage rate charged on the loan, reflecting the borrower's perceived risk.

    **Installment (installment):v The fixed monthly payment required to repay the loan over the specified term.

    **Purpose (purpose):** The intended use of the loan (e.g., debt consolidation, home improvement). Different purposes may carry varying levels of risk.

    **Public Records (public_rec):** The number of negative public records (e.g., judgments, liens) associated with the borrower, increasing loan risk.
    
    **Recoveries:** post charge off gross recovery
    
    **Public Records Bankruptcy (public_rec_bankruptcy):** The number of bankruptcy filings on the borrower's record, significantly impacting creditworthiness and loan approval likelihood.

# Objective

- **Importing necessary Modules**:
Import the modules necessary for Data Manipulation and Visualization.

- **Reading dataset**:
Read the dataset containing loan applicant information.

- **Exploring the Dataset**:
Understand the Structure and various datatypes of the attributes within the dataset.

- **Missing value analysis**:
Identify and analyze missing values in the dataset.

- **Analysing categorical and numerical columns**:
Analyze categorical and numerical columns to understand the statistical properties and relationships within the dataset.

- **Univariate Analysis**:
Conduct univariate analysis to explore the distribution and characteristics of individual variables.

 -   **Outliers**:
Identify and analyze outliers within the dataset to understand their impact on the analysis.

- **Bivariate analysis**:
Conduct bivariate analysis to explore relationships between different variables and their impact on loan default rates.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

# Conclusions

## Risk Assessment and Recommendations

## Grades B, C, and D 

Grades B, C, and D have the highest "Charged Off" loans.Lower grades (B-1396,C-1313,D-1085) exhibit a higher proportion of "Charged Off" loans, suggesting a higher risk of default for borrowers with lower creditworthiness.

**Recommendation:** 
- Reassess the risk evaluation criteria for grades B and C to better distinguish higher-risk borrowers.
- Implement stricter risk assessment and underwriting criteria for applicants in these grades. Utilize additional credit metrics, such as repayment history, to screen high-risk applicants more effectively.
## Subgrades C1, C2, B3, B4, and B5

Subgrades C1,C2, B3, B4, and B5 show a higher likelihood of defaults.Higher default tendencies in specific sub-grades indicate a need for more granular underwriting policies.

**Recommendation:** Focus on applicants in these subgrades by: 
- Offering smaller loan amounts.
- Introducing risk-based pricing with higher interest rates to offset potential losses.
- Providing pre-loan financial counseling.

## States

Applicants from states like California (CA), Florida (FL), and New York (NY) show higher default tendencies. Geographic concentration of risky loans could lead to localized portfolio risk exposure.

**Recommendation:**

- Introduce geographically adjusted lending strategies.
- Implement state-level risk mitigation strategies, such as stricter approval criteria for high-risk states.

## Interest Rate Comparison 

Risky loans are associated with higher interest rates compared to non-risky loans, but the spread between the two categories suggests that some risky loans may still be underpriced. Higher rates on risky loans might indicate an attempt to offset the increased probability of default, but affordability issues may arise.

**Recommendation:** Optimize pricing strategies for high-risk loans to balance profitability and affordability.

## Loan Status Distribution 

Most risky loans have been fully paid, but a significant proportion are charged off or currently delinquent. Charged-off loans highlight direct financial losses.
**Recommendation:** Focus on early warning signals to predict potential defaults and prevent charge-offs.

## DTI Ratios and Interest Rates

Most loans have interest rates between 10% and 20%. Borrowers with rates above 15% might have higher default risks due to affordability issues.

**Recommendation:**
- Adjust interest rates based on borrower DTI ratios.
- Cap DTI ratios for loan approvals or offer smaller loan amounts for borrowers with high DTI.
- Ensure that interest rates align with the borrower’s repayment capacity.

## Term Length

Applicants opting for 60-month loans are more likely to default.

**Recommendation:**

- Evaluate the risks of longer-term loans and consider limiting the maximum term.
- Offer 60-month loans at higher interest rates to account for elevated risk.

## Applicant Experience

Applicants with 10+ years of experience are more prone to defaults, suggesting experience is not a standalone creditworthiness indicator.

**Recommendation:** 
- Use a comprehensive credit scoring system that includes factors such as income, DTI ratio, and past loan behavior.
## Market Trend

Loan applications have steadily increased between 2007 and 2011, indicating market growth.

**Recommendation:** Continue leveraging this growth by:
- Maintaining competitive rates and efficient loan processing.
- Enhancing risk management practices to sustain profitability.
## Loan Demand

*Q4 and December see a peak in loan applications, likely due to holiday-related spending.

**Recommendation:** 
Prepare for seasonal demand surges by:
- Allocating additional resources to ensure timely processing.
- Offering promotional rates or tailored products during peak seasons.
## Debt Consolidation Loans

Debt consolidation accounts for the highest loan volume and default rates.

**Recommendation:**
    - Apply stricter eligibility criteria for debt consolidation loans.
    - Provide financial counseling to help applicants manage existing debts effectively.
## Housing Status

Renters and mortgaged homeowners are more likely to default. Renters may face more financial instability compared to homeowners, while mortgage holders might be over-leveraged.

**Recommendation:** Include housing stability as a key factor in the underwriting process. 
Consider:

- Adjusting interest rates or loan amounts based on housing status.
- Encouraging applicants to secure cosigners if housing status poses a risk.
- Applicants with higher housing costs (Rent or Mortgage) may require lower loan amounts or higher scrutiny.
## Verification Process

Verified applicants are defaulting more frequently than unverified ones.

**Recommendation:** Review the current verification process to:

- Improve its accuracy in identifying risky borrowers.
- Incorporate additional metrics, such as alternative credit data.

## Loan Amounts

Applicants with loan amounts of $15,000 or higher are more likely to default.

**Recommendation:**

- Set stricter caps on loan amounts for higher-risk borrowers.
- Require additional collateral or cosigners for larger loans.

## Annual Income Levels

Borrowers earning less than $38,000 annually have a higher likelihood of defaulting.

**Recommendation:**
- Provide financial education and budgeting resources for lower-income borrowers.
- Restrict maximum loan amounts or shorten loan terms for low-income applicants.
## Revolving Utilization (revol_util)

Revolving utilization is distributed across a wide range, with many borrowers exceeding 50%.High utilization indicates greater dependence on credit, correlating with higher default likelihood.

**Recommendation:** Reduce loan amounts or increase interest rates for high-utilization borrowers.

## Months Since Last Delinquency (mths_since_last_delinq)

Many borrowers have had delinquencies within the past 60 months. Recent delinquencies are strong indicators of repayment challenges.

**Recommendation:** Require additional proof of creditworthiness from borrowers with recent delinquencies.

## Risky Loans by Purpose 
- Debt consolidation and credit card refinancing are the top purposes for risky loans.
- Home improvement and small business loans also show significant representation.
- These categories often reflect financial distress or speculative investments.

**Recommendation:** Tighten evaluation for loans aimed at debt consolidation and small businesses, where risks are inherently higher.

Stricter Criteria for High Utilization Borrowers: Applicants with utilization rates above 50% should be closely monitored or required to lower their utilization before loan approval.

Financial Counseling and Education: Provide resources to help borrowers manage credit utilization and understand its impact on loan approvals and creditworthiness.

Dynamic Interest Rates: Adjust interest rates based on revolving utilization levels, with higher rates for higher utilization borrowers to offset risk.