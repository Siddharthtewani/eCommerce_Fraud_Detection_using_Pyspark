# FIT5202 - Data Processing for Big Data 2024 S2  
## Assignment 2A: Building Models for eCommerce Fraud Detection  

### Due:  
23:55, 20th September 2024 (End of Week 9)  

### Worth:  
15% of the final marks  

---

## Background  
In the dynamic world of eCommerce, **Monash Fashion Corporation (MFC)** has established itself as a leading online retailer of fashion products. While offering a seamless shopping experience, MFC faces significant risks due to increasing fraudulent activities. Traditional fraud detection methods are insufficient to combat sophisticated fraud tactics.  

The company seeks an advanced **real-time fraud detection system** to analyze transaction data, identify suspicious patterns, and mitigate risks efficiently.  

---

## Problem Statement  
Fraudulent transactions, especially **Card-Not-Present (CNP) Fraud**, have caused significant financial and reputational damage. The challenge lies in designing a scalable and efficient real-time solution using **Apache Spark's** data processing capabilities to detect and prevent such fraudulent activities.  

### Example of CNP Fraud Procedure:  
1. A fraudster places an order with a stolen credit card.  
2. The payment is processed, and the order is shipped.  
3. The rightful cardholder disputes the transaction.  
4. The bank reverses the payment, causing a loss to the company.  

---

## Objective  
Develop an advanced fraud detection application using:  
- **Apache Spark MLlib**  
- **Spark Streaming**  

The system should:  
1. Detect fraudulent transactions using machine learning models.  
2. Handle large-scale transaction data efficiently.  
3. Provide real-time visualizations for the operations team.  

---

## Datasets  
1. **category.csv**: Product category information.  
2. **customer.csv**: Customer details.  
3. **product.csv**: Product details.  
4. **transaction.csv**: Sales transaction records.  
5. **browsing_behaviour.csv**: Customers’ browsing activities.  
6. **customer_session.csv**: Relationship between sessions and customers.  
7. **fraud_transaction.csv**: List of identified fraudulent transactions.  

**Metadata**: [Dataset Metadata](https://docs.google.com/document/d/1cbPCTFjqNUk9tdy8HZbLKXh4kj2NHTNp/edit?usp=sharing)  

---

## Tasks  

### Part 1: Data Loading, Transformation, and Exploration (30%)  
1. **Data Loading (7%)**:  
   - Configure a SparkSession.  
   - Define and use schemas to load datasets into PySpark DataFrames.  

2. **Data Transformation (12%)**:  
   - Categorize browsing events into L1, L2, and L3.  
   - Calculate action counts and ratios.  
   - Extract session time of day and enrich with customer info.  

3. **Exploration (11%)**:  
   - Analyze statistics and relationships.  
   - Generate and discuss two meaningful plots.  

### Part 2: Feature Extraction and ML Training (50%)  
1. **Feature Selection (10%)**:  
   - Identify relevant features for fraud detection.  
2. **ML Pipelines (10%)**:  
   - Create pipelines for **Random Forest** and **Gradient-Boosted Trees** models.  
3. **Data Splitting (5%)**:  
   - Split data into training and testing sets.  
4. **Model Training (25%)**:  
   - Train and evaluate the models.  
   - Compute metrics like **AUC**, **Accuracy**, **Recall**, and **Precision**.  
   - Save the best-performing model.  

### Part 3: Customer Clustering (10%)  
- Use **K-Means Clustering** to identify fraudulent customer behaviors.  

### Part 4: Data Ethics, Privacy, and Security (10%)  
- Explore data ethics, privacy, and security in big data processing.  

---
