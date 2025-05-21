# 📘 Day 1 – May 21, 2025

## 🚀 What I Did
- Set up a React project using **Vite**.
- Created a basic React app with custom components.
- Learned about the **difference between `npx create-react-app` and `npm create vite@latest`**.
- Understood basic React structure: `App.jsx`, components, JSX, and rendering.

---

## 🧠 Key Learnings

### ✅ Project Setup
- **Two ways to start a React project:**
  1. `npx create-react-app`
  2. `npm create vite@latest`
- Vite is **faster**, uses **modern ES modules**, and has a **cleaner setup** compared to Create React App (CRA).

### ✅ React Basics
- Every component (function) must:
  - Start with a **Capital Letter**.
  - Have a `.jsx` extension (especially important when using Vite).
- The main entry file typically:
  - Imports `StrictMode` and the main `App` component.
  - Uses `createRoot` to mount the app.

---

## 🧩 Code Written

### 🔹 `main.jsx`
```jsx
import { StrictMode } from 'react';
import { createRoot } from 'react-dom/client';
import App from './App.jsx';

createRoot(document.getElementById('root')).render(
  <StrictMode>
    <App />
  </StrictMode>,
);
```
### 🔹 `App.jsx`
```jsx
import Chai from './Index.jsx';

function App() {
  return (
    <Chai />
  );
}

export default App;
```
### 🔹 `Index.jsx`
```jsx
function Chai(){
  return (
    <h1>Learning react from ChaiAurCode | Anam Saeed</h1>
  );
}

export default Chai;
```