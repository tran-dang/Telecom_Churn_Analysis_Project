# Telecom Churn Rate Insights - Project Overview
## The target of this project is to visualize and analyze a Telecom company's customer data, encompassing personal, accounting, and service-related information. The aim is to study churner profiles, identify areas for implementing marketing campaigns, and develop methods to predict future churners.

In today's fiercely competitive business environment, retaining customers is vital for sustained success. Churn analysis plays a pivotal role in understanding and mitigating customer attrition. This process entails examining customer data to pinpoint patterns and reasons behind their departures. Leveraging advanced data analytics and machine learning, businesses can forecast which customers are at risk of leaving and discern the factors influencing their decisions. This insight empowers companies to take proactive measures to enhance customer satisfaction and loyalty.  

While this project centers on churn analysis for a telecom company, the methods and insights gained are relevant to many industries. Whether in retail, finance, healthcare, or other sectors, any business that prioritizes retaining customers can benefit from churn analysis.


## Dataset Structure
The dataset consisted of one primary table, of which three references were made to base the analysis on combined with two mapping table, including information about customer demographic and geography, talks about services the customer subscribed to, as well as payment & revenue information
<!-- 

case types, wait time and specialties, as well as age demographics, admission date, and related patient information
<details>
  <summary>More Information</summary>
  
  ### Tables used
  - *Inpatient*: Contains data specific to inpatient waiting lists (Combined from 4 tables).
  - *Outpatient*: Contains data specific to outpatient waiting lists (Combined from 4 tables).
  - *All_data*: Consolidates data from the Inpatient and Outpatient tables, and is used for all visualizations and analyses in this project (Appended from Inpatient and Outpatient).
  - *Mapping_Specialty*: Used for mapping purposes and linking data points geographically.
  The All_data table is the primary dataset used for the analysis, allowing for comprehensive visualizations and insights.
  
</details>
<img width="812" alt="image" src="https://github.com/tran-dang/Healthcare_Analytics_Project/blob/main/assets/Tables.png">
-->


## Insights Summary
#### To evaluate customer retention and acquisition, we focused on the following key metrics:
- Total Churn & Churn Rate: The total number of customers who have left the services and the churn rate, calculated as the percentage of customers who have unsubscribed over a specific period.
- Churn Reason & Reason Category: The specific reasons for customer churn and the categories these reasons fall into, to better understand why customers are leaving and address these issues proactively.
- Age Profile: The distribution of customers across different age groups to identify demographic trends.
- Tenure Profile: The distribution of customers based on their tenure with the company to understand retention patterns over time.


#### Total Churn & Churn Rate: 
- Total Customers and total Churn Rate are positively correlated with each other. 
- Total Churn for females (1,111) was higher than for males (621).

#### Churn Reason & Churn Category: 
- Through all indicators, the top Category for Churn Reason is Competitors at 43.94%, followed by Attitude (17.38%) and Dissatisfaction (17.32%).
- In Competitors, the Churn Reason is mostly "Competitor had better devices" (37.98%) and "Competitor made better offer" (36%).

#### Age Profile: 
- Across all categories, the [> 50] age group accounted for a comparatively high portion (42.52%) of Total Customers and constituted a significant portion of Total Revenue (44.14%).
- Notably, this age group has the highest number of Total Customers (2,729) and was 2,232.48% higher than the [< 20] age group, which had the lowest number of Total Customers at 117.
- Regrettably, the churn rate for this demographic is the highest at 31.6%, with the majority (34.42%) leaving within the 6 - 12 months timeframe.

#### Tenure Profile: 
- Across all 5 Tenure Groups, the count of customers ranged from 980 to 2,087, and Churn Rate ranged from 26% to 28%
- Although the Tenure Group [>= 24 Months] has the highest churn rate (27.5%) and is the biggest contributor to the overall churn count (33.12%), it is the highest contributor to Total Revenue (32.9%). 
- Conversely, the [12 - 18 Months] tenure group has the lowest churn rate (26.08%) and overall churn count (15%).
  
<!--
  <details>
    <summary>Detailed Information</summary>
    
    - *Accident & Emergency* saw a 100% increase in patients, rising from 0 to 1,111.
    - *Paed Cardiology* had a 31.82% decrease, dropping from 5,166 to 3,522.
    - *Paed Orthopaedic*'s wait list increased by 2.10%, from 4,962 to 5,066.
    - *Paediatric Dermatology*'s wait list grew by 6.01%, from 4,837 to 5,128.
    - *Paediatric ENT*'s wait list decreased by 9.46%, from 7,549 to 6,835.
  </details>

-->

## Recommendations
<!-- 
- **Inpatient Process Optimization**:
Reallocate resources from elective procedures during peak periods to critical inpatient care, reducing wait times.
Implement a fast-track protocol for acute cases, minimizing non-essential administrative steps.
-->
- **Customer Segmentation by Age**: Direct marketing efforts towards the (> 50) age group, which constitutes a substantial segment of the customer base and a key revenue source, potentially delivering high returns with targeted strategies.

- **Gender-Specific Campaigns**: Since the total churn for females (1,111) was higher than for males (621), consider creating tailored marketing campaigns aimed at female customers to address their specific needs and reduce churn.

- **Tenure-Based Campaigns**: Analyze the tenure group data closely, and focus on customers with (>= 24) months of tenure to minimize churn by engaging and satisfying long-term customers. Additionally, implement targeted retention initiatives and personalized offers for the (12 - 18) months tenure group to ensure they remain engaged and loyal.

- **Competitor Analysis**: Address the top churn reason, which is Competitors. Develop strategies to counteract the main reasons, such as "Competitor had better devices" and "Competitor made better offer". Innovate product offerings to surpass competitors' devices and design captivating promotions that highlight unique value propositions to retain customers.
<!-- 
- **Monitor and Support New Joiners**: Keep track of the new joiners and provide them with excellent onboarding experiences. Offering special promotions or personalized support during their initial months could help improve their satisfaction and loyalty.

- **Overall Churn Strategy**: Given that total customers and churn rate are positively correlated, ensure continuous monitoring and analysis to identify any emerging trends. Use predictive models to proactively address potential churners and implement retention measures.
-->

## Dashboard
The dashboard is created in PowerBI, providing interactive visualizations that enable users to filter by category, specialty, age profile, and tenure groups, focusing on trends and values in total customers and churn rate.  
The analysis is presented through the following views:
- Summary Page: Provides an overall view of the churn status.
- Churn Prediction Page: Offers analysis of predictions on future churners.
View the dashboard [here](https://app.powerbi.com/reportEmbed?reportId=e7f97bbf-41b4-49ff-9e2a-38835ff5025d&autoAuth=true&ctid=5cdc5b43-d7be-4caa-8173-729e3b0a62d9) for more insights.

<img width="812" alt="image" src="https://github.com/tran-dang/Telecom_Churn_Analysis_Project/blob/main/images/SummaryView.png">

<img width="812" alt="image" src="https://github.com/tran-dang/Telecom_Churn_Analysis_Project/blob/main/images/ChurnAnalysisView.png">

