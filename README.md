Ecommerce_Follow_Along
Project Overview:- 1.MERN Integration: Full-stack JavaScript development for seamless front-end and back-end communication.

2.REST APIs: Scalable endpoints for managing users, products, and orders.

3.Database Schema: Models for users, products, and orders, optimized for performance.

4.Backend Setup: Efficient routing and middleware handling with Express.js.

5.Authentication: Secure login and role-based access control using bcrypt and JWT.

6.Order Page:- -->Admin: View and manage all user orders. -->Users: Track personal order history and statuses.

7.Product Page: Interactive product catalog with search, filter, and details view.

8.Payment Gateway:Seamless integration with Stripe/PayPal for secure transactions, Handles payment success, failure, and refunds.

### Milestone 2 overview:-
New Feature Added:

-->Login Page: A user-friendly login page has been added, featuring: Email and password validation. A "Show/Hide Password" toggle for enhanced user experience. Error handling for invalid email format and password length. Loading state to indicate the process of authentication. Navigation to a signup page for new users.

-->Technologies Used: React (Frontend) Tailwind CSS (Styling) React Router (Routing) Express.js (Backend) Stripe/PayPal (Payment Gateway)

-->Installation & Setup: Clone the repository. Run npm install to install dependencies. Start the development server with npm start.

### Milestone 3 - Backend Setup and Integration
Overview
In this milestone, you will set up the foundational elements for your backend. You'll organize your backend code efficiently, configure a Node.js server to handle API requests, connect to MongoDB for data management, and implement basic error handling to ensure smooth server operation. By the end of this milestone, your application will be able to handle requests and store data in MongoDB with proper error feedback.

Tasks
1. Backend Folder Structure 🗂️
Create dedicated folders for organizing your backend code. This includes:

routes: Handles routing of incoming requests.
controllers: Contains the logic for handling requests.
models: Defines the structure and schema of your data (MongoDB).
middlewares: Used for functions that run during the request-response cycle (e.g., validation, logging).
utils: Utility functions that may be used across the backend code.
Note: Terms like “middleware” and “utils” will be explored more in-depth as you progress in the course.

2. Server Setup 🖥️
Use Node.js and Express to create the backend server.

Configure the server to listen on a designated port (e.g., 5000 or 3000).

Steps:

Install necessary dependencies like express using npm.
Create an Express app and set up a basic route to ensure your server is running.
3. Database Connection 💾
Integrate MongoDB with your application to store and manage data.
Use the mongoose library to define schemas and models.
Connect the backend server to MongoDB and ensure the connection is successful.
Test database connection by saving a test document or retrieving data from a collection.
4. Error Handling ⚠️
Implement basic error handling to help with debugging and user feedback.
Create a middleware to handle common errors (e.g., 404 for routes that don’t exist, 500 for server issues).
Ensure that error messages are clear and helpful for both the developer and the user.
5. Documentation 📖
Update your README file to reflect the progress you've made in this milestone.
Provide instructions for setting up and running the backend server.
Document key components of the backend, such as how the server is structured, how MongoDB is integrated, and how to handle errors.
Key Features 🛠️
Backend Folder Structure: Organizing your code in a modular and maintainable way will make future development easier.
Node.js Server: Setting up and configuring a server to handle incoming API requests.
MongoDB Integration: Storing and retrieving data from a MongoDB database.
Error Handling: Implementing basic error handling to ensure smooth debugging and user experience.
Expected Outcome
By the end of this milestone, you will have:

A well-structured backend with clear folder organization.
A running Node.js backend server.
A working MongoDB connection for data storage.
Implemented basic error handling for better app stability.
Mentor Guidance
During this milestone, your mentor will guide you through:

Setting up the backend folder structure and files.
Configuring the server and connecting to MongoDB.
Writing and testing error-handling code.
Milestone 4: User Management with File Uploads
This Node.js application demonstrates user creation, file uploads using Multer, and secure password management using bcrypt and JWT.

Features
User Registration: Securely create users with hashed passwords.
File Upload: Upload user avatars with unique filenames.
JWT Authentication: Generate and validate JSON Web Tokens.
Error Handling: Robust error management using a custom ErrorHandler utility.
Technologies Used
Node.js with Express.js
Mongoose for MongoDB
Multer for file uploads
bcrypt.js for password hashing
jsonwebtoken for authentication
Getting Started
Prerequisitesa
Node.js installed
MongoDB instance running
.env file with the following variables:
### Milestone 5 -Adding SignUp Page
Created a Sign-Up Page in React.

