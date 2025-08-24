#  Customer Segmentation using RFM Analysis

This project performs **customer segmentation** using the **RFM (Recency, Frequency, Monetary)** model. It helps businesses identify customer groups such as **Best Customers**, **Loyal Customers**, and those who **Need Attention**, enabling targeted marketing strategies.

---

##  Project Overview

Customer segmentation is a key step in understanding customer behavior and improving business performance.  
In this project, we:

1. **Load and preprocess transaction data**  
   - Remove missing Customer IDs  
   - Keep only positive purchase quantities  
   - Calculate **Total Price = Quantity × UnitPrice**

2. **Compute RFM metrics**  
   - **Recency (R):** Days since the last purchase  
   - **Frequency (F):** Number of transactions  
   - **Monetary (M):** Total spend by each customer  

3. **Assign RFM Scores**  
   - Use **quartile-based scoring** (1–4 scale)  
   - Reverse scoring for Recency (lower days = better)  
   - Sum R, F, and M scores to get a **total RFM score**

4. **Segment Customers**  
   Customers are grouped into segments based on RFM score:
   - **Best Customers** → RFM Score ≥ 9  
   - **Loyal Customers** → RFM Score ≥ 8  
   - **Potential Loyalist** → RFM Score ≥ 5  
   - **Needs Attention** → Otherwise  

5. **Visualize Results**  
   - Distribution of segments using bar plots  
   - Correlation heatmaps of R, F, and M metrics  

---

## 📂 Project Structure
