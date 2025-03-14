# GroupProject_MIST4610
Group NAME: 61608 Group 3 | Database name: ha_group_crn61608

Team Members
Cavanaugh, Rory
Chadha, Jasmine
McNally, Owen
Mulnix, Hayden
Nguyen, Timmy

Problem Discription
Our Starbucks Database is designed to enhance the quality and efficiency of service at our local college coffee shop. It provides a comprehensive view of key operations, including ingredients used in food and beverages, menu offerings, sales transactions, and employee performance. This database enables us to generate valuable insights for improving sales revenue, tracking employee performance, and implementing targeted marketing strategies. With this system, Starbucks management can optimize operations, streamline service, and maximize overall efficiency.

Data Model
This database models Starbucks' operational efficiency by tracking food and drink sales, ingredient usage, and employee performance. Ingredients are linked to both food and drink entities through a many-to-many relationship, as a single ingredient in inventory can be used in multiple food and drink items. This relationship forms the weak entities food_ingredients and drinks_ingredients, which associate each food or drink item with its corresponding ingredients.

For example, both a Caramel Cold Brew and a Caramel Frappuccino contain sugar and caramel. By structuring the database this way, we enable inventory tracking and supply chain analysis, allowing Starbucks to optimize ingredient management.

Similarly, the receipt entity records food and drink transactions, creating a many-to-many relationship between food and drink items and their sales. The weak entities food_sold and drink_sold capture the food or drink ID and the corresponding receipt(s), enabling the analysis of sales frequency and item demand.

Additionally, the receipt entity is linked to employees through a one-to-many relationship, as one employee can handle multiple sales, but each sale is attributed to a single employee. This structure supports performance evaluation by tracking individual employee contributions to sales. This performance data can be used by Starbucks to see which employees are operating most efficiently at certain times of the day. Employee data, including tenure and position, can further be used for workforce analysis.

By leveraging SQL queries from data being stored within this data model, key business insights can be extracted, such as best-selling items, peak sales times, and ingredient consumption patterns, all of which help Starbucks streamline operations and maximize efficiency.

![image](https://github.com/user-attachments/assets/ebc8437b-1a76-47f6-a840-ccb7d5f4d54f)

![image](https://github.com/user-attachments/assets/4fb436af-4015-4729-ba32-88e47b9d4d45)
![image](https://github.com/user-attachments/assets/9b9478fb-07cf-4f6b-ab22-11bae5986419)
![image](https://github.com/user-attachments/assets/89606c8d-4ee1-49b2-80ca-bb1c1ab0f2f4)
![image](https://github.com/user-attachments/assets/ad51ad92-aa4d-4af8-863a-bc33f597594d)
![image](https://github.com/user-attachments/assets/a7d4528e-0cf4-4314-bcb2-b7037d875f15)

1
Query 1 displays the receipt ids, total sale value, date of transaction, time of transaction, and employee ids
![image](https://github.com/user-attachments/assets/f7948507-d7fc-4d0c-a7a8-cf08ed52fecf)
This query provides management insight on transactions during a specified date. Management can analyze how sale price fluctuates throughout the day, as well as the success or failure of certain employees during the day.
2
This query displays the total revenue of the Starbucks
![image](https://github.com/user-attachments/assets/d404ba71-16ac-492d-8c1b-32bac1828d4d)
Management is able to use this query as a flat numerical value to judge their performance, which can be useful on a broad scale.
3
![image](https://github.com/user-attachments/assets/192f9946-fa4e-4db9-8812-f4d4431afac1)
This query lists the foods Starbucks has to offer, order by price in descending order. 

This is helpful to management as they are able to identify which products would generate the most revenue. This allows managers to create target promotions to push high priced item.
4
This query lists each food item offered, and the ingredients included in that food.
![image](https://github.com/user-attachments/assets/0e800dd2-35cd-4f5d-9cc6-020224ac2845)
Managers will be able to use this information to track ingredient usage, and ultimately reduce waste. This could also be used to forecast supply needs, as some ingredients may belong to 10+ items versus another ingredient might only belong to 1 or 2.
Complex Queries
1
This query displays the highest sold food item with the most ingredients.
![image](https://github.com/user-attachments/assets/dabd8285-b895-4662-bdc6-2b3f6e7649e5)
This can be useful for management as they are able to clearly identify which food item is their best seller, but is costing them the most in terms of ingredients usage. This could lead management to search for alternative ingredient options that would allow for less waste and a greater profit margin.
2
This query displays side by side the food versus drink revenue.

![image](https://github.com/user-attachments/assets/21ad0174-ff27-40e5-85d8-dac1ae97ec2b)
By breaking down revenue into food sales and drink sales, it allows management to compare performance between these categories.This query is a simple yet powerful tool for Starbucks management to track sales performance, optimize inventory, and improve marketing strategies by analyzing the contribution of food and drinks to overall revenue.
3
This query displays the drink name and the corresponding total time it has sold
![image](https://github.com/user-attachments/assets/55dd222f-6f03-405b-b954-f0f0d7eaeae8)
By counting the number of times each drink has been sold and organizing the results in descending order, management can quickly identify the most and least popular beverages. This insight helps in menu optimization, allowing decision-makers to determine which drinks should be promoted, discounted, or potentially removed from the menu

4
This query displays the employees name and id as well as how long they have worked at the starbucks and the total sales they have generated.
![image](https://github.com/user-attachments/assets/df438bef-739c-40ad-81da-31d8bf18f0e9)
This query would prove to be beneficial to Starbucks management as it provides valuable insights into employee performance and experience. By displaying each employee's total sales alongside their tenure, managers can assess how experience correlates with sales performance. Employees with longer tenure may be expected to generate higher sales due to their familiarity with products and customer service skills. However, if newer employees are performing equally well or better, it could indicate strong training programs or highlight high-performing individuals who may be suited for leadership roles

5
This query specifically retrieves the total revenue generated by each employee from food sales on March 10, 2024 and ranks them in descending order.
![image](https://github.com/user-attachments/assets/1250e292-fa6d-4769-83d1-c297c6a4096e)
While this specific example is limited to March 10, 2024 the query can be edited to pull up any date of operations. The query also identifies the maximum revenue earned by an employee on a given day, making it a clear easy process to highlight top performers and optimize staffing decisions based on revenue contribution.

6
This query shows the total number of hours worked, sales made, revenue acquired, and average revenue per sale for each hour in a given day.
![image](https://github.com/user-attachments/assets/063acdef-071f-4f00-a9fd-1007464e08f2)
This query would help Starbucks identify peak and slower hours, allowing them to prepare for better staffing and inventory management. By identifying and understanding hourly sales trends, the Starbucks on Alps can optimize scheduling and promotions to maximize revenue.
Database Information
![image](https://github.com/user-attachments/assets/fe4d0ebe-6eb6-4697-a0d4-e07939ca90b8)





















