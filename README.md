# 🛍️ Secure MERN Commerce Hub

A full-stack online shopping platform built with the **MERN stack** — **MongoDB, Express.js, React, and Node.js**.
This project is designed to deliver a smooth shopping experience for users while giving administrators the tools they need to manage products, orders, customers, and business activity from one place.

## What this project includes

This application combines modern frontend design with a secure backend architecture. It supports account access, product browsing, shopping cart actions, checkout flow, payment processing, and a complete admin management system.

## Main Capabilities

### Shopper Side

* Sign up and log in using JWT authentication
* Explore newly added products
* View popular and high-demand products
* Add items to the cart and update quantities
* Complete checkout with order confirmation
* Cancel an order within 1 hour
* Leave ratings and reviews for products
* Check past purchases and order records
* Search products and apply filters by category, price, and other options
* Pay safely online using Razorpay
* Confirm delivery availability within a 5 km service area

### Admin Side

* Secure administrator login
* Add, edit, and remove products
* Manage customer accounts
* Track and update order progress
* Monitor stock availability
* Review sales data and performance insights
* Remove inappropriate or low-quality reviews

## Technology Used

### User Interface

* React.js
* React Router
* Tailwind CSS
* Axios
* REST API integration
* Context API for app-wide state handling

### Server and Database

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT authentication
* Nodemailer for notification emails

### Development Utilities

* Vite for frontend development
* ESLint and Prettier for code quality
* Git and GitHub for version control
* Dotenv for environment configuration

## Folder Organization

```text
COLLEGEPROJECT-E-COMMERCE/
│
├── admin/
│   └── src/
│       ├── assets/         # Images, icons, logos, and static files
│       ├── components/     # Shared admin UI elements
│       ├── pages/          # Admin screens for products, orders, and analytics
│
├── backend/
│   ├── config/             # Database and app configuration
│   ├── controllers/        # Logic for handling requests
│   ├── middleware/         # Auth, validation, and error handlers
│   ├── models/             # Database schemas
│   ├── routes/             # API endpoints
│   ├── templates/          # Email templates
│   └── utils/              # Helper functions
│
├── frontend/
│   └── src/
│       ├── assets/         # Public images and visual resources
│       ├── components/     # Reusable frontend components
│       ├── context/        # Global state management
│       └── pages/          # Customer-facing pages
│
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/pawan-chaudhary-70056/MERN-Commerce-Hub.git
cd MERN-Commerce-Hub
```

### 2. Run the frontend

Create a `.env` file inside `frontend/`:

```env
VITE_BACKEND_URL=YOUR_BACKEND_URL
VITE_RAZORPAY_KEY_ID=YOUR_RAZORPAY_KEY_ID
```

Then install and start the app:

```bash
cd frontend
npm install
npm run dev
```

### 3. Run the backend

Create a `.env` file inside `backend/`:

```env
PORT=YOUR_PORT_NUMBER
CLOUDINARY_API_KEY=YOUR_CLOUDINARY_API_KEY
CLOUDINARY_SECRET_KEY=YOUR_CLOUDINARY_SECRET_KEY
CLOUDINARY_NAME=YOUR_CLOUDINARY_NAME
JWT_SECRET=YOUR_JWT_SECRET
ADMIN_EMAIL=YOUR_EMAIL/ADMIN
ADMIN_PASSWORD=YOUR_ADMIN_PASSWORD
RAZORPAY_KEY_SECRET=YOUR_RAZORPAY_KEY_SECRET
RAZORPAY_KEY_ID=YOUR_RAZORPAY_KEY_ID
EMAIL_USER=YOUR_APP_EMAIL
EMAIL_PASS=YOUR_APP_EMAIL_PASSWORD
```

Then install dependencies and launch the server:

```bash
cd backend
npm install
npm run server
```

### 4. Run the admin panel

Create a `.env` file inside `admin/`:

```env
VITE_BACKEND_URL=YOUR_BACKEND_URL
```

Then install and start the admin interface:

```bash
cd admin
npm install
npm run dev
```

## Project Purpose

This project demonstrates how a real-world e-commerce system can be built with authentication, payments, inventory control, customer interaction, and administrative oversight. It is suitable for learning, portfolio presentation, and practical full-stack development practice.
