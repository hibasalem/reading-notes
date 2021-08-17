# Read: Class 33 : `<Login /> `and `<Auth />`

---

## Review, Research, and Discussion

- **Why is the Context API useful?**

The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux

- **Can a component outside of a provider get its context?**

when using global context

- **What are some common use cases for using the Context API?**

Context is primarily used when some data needs to be accessible by many components at different nesting levels

- **Describe “Context Hell”**

multiple context provider in class component

---

### Document the following Vocabulary Terms

- **global state** a global state is a set of local states which are all concurrent with each other. By concurrent, we mean that no two states have a cause and effect relationship with each other.

- **global context** context that affects the entire application, and it will share data to everything in the React component tree.

- **provider** Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers.

- **consumer** A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component. Requires a function as a child. The function receives the current context value and returns a React node

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Through RBAC, you can control what end-users can do at both broad and granular levels.

Managing and auditing network access is essential to information security. Access can and should be granted on a need-to-know basis.

