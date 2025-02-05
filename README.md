 NexCart: Serverless E-commerce API

NexCart is a modern, scalable, and cost-effective serverless e-commerce API designed to streamline online shopping experiences. Built with cutting-edge technologies, it simplifies product management, secure payments, and user authentication while ensuring high performance and reliability.

🚀 Features

✅ Serverless Architecture

Built on AWS Lambda, reducing infrastructure costs by 60% compared to traditional servers.

🔒 Secure Payments

Integrated Stripe Checkout for seamless and secure payment processing.

Real-time order updates via webhooks.

🛍️ Efficient Product Management

Designed MongoDB schemas for inventory tracking.

Automated product syncing with Stripe using CRON jobs.

🛡️ Robust Authentication

Implemented JWT-based authentication with refresh tokens for enhanced security.

📊 Rate Limiting

Enforced rate limiting (15 requests/minute) to prevent abuse and ensure fair usage.

🧪 High Test Coverage

Achieved 90% test coverage using Jest for reliable and maintainable code.

📈 Performance Monitoring

Monitored API performance and logs using AWS CloudWatch for real-time insights.

🛠️ Tech Stack

Technology

Purpose

Node.js

Backend development

AWS Lambda

Serverless API hosting

MongoDB

Database for storing e-commerce data

Stripe

Payment processing

JWT

Secure authentication

Jest

Testing framework

AWS CloudWatch

API performance monitoring

CRON jobs

Automated product syncing

RESTful API

API design architecture

📦 Installation

Prerequisites

Ensure you have the following installed:

Node.js (v16 or later)

MongoDB

AWS CLI (configured with your credentials)

Clone the Repository

git clone https://github.com/your-username/nexcart.git
cd nexcart

Install Dependencies

npm install

🔧 Configuration

Create a .env file in the root directory and add the following variables:

PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
AWS_ACCESS_KEY_ID=your_aws_access_key
AWS_SECRET_ACCESS_KEY=your_aws_secret_key

🚀 Running the Project

Start the Development Server

npm start

Run Tests

npm test

📌 API Endpoints

Authentication

Method

Endpoint

Description

POST

/api/auth/register

Register a new user

POST

/api/auth/login

Authenticate user and get token

POST

/api/auth/refresh

Refresh authentication token

Products

Method

Endpoint

Description

GET

/api/products

Get all products

GET

/api/products/:id

Get product details

POST

/api/products

Add a new product (Admin only)

PUT

/api/products/:id

Update product details (Admin only)

DELETE

/api/products/:id

Delete a product (Admin only)

Orders

Method

Endpoint

Description

POST

/api/orders

Create a new order

GET

/api/orders/:id

Get order details
