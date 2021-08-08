# Read: Class 27 : useState() Hook

---

## Review, Research, and Discussion

- **How does React differ from vanilla JS/HTML/CSS?**

Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit , With React, we write HTML using JavaScript. We rely on the power of JavaScript to generate HTML that depends on some data, rather than enhancing HTML to make it work with that data. Enhancing HTML is what other JavaScript frameworks usually do

- **What is the primary difference between a function component and a class component?**

A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element.

---

### Document the following Vocabulary Terms

- **Functional Components** basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.

- **Children / Child Components**
  children is a special property of React components which contains any child elements defined within the component

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

- Hooks let us organize the logic inside a component into reusable isolated units , we used to avoid Huge components , Duplicated logic , Complex patterns .

- Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props.

- Hooks are functions that let you “hook into” React state and lifecycle features from function components

- `useState`

`const [count, setCount] = useState()` is similar to `this.state.count` and `this.setState` in a class

- `useEffect`

adds the ability to perform side effects from a function component. It serves the same purpose as `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount` in React classes

- Hooks are JavaScript functions, but they impose **_two additional rules_**:

  1. Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
  2. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions.

- `useContext`

lets you subscribe to React context without introducing nesting

- `useReducer`

lets you manage local state of complex components with a reducer

- Basic Hooks

  useState
  useEffect
  useContext

- Additional Hooks

  useReducer
  useCallback
  useMemo
  useRef
  useImperativeHandle
  useLayoutEffect
  useDebugValue
