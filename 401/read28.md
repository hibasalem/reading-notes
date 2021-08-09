# Read: Class 28 : Component Lifecycle / useEffect() Hook

---

## Review, Research, and Discussion

- **Why do we not need more .html pages in a multi-page React app?**

react apps are single page app ,A React app consists of a single HTML file index.html. The views are coded in JSX format as components.

- **If we wanted a component to show up on every page, where would we put it and why?**

Inside the `<BrowserRouter />`, outside a `<Route />`, to have it always no matter what the current route is .

- **What does routing do with the components that were rendered when a new route is requested**

it goes to the new componetnt and remove the old one **_cleans up _**

- **What does props.children contain?**

it has the value that we reatern from the component

- **How do useState() and this.setState() differ**

setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won't touch the rest. The useState's updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

---

### Document the following Vocabulary Terms

- **State Hook** The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

- **Mounting and Un-Mounting** The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by **mounting** (adding nodes to the DOM), **unmounting** (removing them from the DOM), and **updating** (making changes to nodes already in the DOM).

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

- Effect Hook

The Effect Hook lets you perform side effects in function components  
you can think of `useEffect` Hook as `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount` combined.

```

 // Similar to componentDidMount and componentDidUpdate:
  useEffect(() => {
    // code block
  });

```

- **_What does useEffect do?_**  
  By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates

- **_Why is useEffect called inside a component?_**

Placing useEffect inside the component lets us access the state variable right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

- **_Does useEffect run after every render?_**

Yes By default, it runs both after the first render and after every update. Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.

- Effects with Cleanup

```
  useEffect(() => {
   function handleStatusChange(status) {
     setIsOnline(status.isOnline);
   }
   ChatAPI.subscribeToFriendStatus(props.friend.id, handleStatusChange);
   // Specify how to clean up after this effect:
   return function cleanup() {
     ChatAPI.unsubscribeFromFriendStatus(props.friend.id, handleStatusChange);
   };
 });

```

- **_Why did we return a function from our effect?_**

  This is the optional cleanup mechanism for effects. Every effect may return a function that cleans up after it. This lets us keep the logic for adding and removing subscriptions close to each other. They’re part of the same effect!

- **_When exactly does React clean up an effect?_**

  React performs the cleanup when the component unmounts. However, effects run for every render and not just once. This is why React also cleans up effects from the previous render before running the effects next time.


