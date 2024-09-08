# Exploring-Customer-Behavior

### The Problem
YoloNet, a telecommunications company, is struggling with a high churn rate and increasing complaints from senior citizens. Senior customers are experiencing difficulties with the technology and inadequate support, leading to dissatisfaction and leaving the company.

### Dataset Overview
The provided dataset contains customer information, demographics, service usage, and contract details. The columns include attributes such as:
- Customer Demographics: customerID, gender, SeniorCitizen, Partner, Dependents
- Service and Contract Details: tenure, PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, streaming movies
- Payment Information: Contract, PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges
- Churn: Whether the customer has churned or not.

### Exploratory Data Analysis (EDA)
We conducted an initial EDA better to understand the data distribution and relationships between variables. The EDA steps included:
- Data Overview: We reviewed the dataset's structure, missing values, and basic statistics.
- Distribution Plots:
  - The distribution of churn (Yes/No) using a count plot.
  - The distribution of tenure and monthly charges.

### Analysis and Insights
Here are the results of the analysis based on the questions we sought to answer:
#### What is the average monthly charge across different customer demographics?
  
  - Average monthly charges by senior citizen status
    
  <img width="395" alt="Screenshot 2024-09-07 at 5 01 13 PM" src="https://github.com/user-attachments/assets/d153e273-5f25-409b-9d2d-d30cea62a9ab">

  - Average monthly charges by gender
 
  <img width="449" alt="Screenshot 2024-09-07 at 6 36 06 PM" src="https://github.com/user-attachments/assets/91806fa2-b080-46b1-aee5-1c45e88ad47c">

  - Average monthly charges by partner status
 
  <img width="474" alt="Screenshot 2024-09-07 at 6 36 31 PM" src="https://github.com/user-attachments/assets/9a9cc3fb-6aa6-4770-8e88-f31362af95b8">

##### Finding:
- Senior citizens contribute 56.3% of the average monthly charges, compared to 43.7% for non-senior citizens.
- On average, males and females have monthly charges around $65.
- Customers with partners have a slightly higher average monthly charge ($68) compared to those without partners ($62).

##### Interpretation: 
Senior citizens may opt for higher-priced services or packages, and being in a relationship (having a partner) correlates with slightly higher service charges.

##### Recommendation: 
To maintain or increase customer satisfaction, consider targeted offers for senior citizens and partner-based households, such as bundling services that cater to their specific needs.

#### How does the presence of dependents affect customer tenure?

<img width="443" alt="Screenshot 2024-09-07 at 7 17 20 PM" src="https://github.com/user-attachments/assets/a07ceeb2-8e18-43fb-8cc1-88a14bfa48fc">


##### Finding: 
A weak positive correlation (0.16) exists between having dependents and customer tenure. Customers with dependents may have slightly longer tenures, but the relationship is not strong.

##### Interpretation: 
While having dependents slightly correlates with longer tenure, other factors like service satisfaction, pricing, and lifestyle needs could be more influential in determining customer retention.

##### Recommendation: 
Although the impact of dependents is small, targeted retention strategies for families, such as family-oriented packages or services, may still help enhance tenure for a specific subset of the customer base.


#### Is there a correlation between payment method and churn?

<img width="395" alt="Screenshot 2024-09-07 at 7 17 53 PM" src="https://github.com/user-attachments/assets/ae549d75-3ddd-489b-9f34-3cbc031aae39">


##### Finding:
- Customers using electronic checks have a higher churn rate than those using other payment methods.
- Automatic bank transfer or credit card payments reduce churn, suggesting better retention.
- Mailed checks have a slightly higher churn rate than automatic payments but lower than electronic checks.
- A correlation value of 0.11 indicates a very weak relationship between payment method and churn.

##### Interpretation: 
While the payment method impacts churn, it is not a strong predictor. However, customers using electronic checks seem less committed to long-term retention.

##### Recommendation: 
Offering incentives (e.g., discounts, perks) for customers who switch to automatic payment methods could encourage them to adopt them, reducing churn.


### Recommendations
- Introduce Family and Senior-Centric Offers: Design specialized service packages for senior citizens and families with dependents. These could include discounts on bundles or tailored services such as health and wellness programs for seniors or family data-sharing plans.

- Promote Automatic Payment Options: Given the lower churn rate among customers using automatic payment methods, consider offering promotional campaigns to encourage customers to switch to automatic billing methods. For example, small discounts can be provided for customers opting for bank transfers or credit card payments.

- Enhance Customer Retention Strategies: Since dependents alone don't seem to increase tenure drastically, focus on other customer retention strategies, such as loyalty programs, personalized customer support, and regular check-ins with customers in the early stages of their tenure (e.g., within the first six months).




