**Creating E-commerce website in PHP**  **Project Proposal**

Jessie Lan

April 27, 2020


# Executive Summary

## Summary

This project is using PHP interacts with MySQL databases to develop an online shopping cart web application. This online shopping cart system is to create a user-friendly website to sell products online and help business to run an online store. People from anywhere can buy products online. And admin can monitor the activity of the users and checks the online transactions. This PHP shopping cart website has functionalities like retrieve product information (example: name, price, photos) from the MySQL database, create product gallery for the shopping cart from the MySQL database, add/remove/ cart actions, manage cart items using the PHP session, submit orders, and log in/log out/registration/reset password forms that interacts with MySQL databases.

On the one hand, this website can benefit my online shopping store business. This website can not only expand my online business and boost the online sales significantly, but also saving my budget and time. PHP requires no download or licensing fees. And PHP&#39;s easiness and availability can lower the threshold for career entry. What&#39;s more, PHP code is flexible, integrative, and less time-consuming. PHP can ensure quick turnaround time with its fast data processing features. Adding PHP code to HTML can provide a good performance and help to retain customers.

On the other hand, this website can also bring benefits to customers. With these functionalities, users can see what product we have clearly and make a purchase online easily without going to a retailer store in person. This website allows customers to shop their desired products virtually, which makes their shopping experience more convenient.

## Outlines of business justifications and benefits

1. Easy to use
2. Cost efficient
3. Flexible
4. Integrative
5. Less time-consuming
6. Secured
7. Convenient
8. Attract more customers and boost its sales

# Database Design

I used XAMPP Control Panel to connect with my local MySQL database. As you can see in appendix 1.1, I have my local database named store with three tables: items, users, and users\_items. Details are listed as the following:

1.
## items table:

This table stores information for item id, item name, price and image. The primary key is id. The output of this table with the screenshot is shown in appendix 1.2. The types of attributes in tables are shown in appendix 1.3.

1.
## Users table:

This table stores user information like user id, user name, user email, password, contact, city, and address. Users can register on the forms that interact with MySQL database. After user register on the website, user information will be stored in MySQL database. Users are also able to log in with these information on the website. The primary key is id. The output of this table with the screenshot is shown in appendix 1.4. The types of attributes in tables are shown in appendix 1.5.

1.
## Users\_items table:

This table is to store status of items in the user&#39;s shopping cart. It contains id, user id, item id, status. For example, we can see the user with which user added which item to his shopping cart, or which user confirmed his order of which item to his shopping cart. The primary key is id. The output of this table with the screenshot is shown in appendix 1.6. The types of attributes in tables are shown in appendix 1.7.

#

# Web Application Design

1.
## Web Application Design Description

I used PHPStorm to write this project web application code and connect PHP with MySQL database. I have my localhost server to store files included php, css, java script and images. My Path is localhost/store/.

This website used bootdtrap css, fonts, and java script to design its style. I also added style.css file to design its navigation bar, banner image, banner content, footer, and other layouts.

When a user enters the website&#39;s index page, a welcome page with a welcome message shows up. A user can start to shop from the welcome page by clicking &quot;Shop Now&quot; button or those three images on the bottom of this page. It will connect with users to the product page. In products.php page, a user can view different types of products with its name, image, and price from &quot;items&quot; table in MySQL database. A user must need to sign in to his account in order to click &quot;buy Add to cart&quot; button and save product into the shopping cart. The website will ask users to log in account or register a new account if a user hasn&#39;t logged in yet. In the cart page, a user can see his saved items in the shopping cart. He can see the item number, item name, and price on this page. He can also choose to remove items in his shopping cart by clicking &quot;remove&quot; link, or confirm his order by clicking &quot;confirm order&quot; button. After confirming the order, a confirmation message will prompt up and information will be store in the table &quot;users\_items&quot; in MySQL database.

1. Welcome Page: index.php (Appendix 2.1 &amp; 2.2)
2. Products Page: products.php (Appendix 2.3 &amp; 2.4)
3.
## Cart page: cart.php (Appendix 2.5)

# Technical Design

1.
## Technical Design Description

I used PHPStorm to write this project technical design code and using PHP sessions to implement the technical design.

When a user enters the website&#39;s index page, a welcome page with a welcome message shows up. A user can sign up for a new account in &quot;sign up&quot; link on the right corner, it will connect user to a sign-up page. In the sign-up page, a user needs to enter his name, email, password, contact, city, and address information. If a user enters these attributes in a correct type and it&#39;s verified, this information will be used to store data in &quot;users&quot; table in MySQL database for the future usage. And &quot;User successfully registered&quot; message will prompt up. If not, it will prompt up an error message. For example, on appendix 3.2, the password should be at least for 5 characters. If a user enters 4 characters, an error message will show up. A user can log out his account in log out page and &quot;You have been logged out.&quot; Message will prompt up. After registered, a user can log in his account by entering his username and password in log in page. If a user types his username and password correctly, he will be redirect to the product page (See appendix 3.9). If a user doesn&#39;t type the username and password correctly, he cannot log in his account. An error massage will prompt up (See appendix 3.8). On the settings.php page, a user is able to change his password by correctly entering the old password and enter the new password twice, it will prompt a successful message (see the example in appendix 3.6). otherwise, it will prompt an error massage (See the example in appendix 3.5).

All information typed into the php forms will store information in the MySQL database(See Appendix 3.9 &amp; 3.10).

b. Registration form: signup.php (Appendix 3.1 &amp; 3.2)

c. Log Out form: logout.php. (Appendix 3.3)

d. Settings form: settings.php (Appendix 3.4 &amp; 3.5 &amp; 3.6)

e. Log In form: login.php (Appendix 3.7 &amp; 3.8)

# Link to your Implemented Solution

All files can be founded here: [http://oit2.sps.nyu.edu/~jl11190/store.zip](http://oit2.sps.nyu.edu/~jl11190/store.zip)

Download and unzip this file into your localhost. (C:\xampp\htdocs\store) or any web server.

Then use XAMPP to connect with your MySQL database.

Create tables in MySQL and import store.sql file in the database folder.

Set up PHP connection to connect your host with MySQL database.

 
