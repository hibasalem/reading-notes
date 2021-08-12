# Read: Class 31 : Context API

---

## Review, Research, and Discussion

- **Describe use cases useState() vs useReducer()**

  useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

- **Why do custom hooks need the use prefix?**

Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.

- **What do custom hooks usually do?**

Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

- **Using any list of custom hooks, research and name one that you think will be useful in your applications**

1. useScript
   React hook to dynamically load an external script and know when its loaded

   useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.

2. use-mouse-action

   A library with three React hooks for listening to mouse events on an element or JSX element.
   useMouseAction: This is used to register mouse actions on an element.
   useMouseDown: This is used to register a mouse down event on an element.
   useMouseUp: This registers a mouse up event on an element.

---

### Document the following Vocabulary Terms

- **reducer** useReducer is one of the additional Hooks , An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX .useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

**_Custom Hook_** is a JavaScript function which we create by ourselves, when we want to share logic between other JavaScript functions. It allows you to reuse some piece of code in several parts of your app

**_Context_** provides a way to pass data through the component tree without having to pass props down manually at every level. Context is primarily used when some data needs to be accessible by many components at different nesting levels.

Context is designed to share data that can be considered **_global_** for a tree of React components, such as the current authenticated user, theme, or preferred language.

**_Caveats_** Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders. To get around this, lift the value into the parent’s state . 

