# Creative Gaming: Uplift Modeling

## Project Overview
This project applies uplift modeling to optimize the marketing campaign effectiveness for the mobile game "Space Pirates" developed by Creative Gaming. The focus is on understanding the incremental impact of the marketing campaign on user conversion rates.

## Objective
To utilize uplift modeling to identify customer segments most likely to respond positively to the marketing campaign, thereby maximizing the efficiency of marketing spend.

## Data Description
The data consists of two main groups:
- **Control group (`cg_organic_control`)**: Users who did not receive the marketing campaign.
- **Treatment group (`cg_ad_random`)**: Users who received the marketing campaign.

Each user record includes demographics, gameplay data, and whether they made a purchase during the campaign.

## Methodology
### Data Preparation
Merged control and treatment data, ensuring balanced groups for unbiased analysis.

### Model Training
- **Logistic Regression and Random Forest Models** were used to predict the likelihood of conversion.
- **Uplift Calculation**: Uplift scores were calculated by the difference in predicted probabilities between the treatment and control models.

### Evaluation Metrics
- **Accuracy and Uplift Scores**: Evaluated using test datasets to ensure model reliability.
- **ROC Curves**: Generated to compare model performance and validate accuracy.
- **Incremental Uplift Curves**: Created to visualize the effectiveness of the models in increasing conversion rates across different customer segments.
- **Uplift Tables**: Detailed tables showing incremental responses and profitability metrics for targeted customer segments.

## Tools Used
- Python, Scikit-Learn, Statsmodels for statistical modeling and machine learning.
- Matplotlib and Seaborn for data visualization.

## Results
- **Model Performance**: Logistic Regression and Random Forest models successfully predicted customer responses with high accuracy.
- **Key Metrics**:
  - **Uplift Score**: Demonstrated significant incremental conversion gains, quantifying the additional conversions achieved by targeting users identified by the model.
  - **Incremental Profit**: The uplift model increases incremental profits by $39,182.65, a 247.39% increase over the propensity model when targeting the top 30,000 customers out of 120,000. There are two reasons for this - First, the uplift model sorts consumers by uplift, not propensity, which is the right sorting order if we want to maximize incremental profits. Second, the uplift model uses a breakeven that takes into account the fact that the marginal customer can generate profit organically.
  
## Visualizations Included in the Repository
- **Uplift Curves**: Demonstrate the incremental conversion gains by targeting different customer deciles.
- **ROC Curve**: Show the diagnostic ability of the logistic regression model.
- **Feature Importance Chart**: Highlight the most influential variables driving model predictions.

## Conclusion
This uplift modeling project has successfully demonstrated how targeted marketing can significantly enhance customer engagement and conversion, leveraging sophisticated predictive modeling to optimize resource allocation and drive substantial business impact in the gaming industry.
