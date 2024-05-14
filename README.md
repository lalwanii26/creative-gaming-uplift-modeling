# Uplift Modeling for Marketing Campaign Optimization

## Project Overview
This project focuses on the application of uplift modeling to optimize the effectiveness of a marketing campaign for the "Zalon" campaign by Creative Gaming. The goal is to identify the incremental impact of targeted advertising on customer behavior, distinguishing between those who received the ad and those who did not.

## Objective
The main objective is to employ uplift modeling techniques to enhance decision-making in marketing strategies, aiming to maximize the return on investment by targeting the customers most likely to respond positively to the campaign.

## Data Description
The dataset includes two main groups:
- **Control Group (cg_organic_control)**: Customers who did not receive the ad.
- **Treatment Group (cg_ad_random)**: Customers who received the ad.

Each record in the dataset includes customer demographics, past interaction data, and whether they responded to the campaign.

## Methodology
### Data Preparation
- Merging control and treatment group data.
- Ensuring balanced representation in training and test sets.

### Model Building
- Logistic Regression was used to predict the probability of a positive response in both the treatment and control groups.
- Calculation of uplift score by estimating the difference in probabilities between the two groups.

### Evaluation
- The models were evaluated using the uplift score, which measures the additional gain from targeting a customer due to the campaign.
- Performance was quantified using incremental uplift curves across various customer segments.

## Tools Used
- **Python**: For data manipulation and modeling.
- **Scikit-Learn**: For implementing logistic regression.
- **Matplotlib and Seaborn**: For data visualization.

## Results
- Developed a model that accurately predicts customer responsiveness to the ad campaign.
- Identified key customer segments that are most likely to be influenced by targeted advertising.
- Estimated an incremental revenue increase of over $1M by targeting the top 30,000 customers identified by the model.

## Conclusion
This project demonstrates the power of uplift modeling in enhancing marketing strategies by enabling more targeted, efficient, and effective ad placements. The approach can be generalized to other marketing datasets and scenarios to optimize resource allocation and maximize impact.
