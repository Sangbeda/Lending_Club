# Lending-Club-Case-Study
> A case study to understand the driving factors or driver variables behind loan default. The company can utilize this knowledge for its portfolio and risk assessment. 


## Table of Contents
* [General Information](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


## General Information
- Lending Club is a marketplace for personal loans that matches borrowers who are seeking a loan with investors looking to lend money and make a return. 
- When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
       If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
       If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial          loss for the company
- If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. 
- Identification of such applicants using EDA is the aim of this case study.
- The loan dataset contains the data of accepted loan requests across the time period of 2007-2011 correspoding to applicants who have fully paid the loan, who are in the process of paying the instalments, or who have defaulted on the loan.


## Conclusions
Overall, based on all the preceding analyses and inferences, we summarize this study as follows:
• The median loan amount, installment, funded amount, and the total amount committed by investors for that loan at that point in time are comparable for both cases of fully paid and charged-off (defaulted) loan status.
• The median loan amount, funded amount, the total amount committed by investors for that loan at that point in time, and the installment vary substantially across the purpose underlying the loan.
• The loans drawn for the purpose of small business are extremely risky, and ~27% of such loans have defaulted.
• Loans for educational purpose are highly likely to default if loan application profile is not verified.
• The state NV has the highest default rate of ~27%.
• The higher-amount loans are more likely to default.
• The verification process is apparently effective for loans with low and very low amount but not as effective for higher-amount loans.
• Loans with long tenure are more likely to default.
• The default percent is observed to increase with the progression from grade A to G.


In particular, it is counter-intuitive that (1) the median annual income is greater in case of defaulted loan status than in case of fully paid loan status, (2) that the number of defaulters is maximum in case of applicants with 10 or more years of experience, and (3) that the default rate is the highest in case of verified profiles.


Overall, based on these observations, we make the following recommendations:
(1) The verification process needs to be revisited at a policy level. Based on the data, verification seems to be apparently effective for loans with low and very low amount but not as effective for higher-amount loans. Necessary changes are required in the existing verification process, such that the loan applicant profiles encompassing diverse ranges of loan amounts are thoroughly verified.
(2) Since the default default percent is observed to increase with the progression from grade A to G, a closer look into the parameters underlying this grade allocation could give us more insight pertaining to this trend noted here. The parameters considered during gradation are not provided in the original data file; thus, we could not proceed with further analysis of such parameters. We recommend invetigation of those parameters underlying gradation.
(3) Since loans characterized by longer terms and higher amounts have shown higher default rates, we recommend deciding on a upper limit on the amount of loan that an applicant can apply for and is sanctioned. Furthermore, shorter terms are recommended.
(4) We recommend treating the loans filed for from NV with additional verification and caution.
(5) The loans applied for the purpose of business should also be treated with additional verification and caution. For these types of loans, specifically focusing on income verification of the application is recommended, as it has been observed that such loans are less likely to default upon income verification.
(6) The loans applied for the purpose of education should be thoroughly verified.

Although by leveraging EDA we have arrived at this stage with the aforementioned inferences and recommendations, to further determine the order of significance and effectiveness of these parameters in predicting loan default, a statistical analysis such as logistic regression or decision tree analysis can be performed. These methods can help identify the most significant predictors of default by assessing the strength of the relationship between each predictor and the outcome variable (default or non-default). After performing the statistical analysis, the parameters can be ranked in order of significance in predicting loan default. This ranking can then be used to develop a predictive model for identifying risky borrowers and mitigating default risk.


## Technologies Used
- NumPy - version 1.23.5
- Pandas - version 1.5.3
- Matplotlib - version 3.7.0
- Seaborn - version 0.12.2

## Contact
Created by Sangbeda Das (sangbeda.das@gmail.com) - feel free to contact me!
