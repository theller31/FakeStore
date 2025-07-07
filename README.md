# FakeStore E-Commerce React App

## Overview

The FakeStore E-Commerce App is a frontend application built using **React**, **React Router**, **React Bootstrap**, and **Axios**. It interacts with the [FakeStoreAPI](https://fakestoreapi.com/) to simulate real-world product listing and CRUD (Create, Read, Update, Delete) operations. This project provides a beginner-friendly approach to mastering asynchronous data fetching, routing, and component-driven architecture in React.

## Features

### 1. Home Page

* Welcoming UI using React Bootstrap.
* Button to navigate to the product listing page.

### 2. Product Listing Page (`/products`)

* Fetches all products from the FakeStore API using Axios.
* Products are displayed in a responsive grid layout.
* Each product card shows the image, title, price, and a link to view details.

### 3. Product Details Page (`/products/:id`)

* Displays detailed product information.
* Allows deletion of the product (fake DELETE request).
* Handles loading and error states.

### 4. Add Product Page (`/add-product`)

* Contains a form with fields: title, price, description, category.
* Submits a POST request to FakeStore API.
* Displays a success message on submission.

### 5. Edit Product Page (`/edit-product/:id`)

* Pre-fills form with existing data using `useParams`.
* Sends a PUT request to FakeStore API to update the product.
* Displays a confirmation message.

### 6. Delete Functionality

* Available in the product details page.
* Shows a confirmation modal.
* Sends a DELETE request.
* Redirects back to `/products` on confirmation.

### 7. Navigation

* A responsive Navbar using React Bootstrap.
* Includes links to Home, Product Listing, and Add Product.
* Collapses properly on mobile screens.

### 8. Additional Features

* API loading states and error handling.
* Fully responsive UI.
*

- Clean and accessible code.

## Technologies Used

* **React** (Vite + JSX + Hooks)
* **React Router DOM** for navigation
* **Axios** for API communication
* **React Bootstrap** for layout and styling
* **Bootstrap** CSS for responsiveness

## Folder Structure

```
/fakestore-app
├── /src
│   ├── /components
│   │   ├── Navbar.jsx
│   │   ├── ProductCard.jsx
│   │   └── LoadingSpinner.jsx
│   ├── /pages
│   │   ├── Home.jsx
│   │   ├── ProductList.jsx
│   │   ├── ProductDetails.jsx
│   │   ├── AddProduct.jsx
│   │   └── EditProduct.jsx
│   ├── App.jsx
│   ├── main.jsx
├── /public
│   └── index.html
├── .gitignore
├── README.md
├── package.json
└── vite.config.js
```

## How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/fakestore-ecommerce-app.git
cd fakestore-ecommerce-app
```

### Step 2: Install Dependencies

```bash
npm install
```

### Step 3: Start the Development Server

```bash
npm run dev
```

Navigate to `http://localhost:5173` in your browser.

## API Notes

* **GET** `/products`: Fetches all products.
* **GET** `/products/:id`: Fetch product by ID.
* **POST** `/products`: Fake create (won't persist).
* **PUT** `/products/:id`: Fake update (won't persist).
* **DELETE** `/products/:id`: Fake delete (won't persist).

## Known Limitations

* Since FakeStore API is mock-based, data changes do not persist.
* No authentication or cart functionality included (can be added as advanced features).



## Author

Created by Toneja Heller as part of the Advanced Frontend React Module at Coding Temple.

---

## License

This project is licensed for educational use only. The FakeStore API is a public mock API provided for learning and development purposes.