Implemented form validation for: Name (required) Email (valid format required) Password (minimum 2 characters) Password Confirmation (must match password)

Used React Router for navigation.

### Milestone 6
Project Overview
Milestone 6 expands on the knowledge gained in previous milestones, focusing on advanced backend development concepts. This milestone emphasizes API design, integration, and optimization while deepening the understanding of database interactions and server performance.

Learning Objectives
Build and document RESTful APIs.
Implement user authentication and authorization.
Explore advanced database operations and optimizations.
Integrate external APIs and manage third-party services.
Optimize backend performance and scalability.
Prerequisites
Completion of Milestone 5 or equivalent backend knowledge.
Familiarity with JavaScript, Node.js, and Express.js.
Understanding of JSON and basic database operations.
Key Topics
Advanced API Design

RESTful principles and best practices.
Structuring APIs for scalability and maintainability.
Versioning and documentation of APIs.
User Authentication and Authorization

Implementing secure authentication mechanisms (e.g., JWT).
Role-based access control (RBAC).
Managing sensitive user data securely.
Database Interactions

Using ORMs like Sequelize or Mongoose for efficient data handling.
Performing complex queries and transactions.
Indexing and optimizing database performance.
Integration with External APIs

Fetching and processing data from third-party APIs.
Handling rate limits and error responses.
Implementing webhooks and real-time updates.
Backend Optimization

Analyzing and improving server response times.
Caching strategies (e.g., Redis or in-memory caching).
Load balancing and horizontal scaling.
Tools and Technologies
Node.js: Backend runtime environment.
Express.js: Framework for building web applications.
MongoDB or PostgreSQL: Database solutions for storage and queries.
Passport.js or Auth0: Authentication libraries.
Redis: Caching for performance optimization.
Postman: For API testing and debugging.
Deliverables
A well-documented, secure RESTful API.
User authentication and role-based access implementation.
Integration with at least one external API.
Demonstration of caching or other performance optimization techniques.
Comprehensive project documentation including setup, usage, and design rationale.
Resources
Node.js Documentation
Express.js Guide
Passport.js Documentation
MongoDB Documentation
Redis Guide
Evaluation Criteria
API functionality and adherence to RESTful principles.
Secure and robust implementation of authentication.
Integration of external APIs with proper error handling.
Use of optimization techniques to improve performance.
Clarity and thoroughness of documentation.
Next Steps
Explore GraphQL for alternative API design.
Learn about microservices architecture and its implementation.
Delve into DevOps concepts for deployment and monitoring.
Milestone 7: User Login Endpoint 🌟
Overview
In this milestone, we created a backend endpoint for user login functionality. The focus was on validating user credentials and securely verifying the encrypted passwords stored in the database.

Key Achievements 🎯
Validated User Credentials: Implemented functionality to accept and process user login requests.
Encrypted Password Verification: Used bcrypt to securely compare hashed passwords stored in the database with the user’s input.
Error Handling: Added robust error handling for scenarios where users are not found or the password does not match.
Why Password Encryption Matters
Protect User Data: Ensures that passwords remain secure even if the database is compromised.
Privacy: Prevents plain-text storage of sensitive information.
Compliance: Meets security standards like GDPR and PCI-DSS.
Prevents Password Theft: Hashing makes it nearly impossible for attackers to reverse-engineer passwords.
How Login Authentication Works 🔑
User Enters Credentials:

The user provides their email/username and password on the login page.
Fetch User Data from Database:

The backend retrieves the user record based on the provided email/username.
If the user is not found, an error is returned: "User does not exist."
Compare Encrypted Passwords:

Hash the user's input password using the same algorithm (e.g., bcrypt).
Compare the resulting hash with the stored hashed password.
Authenticate the user if the hashes match; otherwise, return an error.
Steps Implemented in Milestone 7 📝
Login Endpoint:

Created a backend route to handle user login requests.
Accepted email/username and password as inputs.
Password Validation:

Used bcrypt to securely hash and compare passwords.
Returned appropriate success or failure responses.
Database Interaction:

