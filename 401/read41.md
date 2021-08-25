# Read: Class 41 : React Native

## Review, Research, and Discussion

- **Compare and Contrast Redux Toolkit with Redux “Ducks”**

The Ducks file system dictates that the Redux bits (actions/reducers/types) live with the components they are dealing with.
Implement ducks in React following the redux pattern but using React Context. Uses immer to wrap reducers when creating, ensuring atomic state mutations

Redux allows you to manage your app's state in a single place and keep changes in your app more predictable and traceable. It makes it easier to reason about changes occurring in your app.

- **What is the principle advantage of Redux Toolkit**

Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience

---

### Document the following Vocabulary Terms

- **redux toolkit slices** A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state.Internally, it uses createAction and createReducer, so you may also use Immer to write "mutating" immutable updates

- **namespace** namespace is a set of signs (names) that are used to identify and refer to objects of various kinds. A namespace ensures that all of a given set of objects have unique names so that they can be easily identified

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

React Native is like React, but it uses native components instead of web components as building blocks.

React Native is an open-source UI software framework created by Facebook It is used to develop applications for Android, Android TV, iOS, macOS, tvOS, Web, Windows and UWP by enabling developers to use the React framework along with native platform capabilities.

the commbonent can ve functional or class component and behaves in the same way as in React for the web. This function returns a View component with some styles and aText as its child.

The Text component allows us to render a text, while the View component renders a container. This container has several styles applied, let's analyze what each one is doing.

Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.

Ejecting to ExpoKit

ExpoKit is an Objective-C and Java library that allows you to use the Expo platform and your existing Expo project as part of a larger standard native project -- one that you would normally create using Xcode, Android Studio, or react-native init.

What is this for?
If you created an Expo project and you want a way to add custom native modules, this guide will explain how to use ExpoKit for that purpose.
