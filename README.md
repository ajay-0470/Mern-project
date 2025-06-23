# Product Store 🛒 – A CRUD-based MERN Product Catalog

## Overview 📖

**Product Store** is a MERN-stack (MongoDB, Express.js, React, Node.js) web app for managing a simple product catalog. It offers full **CRUD** functionality: users can add, view, edit, and delete products via a RESTful API. The backend uses Node.js and Express with a MongoDB database (via Mongoose), and the frontend is built with React (Vite) styled using Chakra UI. This results in a responsive, mobile-friendly UI with features like a dark/light mode toggle and toast notifications for user feedback.


## 🖼️ Screenshots

* **Home Page:** Displays all products in a responsive grid. Each product card shows its name, image, and price, with Edit/Delete buttons.
* **Create Page:** A form to add a new product (fields for name, price, and image URL).
* ![image](https://github.com/user-attachments/assets/90610d8a-39e1-4018-8811-9c1981ef233d)
![image](https://github.com/user-attachments/assets/70d7128e-4675-4eb6-bc6e-b9e785cf7993)


## Features ✨

* **Full CRUD Operations:** Add, view, update, and delete products via REST API endpoints.
* **Responsive UI:** Built with Chakra UI’s components (Flex, Grid, etc.) so the layout adapts to different screen sizes.
* **Dark/Light Mode:** Toggle between light and dark themes with a button (powered by Chakra UI’s color mode).
* **Client-side State (Zustand):** Product data is managed on the client using a Zustand store, allowing immediate UI updates after operations.
* **Real-time Feedback:** Success or error toasts notify the user after creating, updating, or deleting a product.

## Tech Stack 🛠️

* **Frontend:** React.js with Vite, Chakra UI, Zustand (state management), React Router DOM (for client-side routing).
* **Backend:** Node.js and Express.js (REST API server) with MongoDB and Mongoose for data persistence.
* **Deployment:** Hosted on Render.

## Getting Started 🏎️

* **Prerequisites:** Ensure you have [Node.js](https://nodejs.org/) installed and a MongoDB database URI (for example from MongoDB Atlas).

### Installation

1. Clone the repo:

```bash
git clone https://github.com/yourusername/product-store.git
cd product-store
```

2. Install backend dependencies:

```bash
npm install
```

3. Install frontend dependencies:

```bash
npm install --prefix frontend
```

### Environment Setup

Create a `.env` file in the `backend/` folder with the following content:

```env
MONGO_URI=your_mongodb_connection_string
PORT=5000
```

### Running the App

* Start the backend server (development mode):

```bash
npm run dev
```

* Start the frontend dev server:

```bash
npm run dev --prefix frontend
```

## API Endpoints 🚧

The backend provides the following REST API routes under `/api/products`:

* `GET /api/products` – Retrieve all products.
* `POST /api/products` – Create a new product.
* `PUT /api/products/:id` – Update a product by its ID.
* `DELETE /api/products/:id` – Delete a product by its ID.

**Enjoy using Product Store!**
