[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/LjLbd9JV)




🍔 Canteen Food Ordering App (MERN Stack)
🚀 Overview

The Canteen Food Ordering App is a full-stack MERN application that allows users (students/employees/customers) to browse food items, place orders, make online payments, and track their order status in real-time.
Admin can manage menus, track orders, and view analytics.

✨ Features
👥 User Features

🔐 Authentication (Signup/Login with JWT)

🍱 Browse Menu (with categories and search)

🛒 Add to Cart / Remove from Cart

💳 Place Orders & Payment Gateway

⏱ Track Order Status (Pending → Preparing → Delivered)

⭐ Rate and Review Food Items

📜 View Order History

🧑‍🍳 Admin Features

📦 Manage Food Items (Add/Edit/Delete)

🧾 View and Manage Orders

📊 Dashboard Analytics (Top selling items, daily revenue, etc.)

👥 Manage Users

🧠 Tech Stack
Layer	Technology
Frontend	React.js, Redux Toolkit, Tailwind CSS
Backend	Node.js, Express.js
Database	MongoDB (Mongoose ODM)
Authentication	JWT, bcrypt.js
Cloud/Storage	Cloudinary (for food images)
Payment	Razorpay / Stripe
Deployment	Render / Vercel (Frontend) + Railway / Render (Backend)
🧱 Folder Structure
canteen-app/
│
├── client/                         # React Frontend
│   ├── public/
│   └── src/
│       ├── assets/                 # Images, icons, etc.
│       ├── components/             # Reusable components
│       │   ├── Navbar.jsx
│       │   ├── Footer.jsx
│       │   ├── FoodCard.jsx
│       │   ├── CartItem.jsx
│       │   ├── Loader.jsx
│       │   └── RatingStars.jsx
│       ├── pages/                  # Page Components
│       │   ├── Home.jsx
│       │   ├── Menu.jsx
│       │   ├── Cart.jsx
│       │   ├── Orders.jsx
│       │   ├── Login.jsx
│       │   ├── Signup.jsx
│       │   ├── AdminDashboard.jsx
│       │   └── ManageFood.jsx
│       ├── redux/                  # Redux Toolkit setup
│       │   ├── store.js
│       │   ├── slices/
│       │   │   ├── userSlice.js
│       │   │   ├── cartSlice.js
│       │   │   └── foodSlice.js
│       ├── services/               # API Calls
│       │   ├── api.js
│       │   └── authService.js
│       ├── utils/                  # Helper functions
│       ├── App.jsx
│       ├── main.jsx
│       └── index.css
│
├── server/                         # Express Backend
│   ├── config/
│   │   ├── db.js                   # MongoDB connection
│   │   └── cloudinary.js
│   ├── controllers/                # Business logic
│   │   ├── authController.js
│   │   ├── foodController.js
│   │   ├── orderController.js
│   │   └── adminController.js
│   ├── models/                     # Mongoose Schemas
│   │   ├── User.js
│   │   ├── Food.js
│   │   ├── Order.js
│   │   └── Review.js
│   ├── routes/                     # Express Routes
│   │   ├── authRoutes.js
│   │   ├── foodRoutes.js
│   │   ├── orderRoutes.js
│   │   └── adminRoutes.js
│   ├── middleware/
│   │   ├── authMiddleware.js
│   │   ├── adminMiddleware.js
│   │   └── errorMiddleware.js
│   ├── utils/
│   │   └── generateToken.js
│   ├── server.js
│   └── .env.example
│
├── package.json
├── README.md
└── .gitignore