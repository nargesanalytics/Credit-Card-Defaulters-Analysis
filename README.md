# Credit Card Defaulter
## Overview
In recent years, the credit card issuers in Taiwan faced the cash and credit card debt crisis and the delinquency is expected to peak in the third quarter of 2006 (Chou,2006).
In order to increase market share, card-issuing banks in Taiwan over-issued cash and credit cards to unqualified applicants.
At the same time, most cardholders, irrespective of their repayment ability, overused credit card for consumption and accumulated heavy credit and cash–card debts.
The crisis caused the blow to consumer finance confidence and it is a big challenge for both banks and cardholders.

# Dataset 
https://www.kaggle.com/datasets/d4rklucif3r/defaulter/data?select=credit_card_defaulter.csv

# What we know about dataset :

We have records of 30000 customers. Below are the description of all features we have.

- ID: ID of each client

- LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family/supplementary credit)

- SEX: Gender (1 = male, 2 = female)

- EDUCATION: (1 = graduate school, 2 = university, 3 = high school, 0,4,5,6 = others)

- MARRIAGE: Marital status (0 = others, 1 = married, 2 = single, 3 = others)

- AGE: Age in years

Scale for PAY_0 to PAY_6 : (-2 = No consumption, -1 = paid in full, 0 = use of revolving credit (paid minimum only), 1 = payment delay for one month, 2 = payment delay for two months, ... 8 = payment delay for eight months, 9 = payment delay for nine months and above)

- PAY_0: Repayment status in September, 2005 (scale same as above)

- PAY_2: Repayment status in August, 2005 (scale same as above)

- PAY_3: Repayment status in July, 2005 (scale same as above)

- PAY_4: Repayment status in June, 2005 (scale same as above)

- PAY_5: Repayment status in May, 2005 (scale same as above)

- PAY_6: Repayment status in April, 2005 (scale same as above)

- BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)

- BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)

- BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)

- BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)

- BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)

- BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)

- PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)

- PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)

- PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)

- PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)

- PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)

- PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)

- default.payment.next.month: Default payment (1=yes, 0=no)

# Objective
- Analysising by gender and education
- Analysising repayment status

# Data Cleaning Process
- Rename columns
- Replace values
- Remove columns
- Sum of total bills and repayments

# Exploratory Data Analysis
## new meausers
- Sum of Bills = SUMX(Data,Data[Total Bill])
- Sum Of Repayment = SUMX(Data,Data[Total Pay Back])
- Defaluters = CALCULATE(COUNT(Data[default payment next month]),Data[default payment next month] = 1)


# Visualization
- https://github.com/nargesanalytics/Credit-Card-Defaulters-Analysis/blob/main/credit.pbix

# Kaggle 
- https://www.kaggle.com/code/nargeshaghparast/credit-card-correlation
- 

# Suggestions:
Addressing the credit card debt crisis in Taiwan requires a multi-faceted approach involving both regulatory measures and consumer education initiatives.
Here are some suggestions to mitigate the crisis:

1. **Regulatory Measures:**
   - Strengthen regulations on credit card issuance to prevent over-issuance to unqualified applicants. Implement stricter eligibility criteria and conduct thorough credit assessments to ensure that cardholders have the financial capacity to repay their debts.
   - Enforce responsible lending practices by imposing limits on credit card limits based on borrowers' income levels and debt-to-income ratios.
   - Introduce caps on interest rates and fees charged by credit card issuers to protect consumers from exorbitant charges that contribute to debt accumulation.
   - Enhance monitoring and enforcement mechanisms to detect and penalize predatory lending practices, including aggressive marketing tactics targeting vulnerable consumers.

2. **Consumer Education and Financial Literacy Programs:**
   - Launch public awareness campaigns to educate consumers about responsible credit card usage, debt management strategies, and the consequences of overspending.
   - Provide financial literacy programs in schools, workplaces, and community centers to equip individuals with the knowledge and skills to make informed financial decisions.
   - Offer counseling services and debt management workshops for individuals struggling with credit card debt, providing them with resources and support to regain control of their finances.
   - Collaborate with financial institutions, consumer advocacy groups, and government agencies to develop educational materials and resources tailored to different demographics and socio-economic backgrounds.

3. **Debt Relief and Rehabilitation Programs:**
   - Establish debt relief programs to assist individuals burdened with heavy credit card debt, such as debt consolidation, repayment plans, or negotiated settlements with creditors.
   - Provide financial assistance and counseling services to help individuals develop personalized debt repayment strategies and improve their financial literacy and money management skills.
   - Encourage banks and credit card issuers to offer flexible repayment options, hardship programs, and debt restructuring arrangements to support borrowers facing financial difficulties.

4. **Credit Reporting and Monitoring Systems:**
   - Strengthen credit reporting systems to ensure accurate and comprehensive data on individuals' credit histories, facilitating better risk assessment and lending decisions by financial institutions.
   - Implement credit monitoring tools and alerts to notify consumers of any suspicious or unauthorized transactions, helping them detect and prevent fraudulent activity on their accounts.
   - Promote responsible credit behavior by incentivizing timely payments, positive credit habits, and prudent financial management through credit scoring mechanisms and rewards programs.

