
---

# ☕ Espresso Emporium  API 

This is a simple RESTful API server built with **Express.js** and **MongoDB Atlas** for managing coffee data. It supports basic CRUD operations like creating, reading, updating, and deleting coffee entries.

---

## 🔗 Live Frontend

👉 Frontend Site: [https://elegant-chaja-103a90.netlify.app/](https://elegant-chaja-103a90.netlify.app/)

---

## ⚙️ Tech Stack

* **Node.js** – JavaScript runtime
* **Express.js** – Web framework for building APIs
* **MongoDB Atlas** – Cloud-hosted NoSQL database
* **dotenv** – For managing environment variables
* **CORS** – For handling cross-origin requests

---

## 📁 Project Structure

```
server.js         → Main server file
.env              → Environment variables
```

---

## 📦 API Endpoints

| Method | Endpoint      | Description                  |
| ------ | ------------- | ---------------------------- |
| GET    | `/`           | Root endpoint (health check) |
| POST   | `/addcoffee`  | Add a new coffee entry       |
| GET    | `/addcoffee`  | Get all coffee entries       |
| GET    | `/coffee/:id` | Get a single coffee by ID    |
| PUT    | `/coffee/:id` | Update coffee by ID          |
| DELETE | `/delete/:id` | Delete coffee by ID          |

---

## 🔐 Environment Variables

Create a `.env` file in the root directory with the following:

```
DB_USER=your_mongodb_user
DB_PASS=your_mongodb_password
PORT=3000
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/plabon2024/Espresso-Emporium-backend.git
cd Espresso-Emporium-backen
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up environment variables

Create a `.env` file and add your MongoDB credentials.

### 4. Run the server

```bash
node server.js
```

The server will start at `http://localhost:3000`.

---

## 📝 Notes

* MongoDB connection is established using the official `mongodb` driver.
* The connection is kept alive for performance, but `client.close()` is commented out to prevent termination.

---