Retrieved user data from the database based on the input credentials.
Verified if the user exists and validated their credentials.
###Milestone 8
🎯 Milestone 8: Building a Product Card Component & Structuring the Homepage

📌 Objective

This milestone focuses on enhancing the UI by designing a reusable product card component and setting up an organized homepage to display product listings effectively.

🔍 Key Takeaways

Develop a product card component to display essential product details.

Render multiple product cards dynamically using props and mapping.

Create an engaging homepage layout with proper structuring.

### Milestone-9
In this milestone we have:
 Create the form for products

 This form takes multiple product images as input.

 ### Milestone 10: Product Management Enhancements


Milestone 10 focuses on refining the product creation and management process. This includes improving the form submission flow, handling errors effectively, and ensuring a seamless user experience.

Key Features Implemented

Form Submission & Error Handling

Implemented a structured form to capture product details including:

Name

Description

Price

Category

Tags

Stock

Email

Multiple Images

Integrated multiple image selection for better product representation.

Enhanced error handling using try-catch methods to catch and display errors during product creation.

Debugging tools added to log form data before submission for easier troubleshooting.

API Integration

Built a POST endpoint to receive and validate product data.

Used FormData to handle file uploads efficiently.

Sent form data to the backend API, ensuring proper request formatting (multipart/form-data).

Provided real-time feedback to users on successful product creation or errors encountered.

Why Validation & Error Handling?

Ensures only valid data is stored in the database.

Helps users identify and correct input mistakes quickly.

Prevents incomplete or invalid submissions, reducing inconsistencies in the system.

Technologies Used

React.js for frontend UI

Express.js for backend API handling

MongoDB & Mongoose for database storage

Axios for HTTP requests

Postman for API testing

Next Steps & Enhancements

Implement user authentication to restrict product uploads to authorized users.

Develop an admin panel to manage and moderate product listings.

Introduce real-time image preview and editing capabilities.

Optimize database indexing for faster search and retrieval.

Repository & Submission Details

GitHub Repository: [Your Repository Link Here]

Progress Summary: This milestone enhanced the product creation process by improving form submission, adding error handling, and integrating API communication.

Submission: The repository has been updated, and all changes have been pushed successfully.

## Milestone 11: Product Data Integration

# Overview

This milestone demonstrates how to send product data from a backend API to the frontend, retrieve the data, and dynamically display it using reusable product card components. It focuses on improving your understanding of data fetching, API integration, and dynamic UI rendering.

# Features

**API Integration:**

Backend API endpoint that provides all product data in JSON format.

**Frontend Data Fetching:**

A function that retrieves the product data from the backend API.

**Dynamic UI Rendering:**

Product data is dynamically passed to a reusable product card component and displayed in a clean layout.

## Instructions

**Backend:**

Create an API endpoint to fetch product data.
Ensure the endpoint returns a structured JSON response.

**Frontend:**

Write a function to fetch the product data using the API endpoint.
Dynamically map the fetched data to product card components.

**Display:**

Render the product cards in a grid or list format for a user-friendly interface.

### Milestone 12:
### Backend: Creating the Endpoint
Set Up the Route

Create a new route in your backend API that filters products based on the user's email.
Fetch Data from MongoDB

Query the database to retrieve all products associated with the authenticated user’s email.
Send Response

Return the filtered products as JSON to the frontend.

 ### Frontend: Fetch and Display Products
Create a Function to Fetch Products

Use fetch or Axios to call the backend endpoint.
Display the Products Dynamically

Pass the fetched data to a ProductCard component for rendering.

### Milestone 13: Updating Data in MongoDB

📌 Objective

In this milestone, we will implement an update feature for our application. This will include:

Creating an endpoint in the backend to update data in MongoDB.

Adding an "Edit" button to the product card in the frontend.

Pre-filling a form with existing product details when the edit button is clicked.

Allowing users to modify the data and save changes.

 Backend: Implementing Update Endpoint

Step 1: Define the Update Route

In your Express server, create an endpoint that will handle update requests.
Step 2: Connect Endpoint to MongoDB

Ensure your database connection is set up in server.js or app.js.
Step 3: Add an Edit Button to Product Card

Modify your product card component to include an "Edit" button.

### Milestone 14: Deleting Data from MongoDB

🎯 Objective

In this milestone, we will implement a DELETE operation in MongoDB using an API endpoint. We will also integrate a delete button in the frontend to allow users to remove data from the database by sending the product ID to the backend.

