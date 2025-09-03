# 📊 Analyze operation performance at Adventureworks - bicyle manufacturer with Power BI

![image](https://github.com/user-attachments/assets/61d18000-d346-45a7-a424-a1e9b2f43735)


Author: Huỳnh Như Yến  
Date: 19/6/2025 <br>
Tool Used: Power BI

---
## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Modeling](#-dataset-description--data-structure)   
3. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
4. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---
## 📌 Background & Overview
### 📖 What is this project about? 
The project aims to analyze the manufacturing operation of a bicycles producer - Adventure Works Cycles. The objective is:
- report general operation of plants
- analyze production efficiency of plants
- analyze the output quality 

### 👤 Who is this project for?  
✔️ Production managers <br>
✔️ Data analysts & business analysts <br>
✔️ Recruiters

###  ❓Business Questions:  
The project aims to solve questions: <br>
- production efficiency of manufacturing process
- output quality of manufacturing process

### 🎯Project Outcome:  
Here are insights after the analysis: <br>
✔️ During the period of 2011-2014, the company successfully increased the annual output quantity, boosting the utilization rate of capacity. <br>
✔️ All production locations meet the target production cost for all products. <br> 
✔️ Subassembly and Final Assembly have really high overdue days.

---
## 📂 Dataset Description & Data Modeling
#### Dataset Description
Dataset is a part of AdventureWork2019 database retrieved from Google BigQuery. 

Dataset is of manufacturing department. It includes data about products, components of final products, production plants, production time and cost, output quantity, and scrap information.

It contains 2 fact tables and 7 dimension tables.

- 2 fact tables: WorkOrder and WorkOrderRouting
<img width="600" alt="image" src="https://github.com/user-attachments/assets/f4c07d18-620d-411f-9790-8c9c2cc448f2" /> 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/851ac2e2-8792-4154-8775-1cdcd09ca5d5" />

- 5 dimension tables:
<img width="600" alt="image" src="https://github.com/user-attachments/assets/22da4fef-1c31-4e7f-a15f-b089b6134287" /> 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/949e9339-2823-4250-9ea8-1db80b7a7802" /> 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/11d6d11a-665c-4c8e-b5b5-3184bed2236e" /> 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/ac259bb3-d17c-4884-aff6-8f3071aa9ee5" /> 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/ae183fac-3502-40ce-933e-a8184ada052b" /> 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/c05298ae-7c8b-40b6-abb3-e84cba79978b" /> 



#### Data Modeling
DimDate is a custom date table created by the author.

<img width="600" alt="image" src="https://github.com/user-attachments/assets/00c554f2-7953-4730-b578-e52cb702bdd0" /> <br>

Table relationships:

<img width="600" alt="image" src="https://github.com/user-attachments/assets/86e2f79f-1ede-48b7-820e-d84dd6bb252a" />

---
## 📊 Key Insights & Visualizations
#### Layout 1: Production overview
![project 3 layout 1_page-0001](https://github.com/user-attachments/assets/c0a028bf-0fe2-4c02-a60c-1c82c9fbb6a7)

Key insights as of 6/2014: <br>
✔️ During the period of 2011-2014, the company successfully increased the annual output quantity, boosting the utilization rate of capacity. <br>
✔️ Operating hours in 6/2014 have dropped significantly to only 7,300 hours, leading to the lowest utilization rate since the beginning of 2014.<br>
✔️ Cycle time in 6/2014 also rises to the highest level at 1.68 days per product. It means that it takes longer to finish a product in comparison to previous months.

#### Layout 2: Production efficiency analysis
![Layout 2_page-0001](https://github.com/user-attachments/assets/d6393931-c01e-483f-9f2c-a6d191a4a273)

Key insights as of 6/2014: <br>
✔️ All production locations meet the target production cost for all products. <br>
✔️ Paint, Debur and Polish and Specialized Paint locations have the highest cycle time at 18, 16.7 and 14.8 days respectively. <br>
✔️ Subassembly and Final Assembly have really high overdue days at 8000 and 7000 days.


#### Layout 3: Quality control analysis
![Layout 3_page-0001](https://github.com/user-attachments/assets/93aeae3b-c3ca-4b54-b087-7cb4b60e5fc4)

Key insights as of 6/2014: <br>
✔️ The scrap rate increases in this month to 0.26%. <br>
✔️ 100% scrap products come from Subassembly location. <br>
✔️ 0.03% of products in Subassembly does not meet quality standards. The top three scrap reasons are Stress test failed, Primer process failed and Drill size too small.

---
## 🔎 Final Conclusion & Recommendations
- Output quantity in 6/2014 drops significantly, leading to lower utilization rate of production capacity. <br>
👉👉👉 The company should boost the output quantity in the next period to utilize the idle capacity and lower cost per unit.
- So far, all production plants meet the target cost which is a really good performance. <br>
- Subassembly and Final Assembly often miss the target finish date. <br>
👉👉👉 The managers should either revise the production plan to reflect the reality or fix procedures to meet the target.
- All scrap products of 6/2014 are from Subassembly. <br>
👉👉👉 Technical teams should inspect procedures of this plant, especially checking the stress resistance, primer and drill size of products.
