# Customer-Lifetime-Value-Prediction
# Background Business Problem Understanding
![image](https://github.com/user-attachments/assets/1d14069b-0e7f-4a2d-a986-e88685a6d452)



Customer Lifetime Value (CLV) is the amount of money a customer spends on a company throughout the business relationship between the customer and the company. Simply put, CLV is a prediction of the total revenue that can be obtained from the customer. Understanding and improving CLV in a company can increase company profits, help plan budgets, and analyze customer satisfaction. In its implementation, the CLV metric is widely used by companies that make repeat sales to customers (e.g., food, household products) as well as companies that use a subscription system in their business (e.g., insurance, telecommunications companies).

Suppose we have a car insurance company, PT Asuransi Mobil Sejahtera. In this context, CLV is the total revenue that PT Asuransi Mobil Sejahtera expects to get from a customer during their business relationship. For example, if a customer pays a car insurance premium of IDR 1,000,000 per year and usually stays with the company for 10 years, then the CLV of the customer is IDR 10,000,000. However, in practice, the calculation of CLV can become more complex. Factors such as customer acquisition costs, retention costs, and churn probability (customers stop subscribing) need to be considered.

For example, if the customer acquisition cost is IDR 200,000 and PT Asuransi Mobil Sejahtera spends an average of IDR 50,000 per year on customer retention efforts, then this needs to be subtracted from the CLV. In addition, PT Asuransi Mobil Sejahtera may also want to consider other factors such as the claim value paid to customers, or additional income obtained from the sale of additional products. By understanding CLV, PT Asuransi Mobil Sejahtera can make better decisions about how much they should invest in customer acquisition and retention, as well as how they can improve customer satisfaction to increase CLV. This is the background of the problem in the context of a car insurance company’s customer lifetime value.

PT Asuransi Mobil Sejahtera can predict Customer Lifetime Value (CLV):

Premium Income: First, PT Asuransi Mobil Sejahtera needs to estimate how much premium will be paid by customers each year. For example, if a customer pays a car insurance premium of IDR 1,000,000 per year, this will be the basis for calculating CLV.

Duration of Relationship: Next, the company needs to estimate how long their business relationship with the customer is. For example, if customers usually stay with the company for 10 years, then this will be used in the CLV calculation.

Acquisition and Retention Costs: Customer acquisition costs and retention costs also need to be considered. For example, if the customer acquisition cost is IDR 200,000 and PT Asuransi Mobil Sejahtera spends an average of IDR 50,000 per year on customer retention efforts, then this needs to be subtracted from the CLV.

Churn Probability: PT Asuransi Mobil Sejahtera also needs to consider the churn probability, which is the chance of customers stopping their subscription. This probability can be calculated based on the company’s historical data.

Claim Value and Additional Income: Other factors such as the claim value paid to customers, or additional income obtained from the sale of additional products, also need to be considered in the CLV calculation.

By understanding and predicting CLV, PT Asuransi Mobil Sejahtera can make better decisions about how much they should invest in customer acquisition and retention, as well as how they can improve customer satisfaction to increase CLV. Simply put, this is the background of the problem in the context of a car insurance company’s customer lifetime value.

# Problem Statement
![image](https://github.com/user-attachments/assets/74f8a3fb-1226-49b5-b34e-508e79b21d54)


In this project, there is a car insurance company in Indonesia, PT Asuransi Mobil Sejahtera, which is having problems in increasing company revenue. One of the causes of the problem is due to an inappropriate marketing strategy approach, where the company spends the same budget for all types of customers. As a result, PT Asuransi Mobil Sejahtera ends up paying more for low-value customers and losing high-value customers.

For this reason, PT Asuransi Mobil Sejahtera uses the Customer Lifetime Value (CLV) metric in order to determine how valuable the customers they have and the marketing strategy that will be used based on the CLV. However, PT Asuransi Mobil Sejahtera does not yet have a system to predict CLV quickly and accurately so that the determination of the current marketing strategy takes longer because data processing is still done manually.

Therefore, faster and more accurate CLV prediction is very important in order to take a more appropriate marketing strategy. Thus, PT Asuransi Mobil Sejahtera can optimize the use of marketing budgets, prioritize high-value customers, and ultimately increase company revenue. This is the background of the problem in the context of the Customer Lifetime Value of a car insurance company like PT Asuransi Mobil Sejahtera.

# Goals
---Based on the problems above, it would certainly be very helpful for PT Asuransi Mobil Sejahtera (especially the marketing division) if there was a tool to predict CLV by looking at demographic data and customer car insurance data (type of insurance, number of policies, premium costs, total claims, and others). With this tool, CLV data processing is no longer done manually and can speed up the decision-making process for marketing strategies. This will have a very positive impact on PT Asuransi Mobil Sejahtera in improving the efficiency and effectiveness of their marketing strategies.

# Metric Evaluation & The Reason for Choosing It
In the context of predicting customer lifetime value (CLV) for PT Asuransi Mobil Sejahtera, there are 3 recommended metrics that align with the objective: RMSE, MAE, and MAPE.

1. RMSE (Root Mean Squared Error):

Description: RMSE measures the average magnitude of errors between predicted and actual CLV values, with a focus on larger errors.

Applicability: For PT Asuransi Mobil Sejahtera, where accurately predicting CLV is crucial for business planning, RMSE is valuable. Large errors in CLV prediction could lead to misallocation of resources or missed opportunities for customer engagement.

2. MAE (Mean Absolute Error):

Description: MAE calculates the average absolute difference between predicted and actual CLV values, offering a measure of the average prediction error.

Applicability: MAE is useful for evaluating the average accuracy of CLV predictions for PT Asuransi Mobil Sejahtera. It provides a balanced view of model performance without emphasizing larger errors, which is important for understanding the overall accuracy of predictions.

3. R-Squared (Coefficient of Determination):

Description: R-Squared indicates the proportion of variance in the target variable (CLV) explained by the model. Higher values suggest better explanatory power.

Applicability: R-Squared helps PT Asuransi Mobil Sejahtera assess how well the model captures variation in CLV. A higher R-Squared indicates that the model effectively explains observed CLV fluctuations, which is essential for strategic decision-making.

4. MAPE (Mean Absolute Percentage Error):

Description: MAPE calculates the average percentage difference between predicted and actual CLV values, providing insight into relative error.

Applicability: MAPE offers perspective on the proportional accuracy of CLV predictions for PT Asuransi Mobil Sejahtera. It helps gauge how well the model performs in predicting CLV relative to actual values, which is valuable for understanding the impact of prediction errors. It's often useful to consider multiple metrics to get a comprehensive view of model performance. While RMSE, MAE, and R-Squared provide different perspectives, using a combination of them can offer a more nuanced evaluation.

There are other metrics that may not be recommended for use in predicting CLV for PT Asuransi Mobil Sejahtera:

1. MSE (Mean Squared Error):

Reason for Not Recommending: MSE places more emphasis on larger errors due to the squared difference. In the context of predicting CLV for PT Asuransi Mobil Sejahtera, where large prediction errors could have significant consequences, MSE might not be ideal as it could disproportionately influence the overall evaluation.
2. RMSLE (Root Mean Squared Logarithmic Error) and RMPSE (Root Mean Squared Percentage Error):

Reason for Not Recommending: Logarithmic or percentage transformations may not be necessary in this context. RMSLE tends to underestimate errors on high-value predictions, and RMPSE could be less intuitive. Simpler metrics like RMSE and MAE may provide a clearer evaluation of CLV prediction accuracy.
In conclusion, the choice of metrics (RMSE, MAE, and MAPE) aligns well with the objective of predicting customer lifetime value for PT Asuransi Mobil Sejahtera, considering the specific challenges and implications associated with insurance customer behavior and market dynamics. These metrics collectively offer a comprehensive evaluation of model performance, addressing both magnitude and relative accuracy of CLV predictions.

# Conclusion
In the conducted modeling, the features Number of Policies and Monthly Premium Auto emerged as the most influential features on Customer Lifetime Value. This aligns with the initial assumption that both features also have the strongest positive correlation with Customer Lifetime Value.

The evaluation metrics used for the model are RMSE, MAE, and MAPE. Considering the MAE value (as it is easier to interpret) obtained after hyperparameter tuning, which is 373.974, we can conclude that if in the future the built model will estimate the CLV of an auto insurance company within the range of values according to the model's limitations (maximum CLV value of 16624.75), then the estimated CLV value may deviate by approximately ± 373.974 from the actual CLV value. Alternatively, using the MAPE value, the estimated CLV value may deviate by approximately ± 4.8% from the actual CLV value.

However, this does not rule out the possibility of further deviations in predictions because there is non-uniform variance in the residual plot (estimation at CLV > 8000). The bias produced by this model could be due to the lack of features and data in the dataset that could better represent the CLV value itself.

Recommendation
# For Machine Learning Modeling
Check which predictions have high errors (either overprediction or underprediction), then explore further to identify which features contribute to high errors. If possible, add features related to CLV prediction, such as the length of time being a car insurance customer, classification of insurance coverage (e.g., Basic I, Basic II, Basic III, etc.), geographical region, and others. Add more customer data to improve the CLV prediction of the machine learning model. Utilize the built model for further model development, such as exploring the use of unsupervised learning (clustering) to segment profitable and unprofitable customers for better marketing strategy determination.

# For Business
Regarding Number of Policies and Monthly Premium Auto being the most influential features in predicting CLV, it is recommended to provide personalized offers to customers based on the number of policies and premium costs paid. Personalized offers are advantageous because the marketing budget used will also be personalized, thereby avoiding overpaying for low-value customers and losing high-value customers. With the knowledge of CLV predictions from machine learning, companies are advised to engage in upselling and cross-selling to customers. Upselling and cross-selling opportunities can lead to additional policy purchases and premium payments, potentially increasing customer CLV as well.

About
By understanding and predicting CLV, PT Asuransi Mobil Sejahtera can make better decisions about how much they should invest in customer acquisition and retention, as well as how they can improve customer satisfaction to increase CLV.
