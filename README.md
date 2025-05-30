# MERN Stripe Commerce Platform

This project is a full-stack e-commerce application built using the MERN stack (MongoDB, Express.js, React.js, and Node.js) with Stripe integration for secure and seamless payment processing. Key features include user authentication, product management, shopping cart functionality, and order handling.

## Features

- User Authentication (Sign-up, Login, Logout)  
- Product Management (Add, View, List Products)  
- Shopping Cart (Add, Remove, Modify Items)  
- Secure Payment Processing with Stripe Checkout  
- Order Management with storage in MongoDB  
- Responsive User Interface built with React  

## Technology Stack

- **Frontend:** React.js, Redux Toolkit, Axios  
- **Backend:** Node.js, Express.js  
- **Database:** MongoDB (via Mongoose)  
- **Payments:** Stripe API  
- **Authentication:** JSON Web Tokens (JWT)  
- **Development Tools:** Nodemon, concurrently, dotenv

## Stripe Integration

Stripe Checkout is used for payment handling. When a user initiates checkout, the backend creates a Stripe session and redirects the user to Stripe’s secure payment page. After payment completion, Stripe’s webhook notifies the backend to finalize the order.

## Environment Variables

Create a `.env` file inside the `backend/` directory with the following variables:

\```
DB_URI=your_mongodb_uri
JWT_SECRET_KEY=your_jwt_secret
STRIPE_KEY=your_stripe_secret_key
CLIENT_URL=http://localhost:3000
STRIPE_WEB_HOOK=your_stripe_webhook_secret
\```

```
DB_URI=your_mongodb_uri
JWT_SECRET_KEY=your_jwt_secret
STRIPE_KEY=your_stripe_secret_key
CLIENT_URL=http://localhost:3000
STRIPE_WEB_HOOK=your_stripe_webhook_secret
```

## Installation and Setup

1. Clone the repository:
git clone https://github.com/your-username/mern-stripe-commerce.git
cd mern-stripe-commerce

2. Install dependencies:
npm install
cd frontend
npm install

3. Run the project:
From the root directory, run:
npm run dev

This will start the backend server on [http://localhost:5000](http://localhost:5000) and the frontend on [http://localhost:3000](http://localhost:3000).
