# 🍕 React Pizza

A feature-rich, modern single-page application (SPA) e-commerce web application built with **React**, **TypeScript**, and **Redux Toolkit**. This project simulates an online pizza ordering platform with advanced filtering, sorting, pagination, search capabilities, and a fully interactive shopping cart synchronized with LocalStorage.

## 🚀 Tech Stack & Core Technologies

* **Core:** React, TypeScript, JavaScript (ES6+)
* **State Management:** Redux Toolkit (with async thunks for API data fetching)
* **Routing:** React Router v6
* **Styling & UI:** SCSS (Sass), CSS Modules, SCSS variables, responsive design (RWD)
* **Build Tool & Bundler:** Vite
* **HTTP Client & Utilities:** Axios, Lodash (debounce for search optimization)
* **Code Quality:** ESLint, Prettier

## ✨ Key Features & Architecture

* **Dynamic Catalog & Filtering:** Multi-category filtering and sorting options (by popularity, price, alphabet) seamlessly integrated with URL query parameters.
* **Server-side Pagination:** Efficient handling of large product lists using pagination components.
* **Debounced Live Search:** Instant search functionality optimized with `lodash.debounce` to reduce unnecessary re-renders and API requests.
* **Interactive Shopping Cart:**
    * Add, remove, and adjust quantities of items.
    * Real-time calculation of total price and total item count.
    * Persistent cart state stored via `LocalStorage`.
* **Skeleton Loaders:** Enhanced UX using modern skeleton loaders (`react-content-loader` style implementation) during asynchronous data fetching.
* **Modular Architecture:** Clean file organization separating components, pages, redux slices, custom hooks, and utility functions.
* **Asynchronous Actions:** Robust API integration using Redux Toolkit `createAsyncThunk` for fetching pizza items cleanly and handling loading/error states.

## 📁 Project Structure

```text
react-pizza-master/
├── public/              # Static assets (favicon, manifests, logos)
├── src/
│   ├── @types/          # TypeScript definitions and asset modules
│   ├── assets/          # Images, icons, and global media
│   ├── components/      # Reusable UI components (Header, CartItem, PizzaBlock, Search, Pagination, etc.)
│   ├── layouts/         # Page layout wrappers (MainLayout)
│   ├── pages/           # Route views (Home, Cart, FullPizza, NotFound)
│   ├── redux/           # Redux Toolkit store, slices (cart, filter, pizza), and typed hooks
│   ├── scss/            # Global styles, variables, component styles, and normalize.scss
│   ├── utils/           # Helper functions (LocalStorage handlers, price calculators)
│   ├── App.tsx          # Root component with routing configuration
│   └── index.tsx        # Application entry point
├── package.json         # Dependencies and scripts
└── tsconfig.json        # TypeScript configuration
```

## ⚙️ Getting Started & Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/iosifchernyshenko/react-pizza.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd react-pizza
   ```

3. **Install dependencies:**
   ```bash
   npm install
   ```

4. **Run the development server:**
   ```bash
   npm run start
   ```

5. **Open your browser:**
   Navigate to `http://localhost:5173` (or the port specified in your terminal).