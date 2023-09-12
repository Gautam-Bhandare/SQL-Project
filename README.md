# SQL-Project

Task Information :
Let us consider a BikeStore company that sells bikes across the country in multiple states along
with the service centers spread across the states.
Consider the below diagram :<img width="799" alt="Screenshot 2023-08-30 at 4 51 57 PM" src="https://github.com/Gautam-Bhandare/SQL-Project/assets/95260147/f849ec93-435e-4114-ac1c-122f0a4db908">

As you can see from the diagram, the BikeStores sample database has two schemas : **sales**
and **production,** and these schemas have nine tables while * indicates PRIMARY KEY in each table
Database Tables :

**sales.stores**
The sales.stores table includes the store’s information. Each store has a store name,
contact information such as phone and email, and an address including street, city,
state, and zip code.

**sales.staffs**
The sales.staffs table stores the essential information of staffs including first name,
last name. It also contains the communication information such as email and phone.
A staff works at a store specified by the value in the store_id column. A store can have
one or more staffs.
A staff reports to a store manager specified by the value in the manager_id column. If
the value in the manager_id is null, then the staff is the top manager.
If a staff no longer works for any stores, the value in the active column is set to zero.

**production.categories**
The production.categories table stores the bike’s categories such as children bicycles,
comfort bicycles, and electric bikes.

**production.brands**
The production.brands table stores the brand’s information of bikes, for
example, Electra, Haro, and Heller.

**production.products**
The production.products table stores the product’s information such as name, brand,
category, model year, and list price.
Each product belongs to a brand specified by the brand_id column. Hence, a brand
may have zero or many products.
Each product also belongs a category specified by the category_id column. Also, each
category may have zero or many products.

**sales.customers**
The sales.customers table stores customer’s information including first name, last
name, phone, email, street, city, state and zip code.

**sales.orders**
The sales.orders table stores the sales order’s header information including customer,
order status, order date, required date, shipped date.
It also stores the information on where the sales transaction was created (store) and
who created it (staff).
Each sales order has a row in the sales_orders table. A sales order has one or many
line items stored in the sales.order_items table.

**sales.order_items**
The sales.order_items table stores the line items of a sales order. Each line item
belongs to a sales order specified by the order_id column.
A sales order line item includes product, order quantity, list price, and discount.

**production.stocks**
The production.stocks table stores the inventory information i.e. the quantity of a
particular product in a specific store.

Note - 
- The dataset is in Txt format, convert into CSV and directly import into Snowflake.
- The table structure is included in the file attachment.
- All the task information is present in a pdf file which includes the task and solution.
