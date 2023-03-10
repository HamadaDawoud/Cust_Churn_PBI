<h1>POWER-BI - Analysing Customer Churn</h1>


<h2>Description</h2>
The problem we will be working on is customer churn. You'll be using churn dataset from a Telecom provider . our task is to analyze why customers are churning, or in other words, leaving the company.

Defining churn <br />
A good definition is the one from Investopedia: "The churn rate, also known as the rate of attrition or customer churn, is the rate at which customers stop doing business with an entity." You can compare churn with the leaky bucket problem. You can fill the bucket with more water (or new customers in this case), but your overall revenue won't increase if existing customers are leaving your company. It's easier to retain customers than to attract new customers, so for many companies it's a priority to reduce churn..
<br />


<h2>Language / Technolgies Used</h2>

- <b>PowerBI Desktop</b> 
- <b>DAX Language</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Project Steps:</h2>
1.Check data for duplication to ensure each data row reflects a unique customer in the customer table, will create two measures; one to count cust_id and the other to count dist_cust_id.
 <br/>
 <br/>
<p align="center">
<img src="https://i.ibb.co/16g5Jx3/1.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
<p align="left">
2.Create churned column to convert churn status into binomial for the ease of analysis instead of (yes,no) structure using (IF). Then create a measure with the number of churned_customers to find the churn rate. 
 <br/>
 <br/>
<p align="center">
<img src="https://i.ibb.co/w4KRcY0/2.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
<p align="left">
3.Next a bar chart is created to represented the different reasons that causes customers to churn  
 <br/>
 <br/>
<p align="center">
<img src="https://i.ibb.co/XCvSdPW/3.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
<p align="left">
4. Reasons that cause customers to churn are categorized into four distinct churn categories. For example, reasons related to other competitors, attitude…etc.   
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/zbP8zpN/4.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br/>
The pie chart shows clearly that almost half of all customers churning are related to other competitors
<br />
<br />
 <p align="left">
5. Meanwhile, the competitors launched aggressive promos in certain states, and it’s needed to analyze how those promos is impacting our customers
A map chart is used to visualized the number of churned customers and their percentage of total customers in each state    
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/hDx3QSM/5.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br/>
 The map show that the state of California has abnormally high churn rate (>60%)
<br />
<br />
 <p align="left">
6. The next step is to dig dipper in the analysis and it’s a good way to categorize the data we have and create a metadata table to ease the process of the analysis and help in specifying different analysis dimensions    
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/CM6BkTF/6.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
 <p align="left">
7. According to the findings in the previous step, it is obvious that we need to investigate more on the demographic dimension of our customer data. A new calculated column “demographics” is created to categorize the age of our customers to (Senior, Under-30 & Other) using nested-if function.   
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/XkvQ3rw/7.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
 <p align="left">
8. Analyzing churn customers’ age prevail that senior customers tend to churn more often, that indicate that customer age analysis can lead to more insight about churning. By Binning the customer age column into groups of 5 years.   
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/8j7gM8B/8.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br/>
 It can be seen that the high churn rate in senior customers is mainly derived by the low customer number in this age 
<br />
<br />
 <p align="left">
9.Next we will examine customers with different contract periods into Monthly & Yearly contract category using “Switch function” to identify how the period of contracts affect churn rate.
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/9hjcMjk/9.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br/>
 The graph shows the monthly subscription customers tend to churn more than other long contract customers
<br />
<br />
 <p align="left">
10.International call activity of customers are analyzed for churn rates.   
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/vvNfC15/11.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<img src="https://i.ibb.co/nCHmnNS/10.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
The graph shows that California (state with highest churn rate) also has 72% of people making international calls have no call plan. Those can be potential customers. Also, the churn rate for customers who pay for international plan but don’t call internationally is very high.
<br />
<br />
<p align="left">
B.	Age group dashboard
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/vvNfC15/11.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
<p align="left">
C.	Payments & Contract
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/vvNfC15/11.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
<p align="left">
D.	Extra Charge   
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/vvNfC15/11.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
<p align="left">
At the end; this dashboard highlits the main findings of our analysis that can help in making data-informed decisions   
<br/>
<br/>
<p align="center">
<img src="https://i.ibb.co/vvNfC15/11.jpg" height="80%" width="80%" alt="Analysing Customer Churn"/>
<br />
<br />
 
 
 
 
 
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
