# Read: Class 32 : Context API - Behaviors

---

## Review, Research, and Discussion

- **What are some good use cases for using the Context API for global state?**
  Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

- **How can you best test context?**
  The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).

---

### Document the following Vocabulary Terms

- **context** it provides a way to pass data through the component tree without having to pass props down manually at every level. Context is primarily used when some data needs to be accessible by many components at different nesting levels.
  Context is designed to share data that can be considered **_global_** for a tree of React components, such as the current authenticated user, theme, or preferred language.

- **useContext()** useContext hook allows passing data to children elements without using redux. useContext hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”

- **static context** A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object.

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

Dynamic context defines items that are unique to each invocation of an executable, items such as the values for external variables, external function implementations, and resolvers to external inputs or results. These items might change across invocations.

**_Context_** provides a way to pass data through the component tree without having to pass props down manually at every level. Context is primarily used when some data needs to be accessible by many components at different nesting levels.

Context is designed to share data that can be considered **_global_** for a tree of React components, such as the current authenticated user, theme, or preferred language.

**_Caveats_** Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders. To get around this, lift the value into the parent’s state .

