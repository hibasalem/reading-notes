# Read: Class 36 : Application State with Redux

---

## Review, Research, and Discussion

- **What are the advantages of storing tokens in “Cookies” vs “Local Storage”**

* Local Storage :

  - pros: It's convenient.
  - pros: It's vulnerable to XSS attacks.

* Cookies :
  - Pros: The cookie is not accessible via JavaScript; hence, it is not as vulnerable to XSS attacks as localStorage.
  - Cons: Depending on the use case, you might not be able to store your tokens in the cookies.

- Both localStorage and cookies are vulnerable to XSS attacks but it's harder for the attacker to do the attack when you're using httpOnly cookies.
- Cookies are vulnerable to CSRF attacks but it can be mitigated using sameSite flag and anti-CSRF tokens.
  You can still make it work even if you need to use the Authorization: Bearer header or if your JWT is larger than 4KB. This is also consistent with the recommendation from the OWASP community:

  > Do not store session identifiers in local storage as the data are always accessible by JavaScript. Cookies can mitigate this risk using the httpOnly flag.

- **Explain 3rd party cookies.**
  Third-party cookies are cookies that are set by a website other than the one you are currently on.

- **How do pixel tags work?**

You add the tracking pixel using a code in your site's HTML code or email, which contains an external link to the pixel server. When someone visits your website, the HTML code is processed by their browser, which follows the link and opens the hidden graphic.

---

### Document the following Vocabulary Terms

- **cookies** Cookies are small pieces of data stored as text on the client's computer. Normally cookies are used only to store small amounts of data, including user preferences, time and more. Even though cookies are not harmful some people do not permit cookies due to concerns about their privacy.its used to identify your computer as you use a computer network. Data stored in a cookie is created by the server upon your connection. This data is labeled with an ID unique to you and your computer.

- **authorization** Authorization is the process of giving someone permission to do or have something. and its a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features.

- **access control** Access control is a security technique that regulates who or what can view or use resources in a computing environment.

- **conditional rendering** Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false. In React, it allows us to render different elements or components based on a condition

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

Redux is an open-source JavaScript library for managing application state. It is most commonly used with libraries such as React or Angular for building user interfaces.
Redux is a predictable state container for JavaScript apps.

- Redux provides a solid, stable, and mature solution to managing state in your React application.
- Centralizing your application's state and logic enables powerful capabilities like undo/redo
- The Redux DevTools make it easy to trace when, where, why, and how your application's state changed. Redux's architecture lets you log changes, use "time-travel debugging", and even send complete error reports to a server.

Testing redux reducers with Jest

Usually reducer consists of initial state and switch statement to handle every action.  
break down my store into different sub-stores and have separate reducers for each sub-store.  
Sometimes one switch/case may handle few actions, because the business logic is the same and outcome should be the same.  
Some example GET_POST and UPDATE_POST should update the same store and produce same outcome.
it starts with boilerplate setup and writing empty tests just to outline what needs to be tested.  
test the initial state and then every switch/case in the reducer to see if action.payload will produce expected store.

