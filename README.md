# Product List Task

---

## Project Overview

A full-stack Product Listing application built using React (frontend) and Node.js with Express (backend). This project demonstrates implementation of search, category filtering, and price sorting using REST APIs.

---

## Frontend Implementation

- Built using React functional components following modern React conventions
- Communicates with the backend via Axios for all HTTP requests
- Search functionality is triggered for controlled user interaction
- UI updates **dynamically** in response to API data changes without full page reloads
- Styled and structured using **Material UI (MUI)** component library for a consistent, professional interface

---

## Backend Implementation

- Exposes REST APIs to serve product data to the frontend
- Implements server-side search logic to filter products by name query
- Implements category-based filtering to return products within a specified category
- Implements price sorting logic to return products in ascending or descending order
- Follows a clean project structure with dedicated **models**, **routes**, and **validation** layers
- Returns well-structured **JSON responses** for all API endpoints

---

## Technology Stack

**Frontend:**
- React.js
- Axios
- Material UI (MUI)

**Backend:**
- Node.js
- Express.js

**Database:**
- MongoDB

---


## Project Structure

```
Product List Task/
├── Backend/
│   ├── src/
│   │   ├── models/          # Mongoose schemas and data models
│   │   ├── routes/          # Express route handlers and API endpoints
│   │   └── validation/      # Request validation logic
│   └── server.js            # Entry point for the Express server
├── Frontend/
│   ├── src/
│   │   ├── App.jsx          # Root React component
│   │   └── main.jsx         # Application entry point
│   ├── index.html           # Base HTML template
│   └── vite.config.js       # Vite bundler configuration
└── README.md
```

---

## Installation and Setup

### Prerequisites

Ensure the following are installed before proceeding:

- [Node.js](https://nodejs.org/) 
- [MongoDB](https://www.mongodb.com/) (local instance)
- npm 

---

### Backend Setup

```bash
cd Backend
npm install
npm run dev
```

The backend server will start on the configured port (default: `http://localhost:5000`).

---

### Frontend Setup

```bash
cd Frontend
npm install
npm run dev
```

The frontend development server will start at `http://localhost:5173` (Vite default).

---

## Application Flow

1. **Request Initiation** — The frontend sends HTTP requests to the backend using Axios, passing query parameters for search terms, category filters, or sort preferences.
2. **Server-Side Processing** — The Express backend receives the request and applies the appropriate search, filtering, and sorting logic before querying MongoDB.
3. **JSON Response** — The backend returns a structured JSON response containing the matching product data.
4. **Dynamic UI Update** — The React frontend receives the response and dynamically re-renders the product list to reflect the updated results — without requiring a full page reload.
