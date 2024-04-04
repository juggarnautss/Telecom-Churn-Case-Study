# Project Name
> Telecom Churn Prediction

# Overview
In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business goal. To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. In this project, you will analyze customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn.
 

# Problem Statement
To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. 
- The goal is to build a predictive model that can predict the churn probability for a customer accurately.
- Identify key features that indicates the customer behaviour to churn

# Approach

**Data Understanding, Preparation, and Pre-Processing:**
- Data understanding involves the identification of potentially useful and non-useful attributes, as well as variable importance and impact estimation.
- Data preparation includes performing data cleaning, missing values imputation, outlier removal, and column level standardization (e.g., date) into one format.

**Exploratory Data Analysis:**
- Basic preliminary data analysis involves finding the correlation between variables and scatter plots to identify relationships between variables.
- Advanced data analysis includes plotting relevant heatmaps, histograms, and basic clustering to find patterns in the data.

**Feature Engineering and Variable Transformation:**
- Feature engineering involves performing one or more methods on attributes that can lead to the creation of a new potentially useful variable (e.g., day from the date).
- Variable transformation includes applying categorical variable transformations to turn them into numerical data and numerical variable transformations to scale the data.

**Model Selection, Model Building, and Prediction:**
- Identifying the type of problem and making a list of decisive models from all available choices.
- Choosing a training mechanism (e.g., cross-validation) and tuning hyperparameters of each model.
- Testing each model on the respective model evaluation metric.
- Choosing the best model based on the fit of the data set and output variable.
- Using ensemble options to improve efficacy based on the evaluation metric stated in the problem.

**Business Recommendation**


## Conclusions
- Logistic Regression with feature selection using Random Forest and RFE emerges as the best model from a business perspective.
- The primary goal is to reduce customer churn, making the identification of potential churning customers is crucial.
- Therefore, the most important metric is **SENSITIVITY**.
- The model demonstrates the following performance:
    - **Accuracy**: 0.76 (76% of the predictions are correct)
    - **Sensitivity**: 0.85 (85% of the customers identified have actually churned)

**Most important features are -**
- 'total_og_mou_8',
- 'total_og_mou_7',
- 'total_ic_mou_6',
- 'total_rech_num_8',
- 'loc_ic_t2m_mou_8',
- 'aon',
- 'last_day_rch_amt_8',
- 'mloc_ic_t2t_mou_8',
- 'av_rech_amt_data_8',
- 'std_ic_mou_8',
- 'roam_og_mou_8'

## Recommendations
- Total outgoing call duration (total_og_mou) shows a constant decline from June to August for churning customers. So, the sales team may talk to customers who are showing this decreasing trend and may provide discounts and offers as per their need.
- There is a decrease in incoming and outgoing calls usage for churning customers. If the business finds a decrease in the mou, then they should try to retain those customers by coming up with better offers, most likely unlimited plans, etc. Also, this may be due to poor network service in some areas where the network needs to be improved.
- A declining trend is observed with recharge columns as well. A decrease in the average recharge amount or an increase in the number of days since the last recharge is an indicator of churn. Provide offers and discounts.
- Outgoing calls during roaming are an important predictor variable; it looks like customers are churning for better roaming plans. The business can come up with better roaming packs for its customers.
- Age on network 'aon' is also an important feature. Old customers are least likely to churn. However, relatively new customers are prone to churn. The sales team must provide offers to new high-revenue customers to stop the churn.

## Contributors
- Sirin Shaikh


