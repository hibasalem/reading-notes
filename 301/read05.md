# Read: Class 05 :  Putting it all together

- - - 

## Article : React Docs - thinking in React
   
* ***How would you break a mock into a component heirarchy?***     

   first we try to know what component do we have then the components that appear within another component in the mock should appear as a child in the hierarchy

* ***What is the single responsibility principle and how does it apply to components?***    
   There should never be more than one reason for a class to change." In other words, every class should have only one responsibility.

* ***What does it mean to build a ‘static’ version of your application?***   
 build a version that doesnt use any states , only props so it have no interactivity

* ***Once you have a static application, what do you need to add?***    
state 

* ***What are the three questions you can ask to determine if something is state?***   

1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.


* ***How can you identify where state needs to live?***    

   For each piece of state in your application:

1. Identify every component that renders something based on that state.
2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
3. Either the common owner or another component higher up in the hierarchy should own the state.
4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
   
- - - 

### the thought process of building a searchable product data table using React. 

 ***DRY: Don’t Repeat Yourself***   

* Start With A Mock

* Break The UI Into A Component Hierarchy

* Build A Static Version in React

* Identify The Minimal (but complete) Representation Of UI State

* Identify Where Your State Should Live
 
* Add Inverse Data Flow

- - - 


## Things I want to know more about   

- - - 
