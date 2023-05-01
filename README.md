Download Link: https://assignmentchef.com/product/solved-cis336-lab5-joining-tables
<br>



Lab 5 will introduce the concept of multi-table JOINS in order to work with data in two or more related tables simultaneously.  This lab may be completed using either DeVry’s Omnymbus EDUPE-APP lab environment, or a local copy of the MySQL database running on your own computer using the OM database tables. The lab will utilize a set of tables that are represented by the ERD (OM_ERD.docx) and are created and populated by the script file (create_OM_db.sql).  Follow the instructions in the file CreateOMTables.docx to create your database, tables, and data.

A few IMPORTANT things to note if using EDUPE MySQL:

**There can be NO SPACES in alias names given to a column.  For example:

Select unit_price as “Retail Price “ from items;  –this does NOT work in EDUPE MySQL.

Any of the following WILL WORK:

Select unit_price as “RetailPrice” from items;

Select unit_price as “Retail_Price” from items;

Select unit_price as Retail_Price from items;

Select unit_price as RetailPrice from items;

**Any calculated fields MUST be given an alias (and note above NO SPACES in alias).  For example:

select unit_price * 2 from items;   –this does NOT work in EDUPE MySQL

This will work:

select unit_price * 2 as NewPrice from items;

Deliverables

<ul>

 <li>Lab Report (Answer Sheet) containing both the student-created SQL command(s) for each exercise, and the output showing the results obtained. Be sure your name is on the file.</li>

</ul>

LAB STEPS:  Complete each of the exercises below:

1. Use the JOIN ON syntax to write a query to display the order id, order date, customer name formatted as a single field (i.e. “Tom Jones”) with a heading of Customer, and customer_city  for customers residing in the state of OHIO.   Sort the output to display the newest orders first.

2.  Use the JOIN USING syntax to display the order_id, order date, and shipdate for orders to Karina Lacy that have shipped.

3. Use the implicit join syntax (the WHERE clause) to display the last name, city, order date and ship date for all orders shipped in 2012.

4. Use any join syntax EXCEPT NATURAL JOIN to list the customer_first_name and customer_last_name concatenated with an intervening space as Customer, customer city and state formatted as a single column in the format of “city, ST” with a heading of Location, order_id and order date for orders that have not shipped.

5.  List the customer name, order date, zipcode for any customer(s) placing an order for the item titled ‘Etcetera”.

6.  Write a query to list the title and artist of ONLY the items that have been ordered.  Only list each title once.

7.  Write a query to list the title and price of all items that have been ordered by customer Millerton.

8. Write a query to list the last name and order id of customers that ordered any items by the artist Burt Ruggles?

9. Write a query to display a list of titles along  with the artist name., sorted by artist name.

10.  Write a query to display an invoice for order 693 including the title, quanty, price, and a calculated column to display the line item subtotal (quantity times price) with a heading of Subtotal.

11.  Display the order id, last name,  title , and quantity for any items where customers have ordered 2 or more of a particular item in an order.

12. The employees table contains a list of employees of a company. An employee may be managed by another employee. To denote an employee’s manager, the employee_id of the manager is entered into the manager_id field of the employee reporting to that manager. In order to produce a list of which managers supervise which employees, the table may be joined to itself using these two attributes (employee_id, manager_id). This is known as a SELF-JOIN.  Use a SELF-JOIN on the employees table to produce a result containing two columns: the concatenated last_name and first_name of the manager, and the concatenated last_name and first_name of the employee. Label the first-column supervisor, and the second-column employee. Order the output by the supervisor’s last_name and first_name.

13.  Write a query to display the order id, order date, ship date, and customer last name for all SHIPPED orders placed on the internet (no employee id).  Show the most recently shipped orders first.

14.  Write a query that displays the order id, order date, and employee name as a single field labeled Employee for each order that an employee assisted with.

15. Write a query that displays the order id, order date, customer name as a single field labeled Customer for all orders for the sales rep Thomas Hardy, sorted by customer last name.

This is the end of Lab 5.