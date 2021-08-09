# Read: Class 28 : Advanced State with Reducers

---

## Review, Research, and Discussion

- **How can we ensure that an effect hook runs only once?**

If we pass an empty array [] , it just renders the component only once like componentDidMount .

- **Can useState() update more than one state variable at the same time?**

You could combine the state into one state object and then you could do one setState call and there will only be one render. Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely.

```
  const [form, setState] = useState({
    username: '',
    password: ''
  });

```

- **Is useState() synchronous?**

useState and setState both are asynchronous. Even though they are asynchronous, the useState and setState functions do not return promises.
Therefore we cannot attach a then handler to it or use async/await to get the updated state values.

---

### Document the following Vocabulary Terms

- **State Hook** The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

- **Component Lifecycle** the series of methods that are invoked in different stages of the component’s existence. The three phases are: Mounting, Updating, and Unmounting.

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

- useReducer

useReducer is one of the additional Hooks , An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX .

it accepts a reducer of type `(state, action) => newState`, and returns the current state paired with a dispatch method.

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one

```
const [state, dispatch] = useReducer(reducer, initialArg, init);

```

- Specifying the initial state

There are two different ways to initialize useReducer state.

1.  The simplest way is to pass the initial state as a second argument

```
  const [state, dispatch] = useReducer(
    reducer,
    {count: initialCount}
  );

```

2. You can also create the initial state lazily

To do this, you can pass an init function as the third argument. The initial state will be set to init(initialArg)


