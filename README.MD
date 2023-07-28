**ChocoSmith Chocolate E-Commerce Website**


**Description:**

ChocoSmith is an e-commerce website that specializes in selling a variety of delicious chocolates. This website is built using PHP, HTML, CSS, JavaScript, and MySQL to provide users with a seamless and enjoyable shopping experience for all their chocolate cravings.

**Features:**

1. **User Registration and Authentication:**
   - Users can register and create an account to log in to the website.
   - Secure authentication to protect user data and ensure privacy.

2. **Product Catalog:**
   - Display a wide range of chocolates available for purchase.
   - Products organized into categories for easy navigation.

3. **Product Details:**
   - Each product has a dedicated page displaying detailed information.
   - Customers can view product images, descriptions, prices, and other relevant details.

4. **Shopping Cart:**
   - Users can add products to their shopping cart for later checkout.
   - Real-time updates to the cart to show the total amount and number of items.

5. **Checkout and Order Processing:**
   - Simple checkout process for customers to place their orders.
   - But no payment gateway(s).


**Database:**

Two databases are used for this website:

1. **chocosmith_users:**
   - Contains user-related information.
   - Users' authentication data and personal details.

To create the table, import the `users_table.sql` file provided in the project.

2. **chocosmith_items:**
   - Stores information about the chocolates available for sale.
   - Product details like name, description, price, and stock.

To create the table, import the `products_table.sql` file provided in the project.

**Installation:**

1. Clone the repository to your local server.

```bash
git clone https://github.com/your_username/chocosmith.git
```

2. Create the `chocosmith_users` and `chocosmith_items` databases.

3. Import the table structures:

   - For `chocosmith_users`, run the following command:

   ```bash
   mysql -u your_username -p chocosmith_users < users_table.sql
   ```

   - For `chocosmith_items`, run the following command:

   ```bash
   mysql -u your_username -p chocosmith_items < products_table.sql
   ```

4. Configure the database connection in `config.php`:

```php
// config.php

define('DB_HOST', 'your_database_host');
define('DB_USER', 'your_database_username');
define('DB_PASS', 'your_database_password');
define('DB_NAME_USERS', 'chocosmith_users');
define('DB_NAME_ITEMS', 'chocosmith_items');
```

5. Start your local server (e.g., XAMPP, WAMP, or MAMP) and access the website in your browser.



**Contact:**

For any inquiries or support, please contact us at support@chocosmith.com.
