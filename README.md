# SHOPCASE

## Description

An ecommerce store called "ShopCase" has been created which is built with MERN stack, and utilizes third party API's. It aims to provide a convenient and user-friendly experience for local shopkeepers and businesses. Customers can search for products or shops based on their preferences and location, and the platform supports various sorting filters. The user interface is designed to be easy to navigate, and customers can add products to their cart for checkout. The platform will supports multiple payment options, making transactions convenient for users.
The platform will be built using modern web technologies including React, Node.js, Express.js, and MongoDB. The backend will be hosted on AWS and will use AWS Simple Storage Bucket for storing images and Amazon Comprehend for analyzing customer feedback.

### Modules:

here's an overview of the common, manager, and store modules for the Shopcase platform:

## 4.1.1 Common Module:

The Common Module will contain the basic functionalities that are shared by all the other modules. This module will handle user authentication, session management, and database connection. It will also contain utility functions for formatting and validating data. Here are the submodules for Common module:

● Authentication: This Submodule allows users to register, login, and logout.
● Search: This submodule enables users to search for products or shops by
keywords, category, location, etc.
● Cart: This submodule allows users to add/remove products from their cart and
proceed to checkout.
● Payment: This submodule integrates with payment gateways to enable secure
and easy payment options.
● Review: This submodule enables users to rate and review products and shops.
● Notification: This submodule sends notifications to users regarding their
orders, cart updates, and other important events.
## 4.1.2 Manager Module:

The Manager Module will contain functionalities related to managing the shopkeepers, their shops, and products. This module will handle the CRUD (Create, Read, Update, Delete) operations for shopkeepers, their shops, and products. It will also contain functionalities to assign and manage the roles of different users. The manager module will also provide functionalities to generate reports and analytics.
Here are the submodules for Manager module:

● Product Management: This submodule allows managers to add, edit, and
delete products from the shop.
● Shop Management: This submodule enables managers to manage their shop
details, such as name, location, working hours, and contact information.
● Order Management: This submodule allows managers to view and manage
orders placed by customers, such as order status, payment status, and shipping
status.
● Inventory Management: This submodule enables managers to manage their
inventory, such as stock availability and stock updates.
## 4.1.3 Store Module:

The Store Module will contain functionalities related to the customer-facing side of the platform. This module will handle the search functionality for products and shops, shopping cart management, checkout, and payment processing. The store module will also provide functionalities to handle orders and track their status. It will also contain functionalities to handle customer reviews and ratings. Here are the submodules for Store module:

● Shop Listing: This submodule enables store owners to list their shops on the
platform.
● Shop Verification: This submodule verifies the authenticity of the shop and
its products to ensure customer trust.
● Shop Dashboard: This submodule provides store owners with a dashboard to
view their shop's performance, such as sales, revenue, and customer analytics.
● Customer Management: This submodule enables store owners to manage
their customers, such as customer information, order history, and
communication.

The common, manager, and store modules will be interconnected and will work
together to provide a seamless shopping experience to the customers. The common
module will provide the foundation for the other modules, while the manager and
store modules will handle the backend and frontend functionalities, respectively and each of these submodules is essential for the smooth functioning of the platform and provides necessary features to cater to the needs of customers, managers, and store owners.


The shopcase platform will provide the following functions:

● Registration: The platform will allow shopkeepers and businesses to register themselves with their basic information such as name, contact number, email address, and location.
● Login: Registered users will be able to login into the platform using their registered email address and password.
● Profile Management: Users will be able to manage their profiles by updating their information, such as contact number, email address, and location.
● Product Management: Users will be able to add new products to their inventory, update existing product information, and remove products from their inventory.
● Shop Management: Users will be able to create and manage their shops by adding new shop locations, updating shop information, and removing shop locations.
● Search: The platform will provide a search functionality to enable users to search for products or shops by name or category. The search results will be sorted based on relevance, and users will be able to filter the results using various sorting filters.
● Order Management: The platform will allow users to manage their orders by tracking the order status, managing returns and refunds, and generating reports on order history and revenue.
● Payment Gateway Integration: The platform will integrate with a payment gateway to enable users to make secure online payments.
● Review and Rating: The platform will allow users to rate and review products and shops, helping other users make informed purchase decisions.
● Admin Dashboard: The platform will have an admin dashboard to enable the site administrator to manage users, products, shops, and orders, and generate reports on site usage and revenue.
● Customer Support: The platform will provide customer support through a
chatbot or a support email address to address any issues or concerns raised by users.

