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
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
