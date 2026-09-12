# 🌱 e-plantShopping

A simple e-commerce web application for browsing and purchasing plants, built with **React** and **Redux Toolkit**. Users can view products, add them to a shopping cart, adjust quantities, remove items, and see the total cost update in real time.

## Features

- 🛒 Add products to cart
- ➕➖ Increase or decrease item quantity
- ❌ Remove items from the cart
- 💰 Automatic calculation of total cost per item and overall cart total
- ⚡ Fast development/build powered by Vite
- 🌐 Deployed with GitHub Pages

## Tech Stack

- **React** — UI library
- **Redux Toolkit** — state management (cart logic via `createSlice`)
- **React Redux** (`useSelector`, `useDispatch`) — connecting components to the store
- **Vite** — build tool and dev server
- **gh-pages** — deployment to GitHub Pages

## Project Structure

```
src/
├── assets/
├── AboutUs.jsx / AboutUs.css
├── App.jsx / App.css
├── CartItem.jsx / CartItem.css
├── CartSlice.js
├── ProductList.jsx / ProductList.css
├── index.css
├── main.jsx
└── store.js
```

- **`store.js`** — configures the Redux store and registers the `cart` reducer
- **`CartSlice.js`** — defines the cart's initial state and reducers (`addItem`, `removeItem`, `updateQuantity`)
- **`ProductList.jsx`** — displays available plants and lets users add them to the cart
- **`CartItem.jsx`** — displays cart contents, quantity controls, item totals, and the cart's grand total

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended)
- npm

### Installation

```bash
git clone https://github.com/jasurbek-dev-code/e-plantShopping.git
cd e-plantShopping
npm install
```

### Run in development mode

```bash
npm run dev
```

### Build for production

```bash
npm run build
```

## Deployment

This project is deployed to GitHub Pages using the `gh-pages` package.

```bash
npm run deploy
```

This runs `npm run build` automatically (via the `predeploy` script) and pushes the contents of the `dist` folder to the `gh-pages` branch.

Live site:
```
https://jasurbek-dev-code.github.io/e-plantShopping/
```

> Note: `git push` only updates the source code on the `main` branch. To update the live site, `npm run deploy` must be run separately after pushing changes.

## License

This project is licensed under the terms specified in the `LICENSE` file.