The user characteristics for the Shopcase platform are:

a. Customers:
● Customers are the primary users of the platform who can browse the products and purchase them.
● They can search for products or shops by name, category or location.
● Customers can create an account and save their delivery address and payment information for quick checkout in the future.
● They can also leave ratings and reviews for the products or shops.

b. Shop Owners:
● Shop Owners can create an account and list their products on the platform.
● They can manage their product inventory, view sales reports, and fulfill customer orders.
● They can also view customer ratings and reviews for their shop and products and respond to customer queries or complaints.

c. Admins:
● Admins are the platform's superusers who have access to all functionalities of the platform.
● They can manage user accounts, verify shop ownership, and moderate
user-generated content such as product listings, ratings, and reviews.
● They can also view platform analytics and generate reports for performance evaluation.

d. Guest Users:
● Guest users are unregistered users who can browse the products and shops on the platform but cannot make purchases or leave ratings and reviews.
● They can create an account at any time during the browsing process to avail of the platform's features.

The Shopcase platform caters to a diverse user base, including customers, shop owners, admins, and guest users. Each user type has a unique set of characteristics, needs, and objectives, and the platform aims to provide a seamless experience for all of them
## Database Seed

* The seed command will create an admin user in the database
* The email and password are passed with the command as arguments
* Like below command, replace brackets with email and password. 
* For more information, see code [here](server/utils/seed.js)

```
npm run seed:db [email-***@****.com] [password-******] // 
```
 
## Install

Some basic Git commands are:

```
$ git clone https://github.com/Shubhanshu-1507/shopcase.git
$ cd project
$ npm install
```

## Setup

```
 Create .env file that include:

  * MONGO_URI & JWT_SECRET
  * PORT & BASE_SERVER_URL & BASE_API_URL & BASE_CLIENT_URL
  * MAILCHIMP_KEY & MAILCHIMP_LIST_KEY => Mailchimp configuration
  * MAILGUN_KEY & MAILGUN_DOMAIN & MAILGUN_EMAIL_SENDER => Mailgun configuration
  * GOOGLE_CLIENT_ID & GOOGLE_CLIENT_SECRET & GOOGLE_CALLBACK_URL => Google Auth configuration
  * FACEBOOK_CLIENT_ID & FACEBOOK_CLIENT_SECRET & FACEBOOK_CALLBACK_URL => Facebook Auth configuration
  * AWS_ACCESS_KEY_ID & AWS_SECRET_ACCESS_KEY & AWS_REGION & AWS_BUCKET_NAME => AWS configuration
```

## Start development

```
$ npm run dev
```

## Simple build for production

```
$ npm run build
```

## Run build for production

```
$ npm start
```


## Languages & tools

- [Node](https://nodejs.org/en/)

- [Express](https://expressjs.com/)

- [Mongoose](https://mongoosejs.com/)

- [React](https://reactjs.org/)

- [Webpack](https://webpack.js.org/)


### Code Formatter

- Add a `.vscode` directory
- Create a file `settings.json` inside `.vscode`
- Install Prettier - Code formatter in VSCode
- Add the following snippet:  

```json

    {
      "editor.formatOnSave": true,
      "prettier.singleQuote": true,
      "prettier.arrowParens": "avoid",
      "prettier.jsxSingleQuote": true,
      "prettier.trailingComma": "none",
      "javascript.preferences.quoteStyle": "single",
    }

```