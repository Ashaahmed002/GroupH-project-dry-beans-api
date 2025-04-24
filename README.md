# GroupH-project-dry-beans-api
# Dry Beans Classification System with Node.js, PostgreSQL & Swagger

This project is a full-stack application for managing and analyzing dry bean classification data using a PostgreSQL database, a Node.js/Express.js backend, and a modern frontend interface. It enables CRUD operations on dry bean records and provides comprehensive API documentation using Swagger.

---

## 📌 Project Overview

Dry beans are classified into **7 varieties** using **16+ morphological attributes** (such as area, perimeter, major axis length). This system helps store, manage, and query bean data efficiently.
📊 Dataset Information

The dataset classifies seven types of dry beans:

    DERMASON

    SEKER

    BARBUNYA

    BOMBAY

    CALI

    HOROZ

    SIRA


### 🧠 Technologies Used

✅ Project Deliverables

    ✅ Optimized Database Schema

    ✅ Node.js + Express REST API

    ✅ Swagger API Docs

    ✅ Stored Procedures & Triggers

    ✅ Frontend for CRUD interaction

    ✅ PostgreSQL performance optimizations
---

## 📂 Folder Structure

DRY_BEANS_API/
├── .vscode/
│   └── launch.json
├── database/
│   └── database.sql
├── dry-beans-frontend/
│   └── public/
│       ├── index.html
│       ├── script.js
│       └── styles.css
├── sql/
│   ├── procedure.sql
│   └── triggers.sql
├── .env
├── .gitignore
├── package.json
├── query.sql
└── server.js

🧪 API Documentation with Swagger

Swagger is fully integrated and accessible via:

👉 http://localhost:3000/api-docs
Swagger Features:

    Interactive API testing

    Clear and complete endpoint descriptions

    Supports POST, PUT, GET, DELETE with parameters and request bodies.

🔁 API Endpoints
Method | Endpoint | Description
GET | /beans | Fetch all beans
GET | /beans/:id | Fetch a bean by ID
POST | /beans | Add a new bean entry
PUT | /beans/:id | Update an existing bean
DELETE | /beans/:id | Delete a bean entry

🚀 How to Run the Project

1️⃣ Backend (Node.js + PostgreSQL)
Step 1: Install Dependencies;
npm install

Step 2: Configure Environment Variables

Create a .env file in the root directory:
DB_USER=postgres
DB_HOST=localhost
DB_NAME=drybeans
DB_PASSWORD=MySecurePass123
DB_PORT=5432
PORT=3000

Step 4: Start the Server; node server.js

Once server is started it will diplay the following links;
Server running on http://localhost:3000
API docs: http://localhost:3000/api-docs
Test Connection: http://localhost:3000/test-connection
SQL file executed successfully

Database Statistics: 
- Total beans: 13613 
- Distinct classes: 7
- Beans per class:   
  - DERMASON: 3546   
  - SIRA: 2635       
  - SEKER: 2028      
  - HOROZ: 1929      
  - CALI: 1630       
  - BARBUNYA: 1322   
  - BOMBAY: 523      


2️⃣ Frontend
Open Frontend

Navigate to:DRY_BEANS_API/dry-beans-frontend/public/index.html
Open it in your browser. It connects to the backend via API endpoints and displays bean data dynamically.
