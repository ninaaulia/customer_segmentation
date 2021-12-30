# implementing Kmeans for customer segmentation

![image](https://user-images.githubusercontent.com/71708747/147719539-057ca310-dc6d-46f7-adfb-565195d0bce5.png)

## Dataset

Dataset has 9 column with 70864 rows


| Columns       | Description  |
| ------------- |:-------------:|
| Invoiceno     | Number uniquely assigned to each transaction |
| Stockcode     | Number uniquely assigned to each distinct product |
| Description   | Product (item) name |
| Quantity      | The quantities of each product (item) per transaction |
| Invoicedate   | Purchase date |
| Unitprice     | Product price per unit |
| Customerid    | Number uniquely assigned to each customer |
| Country       | The name of the country where a customer resides. |
| Totalprice    | Total price (unitPrice * quantity) |



## Exploratory Data Analysis

![image](https://user-images.githubusercontent.com/71708747/147719457-c75966ee-fe09-44b0-ab8c-eb3c08154804.png)



## Cohort Analysis

![image](https://user-images.githubusercontent.com/71708747/147719568-f584e626-a31c-4267-8b47-f0cd53bbfd60.png)


desc :

* there is an retention rate of 34% for the Cohort Month 2010–12–01, with the highest retention rate occurring after 11 months 49% 
* despite the drop off in Month 12, 30-40% of visitors were still coming back until then.
* the highest retention rate was in the last 3 months (August– October2011).
* For all the other Cohort Months, the average retention rates are around 18–30%.



## RFM 

![image](https://user-images.githubusercontent.com/71708747/147719635-9ef359ab-7399-4a82-aaea-5e3e66e23dfa.png)



## Data Preprocessing 

1.Log tranformation
2.Standard Scaler







* Implement 3 cluster for dataset

![image](https://user-images.githubusercontent.com/71708747/147719690-74e8b0e6-278e-4af3-af88-887631827772.png)

* Snake plot

![image](https://user-images.githubusercontent.com/71708747/147719752-be4cb190-24c7-4b14-ae4a-6644daeea8e0.png)


* Group of The Customers

| Segmentation | Total Customers| Description |
| :- | -: | :-: |
| Champions | 566 |Best customers, who bought most recently, most often, and are heavy spenders. 
| Big Spander | 245 | Customers who spend big amount.
| Potential Loyalists | 492 |Our recent customers with average frequency and who spent a good amount.
| New | 174 | Customers who have a high overall RFM score but are not frequent shoppers. 
| At Risk Customers | 469 |Customers who purchased often and spent big amounts, but haven’t purchased recently. 
| Lost Potential |1230 | Customers who used to visit and purchase quite often, but haven’t been visiting recently.
| Lost  | 525 |Customers who haven't made a purchase for a long time, only make a one-time transaction and spend less.