📌 Steps to Implement
Create the Delete EndpointFrontend Implementation

Add a Delete Button

Modify your product card component (e.g., ProductCard.js) to include a delete button
✅ Summary

Created a DELETE API endpoint in Express to remove a product by ID.

Added a delete button in the frontend to call the endpoint.

Ensured that the backend and frontend interact correctly to delete data.

This milestone provides a detailed understanding of handling DELETE operations in a full-stack application.


### Milestone 15: Creating a Responsive Navbar

Overview

In this milestone, we will create a new Nav component that includes navigation links to all major pages of the application. The navbar will be designed to be responsive, ensuring a smooth user experience across different screen sizes. The Nav component will be added to all pages for seamless navigation.

Steps to Complete Milestone 15

1. Create the Nav Component

Inside the components folder, create a new file named Nav.js (or Nav.jsx if using React with JSX syntax).

Define a functional component that contains navigation links to:

Home

My Products

Add Product

Cart

Use the Link component from React Router (if applicable) to enable navigation between pages.

2. Style the Navbar for Responsiveness

Use CSS or a styling framework (e.g., Tailwind CSS, Bootstrap) to ensure the navbar adapts to different screen sizes.
3. Add the Nav Component to All Pages

Import and include the Nav component in each page’s layout.

### Milestone 16: Product Page and Add to Cart
We have created a new page that displays all the product data.

Fetched product details (name, price, image, description, etc.).
Display them in a structured layout.
Added -Add quantity selection and "Add to Cart" button to each product.

Include an input field or buttons for selecting quantity.
Ensure the "Add to Cart" button updates the cart with the selected quantity.

### Milestone 17: Cart Functionality
📌 Overview
In this milestone, we enhance our application by implementing a cart feature where users can store selected products.

In Milestone 17, we implemented a cart functionality by modifying the User Schema and creating a Cart Schema to store product details. We also built an API endpoint to receive product data and save it in the cart. This allows users to add products to their cart, ensuring the data is persistently stored in the database.

###  Milestone 18
### Milestone 18 📝

1. Create a Backend Endpoint for Cart Page

We need to create an API endpoint that allows the frontend to fetch the cart items for a specific user.

2. Implement the Endpoint Logic

Retrieve the user's email from the request.

Query the database to fetch all products inside the cart associated with that user.

Return the cart data as a JSON response.

3. Test the Endpoint

Use tools like Postman or cURL to send requests and verify that the correct data is returned.


### Milestone 19:
In this milestone, we have implemented a cart page that displays the products added to the cart using the backend API from Milestone 18. Each product in the cart has an option to increase or decrease its quantity using + and - buttons. When a user interacts with these buttons, the frontend calls newly created backend endpoints to update the product quantity in real time. The backend includes two endpoints: one to increase the product quantity and another to decrease it, ensuring that the quantity does not go below one. This milestone enhances the user experience by allowing seamless cart management and provides a smooth and interactive shopping experience.

### Milestone 20
In this milestone, we have implemented a backend endpoint that retrieves all user data and sends it via email. Additionally, we have created a frontend profile page that displays the user's profile photo, name, and email in one section, while another section lists their saved addresses. If no addresses are found, the page displays a message stating "No address found." To enhance usability, we have also included an "Add address" button, allowing users to easily manage their addresses. This milestone helps in understanding how to structure and display user profile data efficiently while integrating backend functionality for data retrieval and communication.


### Milestone 21
In this milestone, we will create a frontend form to collect user address details. The form will capture:

Country
City
Address Line 1
Address Line 2
Zip Code
Address Type
Features
A dedicated address form page.
State management to store user input.
Navigation from the profile page when the "Add Address" button is clicked.

### Milestone 22

In this milestone, we have created an endpoint in backend that stores the address inside user profile in database. The endpoint receives the address from address form in front and adds the address to the address array inside the user collection.

### Milestone 23
In this milestone, we will add a "Place Order" button inside the cart page, which navigates to a Select Address page where users can choose a delivery address. The backend will provide an endpoint to fetch user addresses, and we will create a Mongoose schema to store order details, including user ID, selected address, cart items, total price, and order status. This feature ensures a smooth checkout experience and sets the foundation for order management in the system.

