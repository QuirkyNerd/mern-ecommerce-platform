# MERN Stripe Commerce Platform
This is a full-stack e-commerce application built using the MERN stack (MongoDB, Express.js, React.js, and Node.js) with Stripe integration for seamless payment processing. The project includes features such as user authentication, product listings, shopping cart functionality, and secure checkout.

# Features
User Authentication (Sign-up, Login, Logout)

Product Management (Add, View, and List Products)

Shopping Cart (Add, Remove, and Modify Cart Items)

Stripe Checkout (Secure Payments via Stripe)

Order Management (Store Orders in MongoDB)

Responsive UI built with React

# Tech Stack
Frontend: React.js, Redux Toolkit, Axios

Backend: Node.js, Express.js

Database: MongoDB (via Mongoose)

Payments: Stripe API

Authentication: JWT (JSON Web Tokens)

Dev Tools: Nodemon, concurrently, dotenv

# Folder Structure
pgsql
Copy
Edit
root/
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── index.js
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── slices/
│   │   ├── App.js
│   │   └── index.js
├── .gitignore
├── package.json
└── README.md

# Stripe Integration
This application uses Stripe Checkout for handling payments. When a user clicks the checkout button, a session is created on the backend and the user is redirected to Stripe’s secure payment page. After a successful payment, Stripe's webhook notifies the server to finalize the order.

# Environment Variables
Create a .env file in the backend/ folder and define the following:

DB_URI=your_mongodb_uri
JWT_SECRET_KEY=your_jwt_secret
STRIPE_KEY=your_stripe_secret_key
CLIENT_URL=http://localhost:3000
STRIPE_WEB_HOOK=your_stripe_webhook_secret

# Installation
Clone the repository
git clone https://github.com/your-username/mern-stripe-commerce.git
cd mern-stripe-commerce

# Install dependencies
npm install
cd frontend
npm install

# Run the project
From root directory
npm run dev

This will concurrently run the backend on http://localhost:5000 and the frontend on http://localhost:3000.

# Testing Stripe Payments
Use the following test card to simulate successful payments:

Card Number: 4242 4242 4242 4242

Expiry: Any future date

CVC: Any 3 digits

ZIP: Any 5 digits

# License
This project is open-source and available under the MIT License.
