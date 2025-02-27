

# Aoushadhi Ecommerce Backend

## Description
This project serves as the backend for Aoushadhi, an ecommerce platform specializing in medicinal products. It provides APIs for user management, product listings, orders, payments, and more.

## Environment Variables
Make sure to set up the following environment variables:

- `PORT`: Port number for the server
- `MONGODB_URI`: URI for MongoDB database connection
- `CORS_ORIGIN`: Allowed origin for CORS
- `ACCESS_TOKEN_SECRET`: Secret key for generating access tokens
- `ACCESS_TOKEN_EXPIRY`: Expiry duration for access tokens
- `REFRRESH_TOKEN_SECRET`: Secret key for generating refresh tokens
- `REFRRESH_TOKEN_EXPIRY`: Expiry duration for refresh tokens
- `STRIPE_PUBLISH_KEY`: Stripe publishable key (for payments)
- `STRIPE_SECRET_KEY`: Stripe secret key (for payments)

## Project Structure
```
src/
├── controllers/
│   ├── order.controller.js
│   ├── payment.controller.js
│   ├── product.controller.js
│   └── user.controller.js
├── db/
│   └── index.js
├── middlewares/
│   ├── auth.middleware.js
│   └── error.middleware.js
├── models/
│   ├── order.model.js
│   ├── product.model.js
│   └── user.model.js
├── routes/
│   ├── order.routes.js
│   ├── payment.routes.js
│   ├── product.routes.js
│   └── user.routes.js
├── utils/
│   ├── ApiError.js
│   ├── ApiResponse.js
│   └── asyncHandler.js
├── app.js
├── constants.js
├── index.js

├── .env
├── .env.example
├── .vscode/
├── node_modules/
└── README.md
```

## Scripts
- `dev`: Starts the server using nodemon with dotenv configuration
- `start`: Starts the server using Node.js

## Dependencies
- `bcrypt`: Password hashing library
- `bcryptjs`: Alternative password hashing library
- `cookie-parser`: Middleware for parsing cookies
- `cors`: Cross-Origin Resource Sharing middleware
- `dotenv`: Loads environment variables from `.env` file
- `express`: Web framework for Node.js
- `jsonwebtoken`: Library for generating JSON Web Tokens (JWT)
- `mongoose`: MongoDB object modeling tool
- `razorpay`: Razorpay SDK for payment integration
- `stripe`: Stripe SDK for payment integration

## Prettier Configuration
```
{
  "singleQuote": false,
  "bracketSpacing": true,
  "tabWidth": 2,
  "semi": true,
  "trailingComma": "es5"
}
```

## Usage
1. Clone the repository.
2. Navigate to the `src` folder.
3. Install dependencies using `npm install`.
4. Create a `.env` file in the `src` folder and add necessary environment variables.
5. Start the server using `npm run dev` for development or `npm start` for production.

## Contributing
Contributions are welcome. Please follow [GitHub Flow](https://guides.github.com/introduction/flow/) when making contributions.
