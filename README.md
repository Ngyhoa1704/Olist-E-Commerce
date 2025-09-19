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
<img width="962" height="465" alt="image" src="https://github.com/user-attachments/assets/5bdfda76-f6af-4c3f-b21d-ff9fe4f81fba" />

The product category analysis shows how Olist’s marketplace is structured and which segments drive sales. Out of 71 categories, the top ten dominate overall performance, with **health and beauty** leading, followed by **watches & gifts, bed & bath, sports & leisure,** and **computer accessories**. These categories together account for a major share of sales, while the remaining long tail of categories adds up to a smaller but still meaningful contribution under “Other categories.” This concentration suggests that Olist’s growth is powered by everyday essentials and lifestyle products, which are in high demand online.

<img width="941" height="542" alt="image" src="https://github.com/user-attachments/assets/e231bf75-6c5c-42d0-a76d-9d78c7c21c6d" />

When we examine product weights, a clear pattern emerges. Lighter products like computer accessories and watches & gifts weigh under 2 kg and are easier to ship, which makes them attractive for e-commerce. On the other hand, categories such as furniture, auto, and housewares are much heavier, often several kilograms, which raises logistics costs and can slow delivery. Despite this, they still contribute significantly to total sales, showing that customers are willing to purchase bulky items online if the platform provides reliable delivery.

Putting these findings together, we see that Olist benefits from a mix of high-frequency, lightweight categories that sustain regular order volumes, and lower-frequency but higher-ticket bulky items that push up overall sales value. This explains why shipping costs, as noted earlier, are usually low for most orders but can spike for certain categories. It also highlights the importance of logistics strategy: controlling shipping for bulky categories could directly improve margins and customer satisfaction, while lighter categories provide steady growth with minimal delivery risk.


### Order Delivery
<img width="585" height="325" alt="image" src="https://github.com/user-attachments/assets/6e341edf-2579-4c16-b125-72f6939ec314" />
<img width="982" height="779" alt="image" src="https://github.com/user-attachments/assets/df5350ed-4c8a-4ad7-a456-f174f291281c" />

Across cities, the approval and handover-to-carrier steps are consistently quick, usually under three days. The variation comes later: in cities close to logistics hubs such as São Paulo, Guarulhos, and São Bernardo do Campo, delivery to customers averages only 5–6 days, while more distant locations like Salvador, Porto Alegre, and Brasília take 10–16 days. The gap is mainly driven by the last mile, not the start of the process.

<img width="969" height="521" alt="image" src="https://github.com/user-attachments/assets/8add1fec-6f94-46e2-9375-c92e5509c9f4" />

Seasonality plays an important role. From mid-2017 to early 2018, delivery times averaged about 13 days, but during peak shopping seasons like Black Friday and Christmas, they spiked above 18–20 days. This shows how surges in order volume create congestion in the logistics network. A postal strike in early 2018 also added delays. After March 2018, however, delivery times improved sharply, falling below 10 days by June. This indicates not only a seasonal recovery but also likely improvements in logistics efficiency after the disruption.

Taken together, the data suggests two main drivers of delivery performance: structural differences between regions (distance to hubs) and temporary surges from demand or external disruptions. For Olist, this means that while the core process is stable, addressing last-mile delivery in distant regions and planning for seasonal peaks are the key levers to reduce delays.

### Order Reviews
<img width="806" height="466" alt="image" src="https://github.com/user-attachments/assets/c13a3450-d46b-4ae7-9c6e-ff6f997bf5ef" />

<img width="927" height="513" alt="image" src="https://github.com/user-attachments/assets/3ffd7e9e-7bab-4492-a6c6-b57ada5ab34c" />

The review data shows a strong positive bias, with over 57,000 reviews scoring 5, far outnumbering lower ratings. This suggests that many customers are satisfied with their experience. However, the distribution also reveals a meaningful share of negative feedback: more than 11,000 one-star reviews and over 8,000 three-star reviews. When we translate the comments tied to low scores, the most common words are variations of “não recebi o produto” (“I didn’t receive the product”), “ainda não chegou” (“it hasn’t arrived yet”), and “entrega atrasada” (“late delivery”). These patterns make it clear that delayed or failed deliveries are the leading source of dissatisfaction, overshadowing complaints about product defects or incorrect items, which appear less frequently.

Taken together with earlier findings on delivery times, this confirms that logistics performance directly shapes customer satisfaction. While Olist has many happy customers, the negative reviews are not random—they reflect recurring delivery issues. This connection highlights a key point for management: improving delivery reliability could sharply reduce one-star reviews and raise overall customer perception, strengthening both trust and retention.

### Customer Segmentation
Now we will use a simple segmentation method such as RFM to identify group of customers according to three metrics:
- Recency: How recently did the customer place the last order?
- Frequency: How often does the customer place orders?
- Monetary value: How much does the customer spend on average?

Afterward, each customer is assigned to a category according to its RFM scores. This segmentation process is particularly useful for personalized marketing to improve customer service by addressing the specific needs of different customer groups.

<img width="505" height="308" alt="image" src="https://github.com/user-attachments/assets/7376863a-51d6-49a8-b1aa-956b54252271" />

<img width="906" height="599" alt="image" src="https://github.com/user-attachments/assets/2580727c-fc32-41fa-b502-930e82daf4e8" />

<img width="487" height="343" alt="image" src="https://github.com/user-attachments/assets/274afcdb-3519-4592-b08e-ee4cfd1f0764" />

The RFM segmentation highlights an important imbalance in Olist’s customer base. While there are clear high-value groups like Champions and Loyal Customers, the majority of customers fall into segments such as Potential Loyalists, Promising, or Recent Users—all of whom have bought recently but have not yet shown consistent repeat behavior. This is supported by the pie chart: only 3% of customers are repeat buyers, while 97% make just a single purchase.

This shows that Olist’s main challenge is not acquiring customers, but keeping them. The Champions group spends heavily and represents the most reliable revenue stream, but it is small compared to the vast pool of one-time buyers. If even a small portion of Potential Loyalists and Recents could be nurtured into Loyal Customers, the overall revenue base would become far more stable. On the other end, groups like Lost and Hibernating represent customers who have disengaged, showing that retention efforts are not yet effective in bringing people back.

When we link this back to earlier findings, especially the delivery and review analysis, the problem becomes clearer: logistics delays are a major reason why many customers don’t return. Reviews show “did not receive product” or “delayed delivery” as the most frequent complaints, which can directly explain why repeat rates are so low. This suggests that retention is not just a marketing issue but also an operational one. By reducing shipping delays and improving reliability, Olist would likely see a natural lift in repeat buyers, strengthening the Loyal and Champion segments.















