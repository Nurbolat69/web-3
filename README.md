# Assignment 3 – MongoDB CRUD API

## Project Overview

This project is a backend application built with **Node.js**, **Express**, and **MongoDB**.
It is an evolution of Assignment 1, where local JSON storage was replaced with a **MongoDB database**.
The application provides a fully functional **CRUD REST API** and a simple front-end interface to interact with it.

The chosen topic for this project is **Products**, which aligns with the Final Project requirements.

---

## Technologies Used

* Node.js
* Express.js
* MongoDB
* Mongoose
* HTML / JavaScript
* Postman (for testing)

---

## Project Structure

```
project/
│── server.js
│── models/
│   └── Product.js
│── public/
│   └── index.html
│── package.json
```

---

## Database Schema

**Product Object**

* `name` (String, required)
* `price` (Number, required)
* `category` (String, required)
* `createdAt` (Timestamp)
* `updatedAt` (Timestamp)

---

## API Endpoints

### Create a Product

**POST** `/products`
Creates a new product in MongoDB.

### Get All Products

**GET** `/products`
Retrieves all products from the database.

### Get Product by ID

**GET** `/products/:id`
Retrieves a single product by its MongoDB ID.

### Update Product

**PUT** `/products/:id`
Updates an existing product.

### Delete Product

**DELETE** `/products/:id`
Removes a product from the database.

---

## Validation & Error Handling

* All required fields are validated on POST and PUT requests
* Appropriate HTTP status codes are used:

  * `201 Created`
  * `400 Bad Request`
  * `404 Not Found`
  * `200 OK`

---

## Front-End Interface

A simple HTML interface is provided to:

* View all products
* Add new products using a form

The frontend communicates with the backend using the Fetch API.

---

## Testing

All API endpoints were manually tested using **Postman** to ensure correct interaction with MongoDB.

---

## How to Run the Project

1. Install dependencies:

```bash
npm install
```

2. Start MongoDB (local or MongoDB Atlas)

3. Run the server:

```bash
node server.js
```

4. Open in browser:

```
http://localhost:3000
```

---

## Conclusion

This project demonstrates the use of MongoDB with Express to build a scalable CRUD API.
The structure and logic are designed to be easily extended for the Final Project.

