# MEAN Food Delivery Application

A full-stack food delivery application built with the MEAN stack (MongoDB, Express.js, Angular, Node.js). The application provides a seamless and secure shopping experience with advanced search capabilities and a checkout process integrated with PayPal.

## Features

- **Search and filter**: Easily search and filter food items.
- **User authentication**: Secure login and user registration system.
- **Order management**: Place and manage orders.
- **PayPal integration**: Checkout via PayPal for secure payments.
- **Interactive maps**: Location features powered by Leaflet.

## Tech Stack

- **MongoDB**: NoSQL database for storing data.
- **Express.js**: Web framework for Node.js.
- **Angular**: Frontend framework.
- **Node.js**: Server-side JavaScript runtime.
- **TypeScript**: Superset of JavaScript for better tooling.
- **RxJS**: Reactive programming library for handling asynchronous operations.
- **PayPal**: Payment gateway for checkout.
- **Leaflet**: Map rendering library for location-based features.

## Installation Guide

To run this project locally, follow the steps below.

### 1. Clone the repository

Clone the project to your local machine:

```
git clone https://github.com/ArmanWain/mean-food-delivery-app.git
cd mean-food-delivery-app
```

### 2. Configure environment variables

The project requires environment variables for both the server and client. Here's how to set them up.

#### Server-side environment variables

Create a `.env` file in the server directory and add the following:

```
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/mealdash
JWT_SECRET=YOUR-JWT-SECRET
```

Replace `YOUR-JWT-SECRET` with a secure secret key for JWT authentication.

#### Client-side environment variables

Generate an `environment.ts` file for the Angular frontend using the following command:

```
ng generate environments
```

Then, configure the `environment.ts` file like this:

```
export const environment = {
  production: false,
  apiBaseUrl: "http://localhost:5000",
};
```

### 3. Install dependencies

You need to install dependencies for both the client and server.

#### Client dependencies

Navigate to the client directory and install dependencies:

```
cd client
npm install
```

#### Server dependencies

Then, navigate to the server directory and install dependencies:

```
cd ../server
npm install
```

### 4. Run the project

To start the project in development mode, follow these steps:

#### Start the backend

In the server directory, run:

```
npm run start
```

#### Start the frontend

In the client directory, run:

```
npm run start
```

Your application will now be running at http://localhost:4200.
