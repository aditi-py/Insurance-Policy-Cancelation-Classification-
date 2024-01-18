# Insurance Policy Cancellation Prediction

This project involves building a multiclass predictive model to predict the likelihood of policy cancellations and renewals based on historical policy data. The dataset, named Kangaroo, spans four years of property insurance policies from 2013 to 2017.

## Dataset Description

The Kangaroo dataset consists of approximately 1 million policies in the training data, with each policy having one observation. Nearly 230,000 policies were canceled during the effective term. Below are the variable descriptions:

- `id`: Policy id (cannot be used in the model)
- `tenure`: Number of years with Kangaroo
- `claim.ind`: Occurrence of claim (0=no, 1=yes)
- `n.adults`: Number of adults in the property
- `n.children`: Number of children in the property
- `ni.gender`: Gender of the policyholder
- `ni.marital.status`: Marital status of the policyholder (0=no, 1=yes)
- `premium`: Price of the policy
- `sales.channel`: Medium through which the policy was purchased
- `coverage.type`: Type of coverage
- `dwelling.type`: Type of dwelling
- `len.at.res`: Length at residence (how long policyholder lived at the property)
- `credit`: Financial credit level of the policyholder
- `house.color`: Color of the house
- `ni.age`: Age of the policyholder
- `year`: Year of the policy
- `zip.code`: Zip code of the property
- `cancel`: Cancellation indicator (0=not cancel, 1=may cancel but can be convinced, 2=cancel)

Rows with `cancel==-1` have been deleted.

## Project Objective

The main objective is to create a predictive model on the training data to predict the cancellation indicator for each policy in the test data. The model aims to identify policies most likely to be canceled or renewed, and understand the variables most influential in causing a policy cancellation.

## Conclusion

On closely calculating the cancellations based on coverage type I found that coverage A had the highest cancellation percentage at 72% and C had the lowest at 69% , however C saw the most cancellations at 35237 cases and also a may cancel at 11473. This indicates a high dissatisfaction with the coverage type C. Measures must be taken by the company to improve the coverage type C and further introduce marketing strategies like incentivising policy renewals in alignment with the rate of cancellations in all three categories. Furthermore brokers can make sure to put in extra efforts of maintaining an healthy relationship with policy holders of coverage type C . To do an root cause analysis , factors like claims settlement of all the coverage type can be analysed to understand customer behaviour

The insurance company should make a concerted effort to communicate regularly via the brokers with policyholders, providing them with relevant information about their policies, and addressing any concerns they may have.

For detailed code implementations, refer to the provided code file.
