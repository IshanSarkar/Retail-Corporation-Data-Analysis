# Detail:
This particular business case focuses on the operations of the Retail store in Brazil and provides insightful information about 100,000 orders placed between 2016 and 2018. The dataset offers a comprehensive view of various dimensions including the order status, price, payment and freight performance, customer location, product attributes, and customer reviews.<br>
**Platform Used: Mysql**

## Business Problem:
By analyzing this extensive dataset, it becomes possible to gain valuable insights into the Company’s operations in Brazil. The information can shed light on various aspects of the business, such as order processing, pricing strategies, payment and shipping efficiency, customer demographics, product characteristics, and customer satisfaction levels.<br>

#### Exploratory analysis:<br>
- **Database Details:** <br>
**Query:**<br>
![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/07bd3088-4175-4625-9221-b233f0041cb7)<br>
**Output:**<br>
![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/72d5283d-dfd6-4cfd-b1cf-62635d5ac2c9)<br>
**Similarly, output of other tables**<br>
![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/baf0afae-6562-4a65-814f-30bc53a6f680)    ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/c048ea9c-50e0-4a57-9330-4b6db06eaa69)    ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/ad6784df-deae-4a2c-b68d-ee07b39ef74f)    ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/3f0e403a-2e64-4865-9035-281606a4b2f4)     ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/b22fdd75-b060-44a3-8c8e-0ae3c7af6972)    ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/bf676bda-cf17-4838-be77-4aff1221c25f)<br>
- **Time range between which the orders were placed** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/17ab861c-aae2-4791-b70a-c850f16a4ccd)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/d1400bd6-b88a-4293-b3e9-65291c78cb1b)<br>
- **Count of Cities & States of customers who ordered** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/245325fc-dc5b-424e-9c10-ae89d5a6fb26)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/55b457de-b5cc-45a2-9818-49599eed02f6)<br>
**Insights:** According to the dataset, the initial order was placed on September 4, 2016, at 15:19:00 UTC, and the final order was placed on October 17, 2018, at 17:30:18 UTC. Customers from 5,812 cities and 27 states placed non-repeated orders between September 4, 2016, at 21:15:19 UTC, and October 17, 2018, at 17:30:18 UTC.<br>
#### In-depth Exploration:<br>
- **Growing trend in the no. of orders placed over the past years** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/dca3cdfb-3c62-4a59-9340-af85f4c0dfa2)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/33b7ce3c-f77e-4955-b911-42547827cf5f)<br>
**Insights:** We can see how many orders have been placed per year from the snapshot, but we cannot compute the percentage rise or compare it year to year because we do not have complete data on orders for the entire years of 2016 and 2018, as some months are missing.
-  **Monthly seasonality in terms of the no. of orders being placed** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/092ca751-6f4f-417b-a4f8-0fb4d280a24b)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/5131e10d-06ae-4143-85df-ab41eba7095e)<br>
**Insights:** December 2016 is missing from the data collection. We can observe that the number of orders increased significantly in October 2016 compared to the previous month, but decreased significantly in December of the same year. Because of the forthcoming holiday season in the country, the biggest number of orders in 2017 was in November, and the lowest number of orders was in January. In addition, except the first quarter of 2017, the second month always has the highest number of orders in that quarter, followed by the third month. 2018 began with the highest number of orders in that year, and the number of orders remained very high throughout the year when compared to the previous year's months. The number of orders was extremely low in September and October of 2018.<br>
- **Frequency of customers placing their orders in a day** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/8c674ba5-b357-4f54-8002-024973720453)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/20d8bf3a-3251-48a2-b319-72a946a9e4cf)<br>
**Insights:** Customers typically place their orders in the afternoon, followed by the night, morning, and dawn.<br>
#### Evolution of E-commerce orders in the region<br>
- **Month on Month no. of orders placed in each state** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/79232531-a135-4626-bce9-ddb32d9815e2)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/566cb611-d2c6-4e3f-891a-8f2ef8dab750)<br>
**Insights:**  The number of orders placed in each state in each month. Also, when compared to the other states, Sao Paulo has the highest number of orders throughout the year, with August 2018 being the peak.<br>
- **Customers distribution across all the states** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/6e3a8fd1-3e7a-447e-8861-9d485f888c78)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/cba8fa75-0b65-4781-9779-ddba5d1883f4)<br>
**Insights:** Most of the customers are from Sao Paulo and the lowest number of customers are from Roraima. Note: COUNT(customer_id), COUNT(customer_unique_id), COUNT(DISTINCT(customer_id)) all of them are showing the same results.<br>
#### Impact on Economy:<br>
- **% increase in the cost of orders from year 2017 to 2018** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/dbaed51a-d20b-4821-8e1a-1b83447fe44e)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/2c2ccf03-4a6a-452c-8def-de3910371d9d)<br>
**Insights:** In 2018, there is an increase of 137% in the cost of orders. So, it could mean several meanings like an indication that the prices of the products being ordered have increased, or that customers are ordering more expensive items. It could also suggest that there is an increase in demand for the products being offered, which is driving up the prices.<br> 
- **Total & Average value of order price for each state** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/974e2c2e-5742-4c59-8d4b-92ac9fecd7b6)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/6c7ba1d2-ddec-4cde-b002-4af6d017da4b)<br>
**Insights:** As per the result, Sao Paulo has the highest Total value of order price which is 5202955.05 and Paraiba has the highest average value of order price which is 191.48. This suggests that while Sao Paulo may have a larger volume of orders, the average value of each order in Paraiba is higher.<br>
- **Total & Average value of order freight for each state** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/9625615a-a7af-4244-b0d3-419da83588b3)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/b51708ae-8cdf-4cad-b4d9-cbe697703fd9)<br>
**Insights:** As per the result, the total cost of shipping or transporting goods for all orders in São Paulo is 718723.07, which is the highest, while the average cost of shipping or transporting goods for each order in Roraima is 42.98, which is the highest.<br>
#### Analysis based on sales, freight, and delivery time.<br>
- **No. of days taken to deliver each order from the order’s purchase date as delivery time and the difference (in days) between the estimated & actual delivery date of an order.** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/9ac77baa-9cab-4660-8e91-dae42a110217)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/fd06d2de-7d07-4ff9-85ae-16a6683b26a3)<br>
**Insights:** In the ‘diff_estimated_delivery’ column, a negative value indicates how many days it took to deliver the order beyond the estimated delivery date, while a positive value means how early the order has been delivered. Time is measured in days.<br>
- **Top 5 states with the highest & lowest average freight value** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/c68a0e47-4826-49c1-9563-c6b15e346e2f)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/6b844ad0-92e8-422e-b989-a871011ec747)<br>
**Insights:** The first 5 rows show the top 5 states with the lowest average freight value arranged in ascending order (SP<PR<MG<RJ<DF), and the last 5 rows show the top 5 states with the highest average freight value arranged in ascending order(PI<AC<RO<PB<RR).<br>
- **Top 5 states with the highest & lowest average delivery time.** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/019427eb-a40c-4eaa-ba8d-95478b4ce863)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/5a9837cf-18ee-4bb9-9592-f06b58d73fea)<br>
**Insights:** The first 5 rows show the top 5 states with the lowest average delivery time arranged in ascending order (SP<PR<MG<DF<RS), and the last 5 rows show the top 5 states with the highest average delivery time arranged in ascending order (PA<AL<AM<AP<RR). Time is measured in days.<br>
- **Top 5 states where the order delivery is really fast as compared to the estimated date of delivery.** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/4fb98912-affb-4b92-a84d-fecf87f33ce0)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/fe18ce18-15ad-4ec4-8c04-1fedb790a10a)<br>
**Insights:** The values in the ‘average_diff_estimated_delivery’ column is in days and arranged in descending order. Therefore, in the state of Acre, orders are delivered 19 days earlier than the estimated delivery date and the whole table shows the top 5 state where the order delivery is really fast<br>
#### Analysis based on the payments:<br>
- **Month on Month no. of orders placed using different payment types.** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/9dcae54c-fe5d-4f5c-845e-5fba07722d36)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/cdf3ba8c-7b80-4ad5-9a72-48f656cb7f70)<br>
**Insights:** This table shows the monthly and yearly numbers of orders made using different payment types. From the table, we can see that most orders are made via credit card, followed by UPI.<br> 
- **No. of orders placed based on the payment installments that have been paid.** <br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/f9e32433-94ea-4b6c-89c4-1c5345409ba7)<br>
  ![image](https://github.com/IshanSarkar/Portfolio/assets/160044904/a8d72b14-7ac0-4a24-a162-31c406240665)<br>
**Insights:** From the table we can conclude that most of the orders have been made in a single installment.<br><br>
### Overall Summary:<br>
The analysis of the provided insights reveals significant trends and patterns in the company's operations, encompassing order dynamics, geographic distribution, pricing strategies, shipping costs, and delivery efficiency. The data spans from September 4, 2016, to October 17, 2018, providing a comprehensive view of the company's performance during this period. Notably, there are some missing data points, particularly in December 2016, which limits the ability to make year-to-year comparisons accurately.<br>

### Business Recommendation:
- Given the observed fluctuations in order volumes across different months, the company should capitalize on peak seasons such as November, coinciding with the holiday season, by implementing targeted marketing campaigns and optimizing inventory management to meet increased demand effectively.
- The significant increase in the cost of orders in 2018 warrants a thorough examination of pricing strategies and product offerings. The company should analyze market trends, competitor pricing, and customer preferences to ensure competitive pricing and maximize profitability.
- With São Paulo consistently leading in order volumes and total order value, the company should prioritize marketing efforts and resource allocation in this region. However, attention should also be given to regions with high average order values, such as Paraíba, to capitalize on potentially lucrative markets.
- Analyzing freight values and delivery times across different states highlights opportunities for optimizing shipping processes and reducing costs. The company should focus on improving delivery efficiency, particularly in states where delivery times are comparatively longer, to enhance customer satisfaction and loyalty.
- Recognizing that most orders are made via credit card, followed by UPI, the company should ensure seamless payment processing and offer incentives or promotions to encourage the use of preferred payment methods.
- Given that most orders are made in a single installment, the company could explore opportunities to introduce flexible payment options, such as installment plans, to accommodate diverse customer preferences and increase order value.
- Identifying states with the fastest and slowest delivery times provides insights into areas for improvement. The company should strive to replicate the efficient delivery processes observed in states like Acre across its operations to enhance customer satisfaction and differentiate itself in the market.










