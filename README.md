# E-Commerce Customer Experience & Delivery Analytics

## Project Overview

An end-to-end data analytics project analyzing **50,000 e-commerce orders** to understand delivery performance, customer satisfaction, and return behavior.

The project uses **Python for data cleaning and exploratory analysis** and **Power BI for interactive dashboarding and business reporting**.

The main objective was to identify patterns between delivery performance, customer ratings, and returns and translate those findings into actionable business recommendations.

---

## Business Problem

An e-commerce business wants to better understand:

* How delivery performance affects customer satisfaction
* How return rates vary across customer segments and shipping methods
* Which product categories experience higher return activity
* What are the most common reasons for returns
* Whether delivery delays are associated with higher return rates
* Which operational areas require further investigation

---

## Objectives

1. Analyze overall delivery and customer-experience performance.
2. Identify patterns in delivery delays.
3. Analyze customer ratings across different delivery conditions.
4. Understand return behavior across categories, segments and shipping methods.
5. Identify the most common return reasons.
6. Build an interactive Power BI dashboard.
7. Translate analytical findings into business recommendations.

---

## Dataset

The dataset contains **50,000 e-commerce orders** and includes information related to:

* Order details
* Customer segments
* Product categories
* Order value
* Shipping methods
* Delivery status
* Delivery dates
* Delivery delays
* Delivery attempts
* Customer ratings
* Return requests
* Return reasons
* Warehouse information
* Carrier information
* Distance
* Weather conditions
* Order priority

---

## Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Microsoft Power BI**

---

## Data Cleaning & Preparation

The dataset was inspected and prepared using Python.

The analysis included:

* Checking dataset dimensions and data types
* Checking missing values
* Checking duplicate records
* Reviewing categorical variables
* Validating numerical ranges
* Converting `order_date` into a datetime format
* Creating delivery-delay groups
* Validating delivery, rating and return-related fields

### Important Data-Quality Observation

During validation, some orders that had not been successfully delivered contained customer ratings or return requests.

Since customer ratings and returns logically require the customer to have received the order, **delivered orders were used for customer-rating and return analysis**.

The full dataset was retained for delivery-performance analysis because undelivered orders are still relevant when evaluating delivery status and delays.

---

## Exploratory Data Analysis

Python was used to explore relationships between:

* Delivery delays and customer ratings
* Delivery delays and return rates
* Product categories and return rates
* Customer segments and return rates
* Shipping methods and delivery performance
* Return reasons
* Delivery attempts and customer ratings

The analysis focused on business-relevant questions rather than creating unnecessary visualizations.

---

## Key KPIs

The Power BI dashboard tracks metrics including:

* Total Orders
* Delivered Orders
* Late Delivery Rate
* Average Customer Rating
* Return Rate
* Average Delivery Delay
* Returned Order Value
* Average Delivery Attempts

---

# Power BI Dashboard

The final dashboard contains **three pages**.

## Page 1 — Customer Experience Overview

Provides an overall view of:

* Total orders
* Average customer rating
* Return rate
* Late delivery rate
* Average delivery delay
* Delivery status
* Product categories
* Customer segments
* Shipping methods
* Monthly order trends

The page also contains slicers for interactive filtering.

---

## Page 2 — Delivery Performance

Focuses on delivery-related performance, including:

* Delivery status
* Late delivery rate by shipping method
* Delivery-delay groups
* Average delivery delay
* Late orders by shipping method
* Return rate by delay group

The page helps identify differences in delivery performance across shipping methods and delay levels.

---

## Page 3 — Customer Experience Analysis

Focuses on the relationship between logistics and customer experience.

The analysis includes:

* Average customer rating by delivery-delay group
* Return rate by customer segment
* Return rate by shipping method
* Average rating by shipping method
* Average rating by customer segment

---

# Key Business Insights

### 1. Delivery delays are associated with lower customer ratings

On-time orders had an average customer rating of **4.21**, while orders delayed by more than five days had an average rating of **2.62**.

This indicates a strong relationship between delivery performance and customer satisfaction.

### 2. Delayed orders have higher return rates

The return rate increased from approximately **9.39% for on-time orders** to **24.54% for orders delayed by more than five days**.

This suggests that delivery performance and return behavior are closely associated in the dataset.

### 3. International shipping has weaker delivery performance

International shipping recorded the highest late-delivery rate among the shipping methods analyzed.

This makes international shipping an important area for further operational investigation.

### 4. Premium customers have the highest return rate

Premium customers recorded a return rate of approximately **21.20%**, higher than the other customer segments.

This indicates that Premium-customer returns should be investigated further by product category and return reason.

### 5. Product defects are the most common return reason

Product Defect was the largest recorded return reason, representing approximately **25.32% of returned orders**.

This highlights product quality as an important area for further investigation.

### 6. Electronics represents a major share of returned order value

Electronics accounted for approximately **$787K in returned order value**, making it an important category for deeper return analysis.

### 7. Multiple delivery attempts are associated with lower ratings

Orders requiring three delivery attempts had an average rating of approximately **2.42**, compared with **3.39** for orders completed after one attempt.

Because relatively few orders required three attempts, this finding should be interpreted cautiously.

---

# Business Recommendations

### 1. Improve delivery reliability

Investigate the operational causes of late deliveries, particularly for shipping methods with weaker delivery performance.

### 2. Investigate international shipping

Break international delivery performance down by carrier, destination, warehouse and route to identify specific bottlenecks.

### 3. Reduce product defects

Investigate product defects by category, supplier and warehouse to identify potential quality-control issues.

### 4. Investigate electronics returns

Analyze electronics returns by return reason, shipping method, customer segment and delivery performance to identify the main drivers of returned order value.

### 5. Analyze Premium customer returns

Break down Premium customer returns by product category and return reason to understand why their return rate is higher.

### 6. Improve first-attempt delivery

Investigate the causes of repeated delivery attempts and identify opportunities to improve first-attempt delivery success.

---

# Important Analytical Limitation

The analysis identifies **associations rather than causal relationships**.

For example, delayed orders have lower ratings and higher return rates, but the analysis does not prove that delivery delays directly cause customers to return products.

Further analysis with additional operational and customer-level data would be required to establish causal relationships.

---

# Project Outcome

The project transformed raw e-commerce order data into an interactive **three-page Power BI dashboard** that provides a consolidated view of delivery performance, customer satisfaction and return behavior.

The analysis identified delivery delays, international shipping performance, product defects, electronics returns and Premium-customer returns as areas that warrant further investigation.

---

## Project Structure

```text
E-commerce-Customer-Experience-Analytics/
│
├── data/
│   └── E-commerce_Delivery_Shipping_Data_2026.csv
│
├── python/
│   └── ecommerce_analysis.ipynb
│
├── powerbi/
│   └── ecommerce_customer_experience.pbix
│
├── screenshots/
│   ├── page1_customer_experience_overview.png
│   ├── page2_delivery_performance.png
│   └── page3_customer_experience_analysis.png
│
└── README.md
```

---

## Skills Demonstrated

* Data Cleaning
* Data Validation
* Exploratory Data Analysis
* Python / Pandas
* NumPy
* Data Visualization
* KPI Development
* Business Analysis
* Power BI
* DAX
* Dashboard Design
* Data Storytelling
* Business Recommendations
