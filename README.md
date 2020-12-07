 
# Warehouse Sample API

**How to use this source code**

1. Install XAMPP, and start the Apache and mySQL 
2. Download this source code as zip
3. Extract the zip file in c:\xampp\htdocs
4. Rename the root folder as 'warehouse'
5. Configure the database username & password in file api/config.php
6. Go to PHPMyAdmin, create new database name 'nre'
7. At nre database, run the sql command below: 

```
CREATE TABLE users(
user_id int AUTO_INCREMENT PRIMARY KEY,
username varchar(50),
password varchar(300), 
bahagian varchar(300), 
jawatan varchar(300), 
role varchar(300), 
tel varchar(300), 
name varchar(200), 
email varchar(300)); 


CREATE TABLE inventory(
item_id int PRIMARY KEY AUTO_INCREMENT, 
name varchar(300),
serial_number varchar(300),
description text,
category varchar(300),
category status(300),
user_id_fk int,
created int

); 
```
8. Download and install Postman, make sure you sign up and log in.
9. Open Postman, click on import, then choose ```Warehouse API.postman_collection.json``` in \warehouse folder
10. Run and test API!
