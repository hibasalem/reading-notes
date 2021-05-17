# Read: Class 03 :  Passing Functions as Props

- - - 

## Article : Lists and Keys
   
* What does .map() return?  
   
  it return th output of the callback function into an array    
   
* If I want to loop through an array and display each value in JSX, how do I do that in React? 

> ```   
>function List() {
>  const listItems = item.map((item) =>
>    <li key={item}>
>      {item}
>    </li>
>  );
>  return (
>    <ul>{listItems}</ul>
>  );
> }
>
> ReactDOM.render(
>  <itemList item={item} />,
> );
> ```

* Each list item needs a unique ***key***.   
   

* What is the purpose of a key?
     
  Keys help React identify which items have changed, are added, or are removed.
     
- - - 

## Article : The Spread Operator    
    
* What is the spread operator? 
   
  > The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

  ```
  …
  ```
   
* List 4 things that the spread operator can do. 
    
  1.Copying an array
  2.Concatenating or combining arrays
  3.Using Math functions
  4.Using an array as arguments
  5.Adding an item to a list
  6.Adding to state in React
  7.Combining objects
  8.Converting NodeList to an array
    
* Give an example of using the spread operator to combine two arrays.   
    
> ```
> const arr1 = [1,2,3]
> const arr2 = [4,5,6]
> const arr3 = [...arr1, ...arr2] //arr3 ==> [1,2,3,4,5,6]
> ```
   

* Give an example of using the spread operator to add a new item to an array. 
   
> ```
> let a = [1, 2, 3, 4, 5];
> let b = [0, ...a]; 
> ```  
  
* Give an example of using the spread operator to combine two objects into one.

> ```
> const person = { name: 'David Walsh', gender: 'Male' };
> const tools = { computer: 'Mac', editor: 'Atom' };
> const summary = {...person, ...tools};
> /*
> Object {
>   "computer": "Mac",
>   "editor": "Atom",
>   "gender": "Male",
>   "name": "David Walsh",
> }
> * /
>```
- - - 

## Videos : How to Pass Functions Between Components  
    
* In the video, what is the first step that the developer does to pass functions between components?
  
  creat the function to pass an object , 

* In your own words, what does the increment function do?
  
  updating the value of the counts based on the name that passed in 
 

* How can you pass a method from a parent component into a child component?  
   
  The function is passed as a prop to a child component

* How does the child component invoke a method that was passed to it from a parent component?
  
  onClick 


### the data flows during this : 

   * A parent component defines a function
   * The function is passed as a prop to a child component
   * The child component then invokes the prop
   * The parent function is then called, usually changing something
   * Then the parent component is re-rendered along with its children
    

- - - 

## Things I want to know more about   

- - - 
