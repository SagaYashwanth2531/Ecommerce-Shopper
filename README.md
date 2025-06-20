# 🛒 Cyber Tech Store – MERN E‑Commerce Application

**Cyber Tech Store** is a full-stack e‑commerce web application built using the MERN stack (MongoDB, Express, React, Node.js), with both a customer-facing storefront and an admin dashboard.

---

## 📁 Project Structure

/
├── backend/ # Express API + MongoDB via Mongoose
├── frontend/ # React storefront
└── admin/ # React admin dashboard

yaml
Copy
Edit

---

## 🚀 Features

### Customer Storefront (`frontend`)
- Browse categories: Phones, Tablets, Laptops, Audio
- Product pages showcase image, price, description
- Add products to cart (persists via React hooks + MongoDB Atlas)
- Authentication: Sign up, Log in/out
- Clean, responsive UI

### Admin Dashboard (`admin`)
- Add new products across 4 categories
- View product list
- Delete products (updates DB → reflects in storefront)

### Backend API (`backend`)
- CRUD endpoints: products, authentication, cart handling
- Middleware: JWT-based auth, CORS, JSON parsing
- Database via MongoDB Atlas & Mongoose

---

## ⚙️ Tech Stack

- **Frontend**: React (functional components, hooks), CSS
- **Backend**: Node.js, Express.js, Mongoose
- **Database**: MongoDB Atlas
- **Auth**: JWT
- **Other**: CORS, bcrypt, multer (for file uploads)

---

## 🔧 Getting Started

1. Clone the repo:  
   `git clone https://github.com/iahmad16/MERN-ECommerce-Full-Stack-Project.git`

2. Install dependencies:

   ```bash
   cd backend && npm install
   cd ../frontend && npm install
   cd ../admin && npm install
Setup .env in backend/ (example):

ini
Copy
Edit
MONGO_URI=<your MongoDB Atlas URI>
JWT_SECRET=<your_secret>
PORT=5000
Run backend:

bash
Copy
Edit
cd backend
npm start
Run frontend apps (in separate terminals):

bash
Copy
Edit
cd frontend && npm start
cd admin && npm start
All three parts (backend, storefront, admin) will run concurrently.

🧩 API Endpoints
POST /api/auth/register – user sign-up

POST /api/auth/login – user login & JWT

GET /api/products – list products

GET /api/products/:id – get single product

POST /api/products – add product (admin)

DELETE /api/products/:id – delete product (admin)

GET /api/cart – retrieve cart for user

PUT /api/cart – update cart items

## 🔄 Built‑in DB Persistence
Cart data is stored in MongoDB—so it persists across logins.

Products added/deleted by admin affect both DB and storefront.

## 🎨 UI & Design
Custom logo and branding (flaticon.com icons)

Responsive layout for all devices

## 🔗 Credits
Original tutorial by GreatStack Dev on YouTube
Watch Tutorial

## 📈 Roadmap & Enhancements
Add product reviews and ratings

Integrate payment gateway (Stripe, Razorpay)

Advanced filters & search

Order and user management in admin dashboard

## ✅ Why Use This?
Practice full MERN stack flow

Learn authentication, JWT, protected routes

Understand React hooks with persistent cart

Build admin tools and frontend integration