### Milestone 24
In this milestone, we will create an Order Confirmation Page to display the ordered products, selected delivery address, and total cart value. The page will include a "Place Order" button at the bottom to finalize the purchase. This step enhances the user experience by providing a clear summary before confirming the order

###  Milestone 25 - Place Order Button

## Overview

In this milestone, we implemented a "Place Order" button on the cart/checkout page. Clicking the button logs "Order Successful" in the console.

## Key Features

Added a "Place Order" button.

Implemented a click event to log "Order Successful" in the console.

## Testing Steps

Navigate to the cart/checkout page.

Click the "Place Order" button.

Open the browser console and check for the message "Order Successful."

### Milestone 26 - Creating a GET Route in order.js

## Overview

In this milestone, we created a GET route in order.js to fetch order details from the backend.

## Key Features

Implemented a GET route in order.js.

Allows retrieval of order data via API.

Lays the foundation for displaying user orders in the frontend.

## Testing Steps

Start the backend server.

Send a GET request to the order endpoint using Postman or a browser.

Verify that order details are returned as a response.

### Milestone 27: My Orders Page  

## Overview  
In this milestone, we created a My Orders page for our frontend. This page fetches and displays all user orders by sending a GET request to the my-orders endpoint using the user’s email.  

## Learning Goals 🎯  
- Implement a frontend page to display user orders.  
- Send a request to retrieve order data from the backend.  
- Integrate the My Orders page into the navbar for easy access.  

## Implementation Steps 📝  
1. Created a My Orders page.  
2. Sent a GET request to fetch user orders using their email.  
3. Displayed the retrieved orders on the page.  
4. Updated the navbar to include the My Orders page for better navigation.  

### Milestone 28: Cancel Order Feature  

## Overview  
In this milestone, we enhanced the My Orders page by adding a Cancel Order button and implemented a backend endpoint to handle order cancellations.  

## Learning Goals 🎯  
- Enable users to cancel placed orders.  
- Implement order cancellation logic in the frontend and backend.  
- Prevent the cancel button from appearing for already canceled orders.  

## Implementation Steps 📝  
1. Added a Cancel Order button for each order in the My Orders page.  
2. Ensured the button is hidden for already canceled orders.  
3. Created a backend endpoint to receive an order-id, find the order, update its status to canceled, and save the changes.  

  


### Milestone 29 - PayPal Integration (Setup)

In this milestone, we set up PayPal for online payments. First, create a PayPal developer account and log in to the PayPal Developer Dashboard. Navigate to Sandbox Accounts, create an account if needed, and save the User ID. Next, obtain and save your Client ID from the sandbox account. Update the order confirmation page to include two payment options: Cash on Delivery (COD) and Online Payment (PayPal). Implement radio buttons to toggle between these options, ensuring the PayPal button appears when Online Payment is selected. In the next milestone, we will integrate the PayPal payment buttons into the application.

### Milestone 30 - Using paypal api & Integrating Online Payments
In this milestone we have downloaded npm package called react-paypal-js that will provide an component called PayPalScriptProvider which will display online payment methods like credit or debit card etc.

Implemented online payment using PayPal API using the client key you created earlier.



### Milestone 31: Global State Management with React-Redux
In this milestone, we integrate Redux for state management in a React project. First, install react-redux using npm install react-redux. Next, create a store folder containing store.js and userActions.js. Inside store.js, configure a Redux store with a userReducer function to manage the user's email state. In userActions.js, define a function setEmail to update the global state with the user's email. Finally, in index.js, wrap the App component with the Provider component, passing the store as a prop to enable global state management across the application.

### Milestone 32 : Using Redux For Global State Management
In this milestone, we have used dispatch method to store the mail in inside the global state.
In all the remaining pages acc the mail stored in global state using useSelector


### Milestone 33: Creating an JWT token and store them inside an cookie.
In this milestone, we have downloaded jsonwebtoken package using NPM.
Used sign method to create an JWT token with mail and ID.

Gave maxAge to set expire time.

Added the cookie inside the response that helps you to store the cookie inside browser.

### Milestone 34:
Get the token from the browser cookie and send it to the server
In backend write an middleware function to validate that JWT token
In every page make sure that this steps will happen so that user cannot go to that page with out login

### Milestone 35:
Making sure that both frontend and backend were correctly deployed and working properly.

