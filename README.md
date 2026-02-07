# Task Manager API 🚀

A **production-ready Node.js + Express + MongoDB boilerplate** designed with clean architecture, scalable folder structure, centralized error handling, and reusable utilities. This project is ideal for building real-world REST APIs with best practices.

---

## ✨ Features

* ⚡ Express.js with ES Modules
* 🗄️ MongoDB integration using Mongoose
* 🔐 Environment-based configuration with dotenv
* 🌍 CORS enabled
* 🧱 Clean & scalable project structure
* ♻️ Centralized async error handling
* 📦 Standardized API response & error format
* 🧪 Health check endpoint
* 🔄 Auto-restart with Nodemon (dev)
* 🎨 Code formatting with Prettier

---

## 🛠️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB, Mongoose
* **Utilities:** dotenv, cors, express-validator
* **Developer Tools:** Nodemon, Prettier

---

## ⚙️ Environment Variables

Create a `.env` file in the root directory:

```env
MONGO_URI=mongodb://localhost:27017/mydatabase
PORT=8000
NODE_ENV=development
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/task-manager.git
cd task-manager
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Run the Server

#### Development Mode (with hot reload)

```bash
npm run dev
```

#### Production Mode

```bash
npm start
```

Server will start on:

```
http://localhost:8000
```

---

## 🩺 Health Check API

**Endpoint:**

```
GET /api/v1/healthcheck
```

**Response:**

```json
{
  "statusCode": 200,
  "data": {
    "message": "Server is running"
  },
  "message": "Success",
  "success": true
}
```

---

## 🧱 API Utilities

### ✅ ApiResponse

Ensures a consistent success response format across APIs.

### ❌ ApiError

Custom error class extending native `Error` for structured error handling.

### 🔁 asyncHandler

Wraps async controllers to eliminate repetitive try-catch blocks.

---

## 🧯 Global Error Handling

All errors are handled via a centralized middleware:

* Handles Mongoose validation errors
* Supports custom API errors
* Shows stack trace in development mode only

---

## 🎨 Code Formatting

Prettier is configured to enforce consistent styling.

Run manually:

```bash
npx prettier --write .
```

---

## 📌 Best Practices Followed

* Separation of concerns
* Environment-based configs
* Scalable folder structure
* Reusable utilities
* Clean error & response patterns

---

## 🧩 Future Enhancements

* Authentication & Authorization
* Task CRUD APIs
* Role-based access control
* Request validation middleware
* API documentation with Swagger
* Unit & integration tests

---

## 👨‍💻 Author

**Rahul Kumar**
Full-Stack Developer (MERN)

* 💼 Backend | Frontend | DevOps
* 🚀 Passionate about scalable systems

---

## 📄 License

This project is licensed under the **MIT License**.

---

⭐ If you found this helpful, consider giving the repo a star!
