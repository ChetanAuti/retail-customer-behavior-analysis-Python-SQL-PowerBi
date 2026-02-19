📌 Project Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.                                 
The objective is to uncover actionable insights into:                                                                          
•	Customer spending patterns                                                       
•	Demographic-based revenue trends                                                                          
•	Product performance                                                                                             
•	Discount and promotion impact                                                               
•	Subscription behavior                                                                                   
•	Customer segmentation                                                                                                                
The findings are used to support data-driven business decisions.                                                                                           
________________________________________
📊 Dataset Summary                                                                            
•	Total Records: 3,900                                                                          
•	Total Columns: 18                             
Key Features	                                                   
Customer Demographics                                                 
•	Age                                                            
•	Gender                                                                    
•	Location                                                                          
•	Subscription Status                                                                              
Purchase Details                                                                          
•	Item Purchased                                                                                
•	Category                                                                                    
•	Purchase Amount                                                                              
•	Season                                                                              
•	Size                                                                                                      
•	Color                                                                                
Shopping Behavior                                                          
•	Discount Applied                                                        
•	Promo Code Used                                                                                
•	Previous Purchases                                                                              
•	Frequency of Purchases                                                                                    
•	Review Rating                                                                                          
•	Shipping Type                                                                                      
Data Quality                                                                      
•	37 missing values in the review_rating column                                      
•	Missing ratings were imputed using the median rating per product category                          
________________________________________                                                
🧹 Data Cleaning & Preparation (Python)                                                
Exploratory Data Analysis (EDA) and preprocessing were performed using Python.                                
Steps Performed:                                                                          
•	Data Loading: Imported dataset using pandas                                                      
•	Initial Exploration: Used .info() and .describe() for structure and summary statistics                                
•	Missing Value Handling: Imputed missing review ratings                                
•	Column Standardization: Renamed columns to snake_case                              
•	Feature Engineering:                                                    
o	Created age_group using age binning                                            
o	Created purchase_frequency_days                                                          
•	Redundancy Check: Removed promo_code_used after verifying overlap with discount_applied                                                            
•	Database Integration: Loaded cleaned dataset into PostgreSQL for SQL analysis                                    
________________________________________                              
🗄️ Data Analysis (SQL – PostgreSQL)                                                  
Business-focused queries were written in PostgreSQL to answer key analytical questions.                                          
Key Analyses Performed:                                                                              
1.	Revenue by Gender                                                      
o	Compared total revenue generated by male vs female customers.                                  
2.	High-Spending Discount Users                                                                
o	Identified customers using discounts but spending above average.                                                
3.	Top 5 Products by Rating                                                                
o	Ranked products by average review score.                                                                  
4.	Shipping Type Comparison                                                                    
o	Compared average purchase amounts between Standard and Express shipping.                                              
5.	Subscribers vs Non-Subscribers                                                  
o	Compared total revenue and average spend.                                                                            
6.	Discount-Dependent Products                                                                  
o	Identified products most frequently purchased with discounts.                                                          
7.	Customer Segmentation                                                            
o	Segmented customers into:                                                                              
	New                                                                  
	Returning                                                                      
	Loyal                                                    
8.	Top 3 Products per Category                                                              
o	Ranked best-selling products within each category.                                                        
9.	Repeat Buyers & Subscriptions                                                                  
o	Analyzed whether customers with >5 purchases are more likely to subscribe.                                                            
10.	Revenue by Age Group                                                    
o	Evaluated revenue contribution across age segments.                                              
________________________________________                                                    
📈 Dashboard (Power BI)                                                              
An interactive dashboard was built in Microsoft Power BI to visualize insights and support business decision-making.                          
Dashboard Highlights:                                                                        
•	Revenue breakdown by gender and age group                                                                
•	Subscriber vs non-subscriber comparison                                                      
•	Product performance metrics                                                                      
•	Discount impact analysis                                                                        
•	Shipping preference insights                                                                      
•	Customer segmentation view                                                                  
                                                                                              
📷 Dashboard Preview:                                                              
<img width="1306" height="711" alt="Dashboard-02" src="https://github.com/user-attachments/assets/a3077a75-711b-48b0-b4e7-8ccb84d7e682"/>                                      


________________________________________                                          
💡 Business Recommendations                                                                      
Based on the analysis:                                                                    
1.Boost Subscriptions                                                                                                        
•	Promote exclusive benefits for subscribers.                                                                                          
•	Target repeat customers with subscription offers.                                                        
2.Strengthen Loyalty Programs                                                            
•	Incentivize returning customers to move into the “Loyal” segment.                                                                  
3.Optimize Discount Strategy                                                                                                        
•	Balance revenue growth with profit margins.                                                              
•	Identify products overly dependent on discounts.                                                                      
4.Improve Product Positioning                                                                  
•	Highlight top-rated and best-selling products in campaigns.                            
5.Targeted Marketing                                                          
•	Focus marketing efforts on:                                                      
o	High-revenue age groups                                                                    
o	Express-shipping customers                                                          
o	High-value segments                                                              
________________________________________                                                            
🛠️ Tools & Technologies Used                                                            
•	Python (pandas, data cleaning, feature engineering)                                            
•	PostgreSQL (business queries & analysis)                                                      
•	Microsoft Power BI (dashboard & visualization)                                                                    
________________________________________                                        
📁 Project Workflow                                                                          
1.	Data Collection                                                                          
2.	Data Cleaning & Feature Engineering (Python)                                                                
3.	Database Loading (PostgreSQL)                                                        
4.	SQL-Based Business Analysis                                                  
5.	Interactive Dashboard (Power BI)                                                                  
6.	Business Insights & Recommendations                                          
________________________________________                                                              
🎯 Project Outcome                                                                
This project demonstrates:                                                          
•	End-to-end data analysis workflow                                                        
•	Data cleaning & transformation                                                                        
•	SQL-based business intelligence                                                                  
•	Dashboard storytelling                                                                                
•	Strategic recommendation development                                                                  
