# Read: Class 04 :  React and Forms 

- - - 

## Article : React Docs - Forms
   
* What is a ‘Controlled Component’?  

A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange 
   
* Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

* How do we target what the user is entering if we have an event handler on an input field?

event.target.any
   
- - - 

## Article : The Conditional (Ternary) Operator Explained
   
* Why would we use a ternary operator?
 
 to simplify your if-else statements that are used to assign values to variables
   
* Rewrite the following statement using a ternary statement 

```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

```

x===y? true
         : false

```

- - - 

## Things I want to know more about   

- - - 
