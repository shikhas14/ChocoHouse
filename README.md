**The Chocolate House Database Management System**

This is an even simpler Python script: managements of a
SQLite DB for a chocolate house containing seasonal flavors, the count of ingredients, 
and what say the customers. It supports all sorts of table creation and putting new 
records into an empty table and viewing any and all existing data.

**Requirements**

Open source Eg: Google Collab

Python 3.x

SQLite




**Script Overview**

There are three main tables in the script: 
the seasonal flavors table, the s_f, which helps manage information about various chocolate 
flavor descriptions and the season(s) they are associated with.
Ingredient inventory (i_invent) stores information about the ingredients used in the chocolate 
making process, including name and quantity in stock along with units.
Collects the feedback of customers on flavor preferences and possible allergies 
Customer Feedback (c_f).

**Functions**

1. create_tables()
creates the needed tables, s_f, i_invent, c_f, if they have not been created before in SQLite.
2. add_s_f(flavor_name, description, season)
adds new seasonal flavor in the table s_f.
3. add_in(ingredient_name, quantity_in_stock, unit)
add new ingredient to the i_invent table.
4. add_c_f(customer_name, flavor_suggestion, allergy_concern)
Customer's feedback added in the table c_f
5. view_table(table_name)
print the content in the table
6. close_connection()
end.


**Notes**

The script creates an SQLite database named chocolate_house.db in the current working directory. 
If it already exists, it reuses it.
The script can be extended further by adding more functionality, such as updating or deleting 
records. It could also be even extended to handle more complicated customer feedback or 
manage stock levels.
