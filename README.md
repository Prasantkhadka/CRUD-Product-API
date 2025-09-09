# CRUD Product API

A simple RESTful API for managing products. Built with Node.js, Express, and MongoDB (Mongoose).

# Features
--> Create a product
--> Read all products
--> Update product details
--> Delete a product
--> Input validation for required fields
--> Error handling for invalid requests and server issues

# API Endpoints
Method	Endpoint	Description
GET	/api/products	Get all products
POST	/api/products	Create a new product
PUT	/api/products/:id	Update a product by ID
DELETE	/api/products/:id	Delete a product by ID
Example Request Body (POST/PUT)
{
  "name": "Laptop",
  "price": 1200,
  "image": "https://example.com/laptop.jpg"
}

# Tech Stack
Node.js – backend runtime
Express.js – server framework
MongoDB – database
Mongoose – ODM for MongoDB

# Setup Instructions:
--> Clone the repository:git clone https://github.com/Prasantkhadka/CRUD-Product-API.git
--> cd CRUD-Product-API
--> Install dependencies:
--> npm install
--> Add a .env file in the root:
--> MONGO_URI=your_mongodb_connection_string
--> PORT=3000
--> Run the server: npm run dev
--> Test API using Postman or cURL.

# What I Learned
--> How to build a REST API using Express with CRUD operations.
--> Mongoose basics: creating models, validating ObjectId, and performing database operations (find, save, findByIdAndUpdate, findByIdAndDelete).
--> Input validation: ensuring required fields (name, price, image) are provided before saving.
--> Error handling: returning proper status codes (400, 404, 500) with meaningful messages.
--> Using .env file securely: keeping sensitive data like database URI hidden with .gitignore.
--> API testing: using Postman to simulate requests and debug responses.
--> Separation of concerns: organizing logic into controller functions instead of putting everything inside app.js.

# Next Improvements
--> Add authentication (JWT) to protect endpoints.
--> Add pagination & filtering for GET /products.
--> Add file upload support for product images.
--> Write unit tests with Jest or Mocha.
