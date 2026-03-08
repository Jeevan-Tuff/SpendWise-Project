# 💸 SpendWise Backend API

A simple **backend REST API project** built using **Node.js, Express.js, MongoDB, and JWT Authentication**.
This project helps beginner developers understand how real backend systems work with **authentication and CRUD operations**.

---

## 🚀 Project Overview

**SpendWise** is a beginner-friendly backend application designed to demonstrate:

* 🔐 Secure **User Authentication using JWT**
* 📦 **REST API development**
* 💾 **MongoDB database integration**
* ⚙️ **CRUD operations for transactions**
* 🛡️ **Protected routes using middleware**

This project is ideal for students learning **Node.js backend development**.

---

## 🛠️ Tech Stack

| Technology                 | Purpose                             |
| -------------------------- | ----------------------------------- |
| 🟢 Node.js                 | JavaScript runtime for backend      |
| 🚂 Express.js              | Backend framework for building APIs |
| 🍃 MongoDB                 | NoSQL database                      |
| 🔗 Mongoose                | MongoDB object modeling             |
| 🔐 JWT                     | Authentication and authorization    |
| 🔑 bcryptjs                | Password hashing                    |
| 🌐 CORS                    | Cross-origin resource sharing       |
| ⚡ Thunder Client / Postman | API testing                         |

---

## 📁 Project Folder Structure

```
SpendWise
│
├── models
│     ├── User.js
│     └── Transaction.js
│
├── controllers
│     ├── authController.js
│     └── transactionController.js
│
├── routes
│     ├── authRoutes.js
│     └── transactionRoutes.js
│
├── middleware
│     └── authMiddleware.js
│
├── config
│     └── db.js
│
├── .env
├── server.js
└── package.json
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```
git clone https://github.com/YOUR_USERNAME/SpendWise.git
```

---

### 2️⃣ Navigate to Project Folder

```
cd SpendWise
```

---

### 3️⃣ Install Dependencies

```
npm install
```

---

### 4️⃣ Create Environment File

Create a `.env` file in the root folder:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

---

### 5️⃣ Start the Server

Development mode:

```
npm run dev
```

Normal start:

```
npm start
```

Server will run on:

```
http://localhost:5000
```

---

## 🔑 API Endpoints

### 👤 Authentication APIs

#### Register User

```
POST /api/auth/register
```

Example Body:

```
{
"name":"Drago",
"email":"drago@gmail.com",
"password":"123456"
}
```

---

#### Login User

```
POST /api/auth/login
```

Response:

```
{
"token":"JWT_TOKEN"
}
```

---

## 💳 Transaction APIs (Protected)

Requires **Authorization Token**

Header:

```
Authorization: JWT_TOKEN
```

---

### Create Transaction

```
POST /api/transactions
```

Body:

```
{
"title":"Food",
"amount":250
}
```

---

### Get Transactions

```
GET /api/transactions
```

---

### Update Transaction

```
PUT /api/transactions/:id
```

---

### Delete Transaction

```
DELETE /api/transactions/:id
```

---

## 🧪 API Testing

You can test APIs using:

* ⚡ **Thunder Client (VS Code)**
* 📮 **Postman**

---

## 🗄️ Database

Database used:

```
MongoDB
```

Collections:

* 👤 **Users**
* 💳 **Transactions**

Relationship:

```
One User → Many Transactions
```

---

## 🎥 Project Demo

A demo video is included explaining:

* Project structure
* Code explanation
* API testing
* MongoDB database

---

## 👨‍💻 Author

**Student Project – Backend Development**

Built using:

```
Node.js + Express + MongoDB + JWT
```

---

## ⭐ If you like this project

Give it a **star on GitHub ⭐**
