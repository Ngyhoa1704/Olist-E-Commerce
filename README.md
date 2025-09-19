# Olist E-Commerce
### Introduction

This project analyzes the **Olist e-commerce dataset**, which contains nearly 100,000 orders placed in Brazil between March 2016 and August 2018. Olist is a marketplace that connects small businesses to larger online retail platforms, allowing sellers from across the country to reach a wider customer base.

The dataset is rich and relational, covering orders, payments, customers, sellers, products, reviews, and geographic information. Using SQL for data extraction and transformation, and Python for visualization, the analysis explores customer behavior, order trends, seller performance, and regional demand.

The database schema reflects the marketplace ecosystem:
- Orders and payments provide transaction details.
- Customers, sellers, and geolocation allow for behavioral and geographic insights.
- Order items and product data give visibility into pricing and assortment.
- Reviews capture customer experience and satisfaction.

The aim is to uncover patterns in purchasing, retention, and regional demand that can inform business strategy. By combining SQL queries for structured analysis with Python for clear visual storytelling, the project demonstrates how data can guide marketplace growth and operational decisions.

<img width="3000" height="2325" alt="image" src="https://github.com/user-attachments/assets/325ab0ab-1c7b-453e-abaf-beb17e334aa6" />

### Number of Orders
<img width="1268" height="603" alt="image" src="https://github.com/user-attachments/assets/8e97ee95-3559-47bd-8112-a00c2a764ce7" />

Order volume grew steadily from 2016 to 2018, with a strong seasonal peak on December 24. This confirms that Olist follows the same holiday-driven demand patterns seen in retail worldwide. For business planning, this means sellers and logistics partners need to prepare for major spikes in late December while maintaining stable service during normal growth periods.

<img width="1240" height="606" alt="image" src="https://github.com/user-attachments/assets/325894bf-de9c-4e8f-adda-d106612e9f39" />

The breakdown by weekday and hour shows that most purchases are made during work hours (10 AM–4 PM), with another smaller push at 9 PM. This pattern connects with the daily life of customers: many shop from their computers during the day and then switch to mobile in the evening. For Olist, this means marketing campaigns and customer service should be timed around these peaks to catch customers when they are most active.

<img width="1280" height="609" alt="image" src="https://github.com/user-attachments/assets/5a862ac7-e2e1-443a-9f1a-71272f081e9e" />

Finally, looking at cities, the majority of orders come from large urban centers like São Paulo and Rio de Janeiro, followed by other major hubs. When we connect this with the time-of-day and weekday findings, it suggests that urban, working-age customers are the main drivers of Olist’s growth. They shop during office hours, spike around holidays, and are heavily concentrated in big cities.

Together, these findings explain Olist’s demand profile: urban customers, weekday daytime activity, and strong seasonal spikes. This shows that both marketing and logistics strategies should focus on major cities, align campaigns with weekday/evening peaks, and prepare well ahead of the holiday rush.

### Order Prices
<img width="332" height="66" alt="image" src="https://github.com/user-attachments/assets/b9a50af5-8f70-4993-97be-036c7159ecbd" />

<img width="932" height="391" alt="image" src="https://github.com/user-attachments/assets/141288a5-6675-494c-a807-1035e2bdbe09" />


The analysis of order prices shows that the average order value is around R$160.58. However, the distribution is not balanced: most transactions are clustered at the lower end, with many products priced below R$500, while a few very expensive purchases reach as high as R$13,664. This long right tail means Olist primarily processes affordable, everyday products, but there is also a small segment of high-value buyers that influence the average upward.

When looking at shipping, most fees stay below R$80, with a peak between R$10 and R$20. While shipping costs are small compared to product prices, they occur with every order and therefore contribute significantly to the total customer spend. The low and predictable shipping costs also suggest that Olist prioritizes keeping delivery affordable, which likely helps drive repeat purchases.

In business terms, these findings highlight two key customer groups: a large base of budget-conscious shoppers and a smaller group of high-spending buyers. For Olist, this creates an opportunity to balance strategies between volume-driven low-cost products and targeted offers for premium customers. At the same time, shipping policies can be used as a lever — for example, offering free delivery above a certain threshold could motivate customers to increase their basket size.

### Product Categories
<img width="937" height="772" alt="image" src="https://github.com/user-attachments/assets/3051d85c-35be-4649-9143-67ce61591eb3" />

<img width="962" height="465" alt="image" src="https://github.com/user-attachments/assets/5bdfda76-f6af-4c3f-b21d-ff9fe4f81fba" />

The product category analysis shows how Olist’s marketplace is structured and which segments drive sales. Out of 71 categories, the top ten dominate overall performance, with **health and beauty** leading, followed by **watches & gifts, bed & bath, sports & leisure,** and **computer accessories**. These categories together account for a major share of sales, while the remaining long tail of categories adds up to a smaller but still meaningful contribution under “Other categories.” This concentration suggests that Olist’s growth is powered by everyday essentials and lifestyle products, which are in high demand online.

<img width="941" height="542" alt="image" src="https://github.com/user-attachments/assets/e231bf75-6c5c-42d0-a76d-9d78c7c21c6d" />

When we examine product weights, a clear pattern emerges. Lighter products like computer accessories and watches & gifts weigh under 2 kg and are easier to ship, which makes them attractive for e-commerce. On the other hand, categories such as furniture, auto, and housewares are much heavier, often several kilograms, which raises logistics costs and can slow delivery. Despite this, they still contribute significantly to total sales, showing that customers are willing to purchase bulky items online if the platform provides reliable delivery.

Putting these findings together, we see that Olist benefits from a mix of high-frequency, lightweight categories that sustain regular order volumes, and lower-frequency but higher-ticket bulky items that push up overall sales value. This explains why shipping costs, as noted earlier, are usually low for most orders but can spike for certain categories. It also highlights the importance of logistics strategy: controlling shipping for bulky categories could directly improve margins and customer satisfaction, while lighter categories provide steady growth with minimal delivery risk.







