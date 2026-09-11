# 🩸 Blood Bank Management System (BBMS) - Backend API

[![Author - Nitesh Singh](https://img.shields.io/badge/Author-Nitesh%20Singh-red.svg?style=for-the-badge&logo=github)](https://github.com/)
[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-5.x-black?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Database-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Swagger](https://img.shields.io/badge/Swagger-API%20Docs-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)](http://localhost:5000/api/doc/)

**Enterprise RESTful API engine powering the Blood Bank Management System (BBMS).**

Maintained & Developed by **Nitesh Singh**

---

## 📌 Overview

The BBMS Backend is a high-throughput, asynchronous Node.js & Express API engineered to manage blood inventory cycles, emergency hospital requisitions, donor registries, blood drives, and secure role-based operations.

---

## 🛠️ Architecture & Technologies

- **Runtime:** Node.js (ES Modules)
- **Web Framework:** Express.js v5
- **Database:** MongoDB via Mongoose ODM
- **Authentication:** JSON Web Tokens (JWT) & bcryptjs
- **API Documentation:** Swagger / OpenAPI 3.0 via `swagger-ui-express`
- **CORS & Security:** Configured whitelist middleware with pre-flight handling

---

## 🚀 Quick Start

### 1. Install Dependencies
```bash
npm install
```

### 2. Environment Configuration
Create a `.env` file in the `backend/` directory:
```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/bloodbank
JWT_SECRET=your_jwt_secret_key_at_least_32_chars_long
FRONTEND_URL=http://localhost:5174
```

### 3. Seed Initial Administrator Account
```bash
node seedAdmin.js
```

### 4. Start Server
```bash
npm start
```
Server runs at `http://localhost:5000`  
Swagger API Documentation: `http://localhost:5000/api/doc/`

---

## 📡 REST API Route Structure

| Route Prefix | Module | Description |
| :--- | :--- | :--- |
| `/api/auth` | Authentication | Login, registration, token authentication |
| `/api/admin` | Admin Control | Administrative oversight and user management |
| `/api/donor` | Donors | Donor appointments and donation history |
| `/api/facility` | Healthcare Facilities | Facility registrations and hospital requests |
| `/api/blood-lab` | Lab Testing | Sample testing, validation, and component allocation |
| `/api/hospital` | Hospital Services | Requisitions and fulfillment tracking |

---

## 👨‍💻 Maintainer

Developed by **Nitesh Singh**
