# React Router

## 1. Capturing Parameters from the URL
React Router allows us to capture dynamic parameters from the URL and use them inside components.

---

## 2. React Router is Not Part of Core React
React Router is **not part of core React**.  
It is a **third-party library** that must be installed separately.

---

## 3. Official Website
Always refer to the **official React Router documentation** for accurate and updated information.

---

## 4. What is React Router?

React Router ≠ a separate app or tool.

It is:
- A library
- Written in JavaScript
- Used inside React code

Just like:
- `axios` → HTTP requests  
- `react-hook-form` → forms  
- `react-router-dom` → routing  

---

## 5. React vs React Router (Library Concept)

### React itself is a library
React provides functionalities to reduce code and make UI development easier, such as:
- `useState`
- `useEffect`
- `useContext`
- Other hooks

### React Router is also a library
The goal of a library is:
- To reduce our code
- To handle common problems
- To provide ready-made functionality

React Router solves the **routing problem** in React applications.

It provides:
- `<Link>` → navigation without page reload
- `<NavLink>` → navigation with active state
- `<Routes>` → define route mappings
- `<Route>` → map URL to component
- `useParams` → read URL parameters
- `useNavigate` → programmatic navigation

---

## 6. Why We Don’t Use `<a>` Tag in React

We don’t use the `<a>` tag for navigation because it reloads the entire page.

When a page reload happens:
- The whole DOM is destroyed
- A new DOM tree is created
- JavaScript state is lost

React works differently:
- React is a SPA (Single Page Application)
- The page does NOT reload
- React updates only the required parts of the UI
- It uses Virtual DOM and diffing algorithm
- Only changed nodes are updated in the real DOM

So in React:
- `<a href="">` → full page reload 
- `<Link to="">` → client-side navigation without reload  

We use `<Link>` instead of `<a>` in React.

---

## 7. `<a>` vs `<Link>`

### With `<a>` tag:
- Uses the `href` attribute
- Example:
  ```html
  <a href="/about">About</a>

