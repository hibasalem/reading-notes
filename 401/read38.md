# Read: Class 38 : Redux - Asynchronous Actions

---

## Review, Research, and Discussion

- **How granular should your reducers be?**

It’s easy to go full-warp with very specific events, dedicated for every change that occurs when a user is editing forms such as CHANGE_NAME, CHANGE_STREET, CHANGE_AGE, etc…
But it is not actually necessary if the logic behind the update is not different for all those fields. For those parts which require different handling in various reducers; dedicated action is the best solution. For others, sometimes a general action might be good enough.

- **Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched**

Whether this is good or bad depends on your app. having many stores (or Redux reducers) handling the same action is actually very convenient because it divides responsibilities, and also lets people work on feature branches without colliding with the rest of the team. In my experience it's easier to maintain unrelated mutations separately than one giant mutation.
But there are cases where this doesn't work too well. I'd say they are often symptoms of a suboptimal state model. For example,
in some cases, one reducer may depend on data from another(like moving a message from unread to message, or even promote a message as a new thread from message to thread)
is a symptom of a problem. If you have to move stuff inside your state a lot, maybe the state shape needs to be more normalized.

- **Name a strategy for preventing the above**

thunk

---

### Document the following Vocabulary Terms

- **store** A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer. Let us see how we can create a store using the createStore method from Redux.

- **combined reducers** The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

- a **_Redux store doesn't know anything about async logic_**. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

- a **_side effect_** is any change to state or behavior that can be seen outside of returning a value from a function.
  some common kinds of side effects are things like( Logging a value to the console , Setting an async timer , Saving a file , Making an AJAX HTTP request)

Redux **_middleware_** were designed to **_enable_** writing logic that has **_side effects_**.

One possibility is writing a middleware that looks for specific action types, and runs async logic when it sees those actions

we can write a middleware that let us pass a function to dispatch, instead of an action object , We could have our middleware check to see if the "action" is actually a function instead, and if it's a function, call the function right away. That would let us write async logic in separate functions, outside of the middleware definition. this "async function middleware" let us pass a function to dispatch

![](https://redux.js.org/assets/images/ReduxAsyncDataFlowDiagram-d97ff38a0f4da0f327163170ccc13e80.gif)

Redux Thunk Middleware

 The thunk middleware allows us to write functions that get dispatch and getState as arguments. The thunk functions can have any async logic we want inside, and that logic can dispatch actions and read the store state as needed.

Why Do I Need This?
With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store.

Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.

