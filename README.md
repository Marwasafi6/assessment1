# React Product Dashboard - Assignment 1

## Description

This project is a simple **Product Dashboard** built using **React** and **Vite**.  
It demonstrates fundamental React concepts learned in class:

- Building **components**
- Using **props** to pass data
- Managing **state**
- Handling **events**
- Rendering **lists**
- Using **composition** (`children`)
- Writing clean, predictable React code

The dashboard lets the user:

- Show or hide a list of products
- Type their name in an input field
- See a dynamic greeting: `Hello, {name}`

All product data is **static** and hard-coded.

---

## Project Structure

assignment1
├─ index.html
├─ package.json
├─ vite.config.js
└─ src
├─ App.jsx
├─ main.jsx
└─ components
├─ Card.jsx
├─ Product.jsx
└─ ProductList.jsx

---

## Components

### 1. App.jsx
- Root component
- Holds state for:
  - `showProducts` (boolean) – toggles product list visibility
  - `name` (string) – stores user input
- Renders:
  - Heading
  - Toggle button for product list
  - Input field for name
  - Dynamic greeting
  - `ProductList` (conditionally)

### 2. ProductList.jsx
- Contains a static array of products:

```js
[
  { id: 1, title: "Laptop", price: 1200 },
  { id: 2, title: "Phone", price: 800 },
  { id: 3, title: "Tablet", price: 600 }
]
Renders multiple Product components using .map()

Passes title and price as props

Uses id as a stable key

3. Product.jsx

Reusable component

Accepts title and price as props

Wrapped inside the Card component

Stateless — uses props only

4. Card.jsx

Layout wrapper component

Accepts children prop

Provides simple styling (border, padding, margin)

Can wrap any content
How to Run

Open terminal in your project folder:

cd C:\Users\ahmet\Downloads\assignment1


Install dependencies:

npm install


Start the development server:

npm run dev
Open your browser at:

http://localhost:5174/


Note: The port may differ (Vite might pick 5173, 5174, etc.). Use the URL shown in the terminal.


What I Learned / Challenges

Initially opening index.html directly didn’t work → needed Vite server

Figuring out correct folder structure

Connecting components and passing props correctly

Making input a controlled component
