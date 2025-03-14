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





