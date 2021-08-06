# Read: Class 26 : Component Based UI

---

## Review, Research, and Discussion

- **Name 5 Javascript UI Frameworks (other than React)**

  - Ext JS by Sencha.
  - Angular.
  - Vue.
  - Ember.
  - Svelte 3.

- **What’s the difference between a framework and a library?**

  The technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the application flow. You choose when and where to call the library. When you use a framework, the framework is in charge of the flow. It provides you with a few places to plug in your code, but it calls the code you plugged in as needed.
  Framework is often more restrictive and generally have a more set of rules.Whereas, Library is not bounded by many rules.

---

### Document the following Vocabulary Terms

- **Rendering** the process of displaying something on a screen.

- **Templates** a generic class or other unit of source code that can be used as the basis for unique units of code

- **State** an object of a set of observable properties that control the behavior of the component

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

hooks in react

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

- **_JSX_** stands for JavaScript XML. It is simply a syntax extension of JavaScript. It allows us to directly write HTML in React (within JavaScript code). It is easy to create a template using JSX in React, but it is not a simple template language instead it comes with the full power of JavaScript.

- React elements are immutable. An element is like a single frame in a movie: it represents the UI at a certain point in time.

- React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.

