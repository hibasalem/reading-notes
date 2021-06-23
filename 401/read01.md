# Read: Class 01 : Node Ecosystem, TDD, CI/CD

- - - 

## Review, Research, and Discussion  

* ***Describe (in plain English) what Array.map() does***   


    The array.map() iterates over an array and runs a call back for each element , The callback receives the value and the index of the array element as a parameter. always return a **new array** of the **same length** as the original array.    

* ***Describe (in plain English) what Array.reduce() does***  
 
     The `array.reduce()` function iterates over an array and runs a call back for each element. The callback receives the accumalator, the value and the index of the array element as parameters.The original array will never be harmed, The accumaltor is a placeholder for what you want to return when the callback iteration is done running.

* ***Provide code snippets showing how to use superagent() to fetch data from a URL and log the result***
    * With normal Promise .then() syntax
    * Again with async / await syntax

  i am more familer with **axios** so iam using axios in the examples   

**normal Promise.then() syntax** 

```
    functionName = () => {
     axios.get(ApiLink).then((result) => {
     // code block doing something with the result
      });
     };
```

**async / await syntax**  

```
   functionName = async () => {
    let allData = await axios.get(ApiLink);
    // code block doing something with the allData
   };

```
 
* ***Explain promises as though you were mentoring a Code 301 level student***

    **I Promise a Result!**   

   **Producing code** is code that can take some time    

  A Promise is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action's eventual success value or failure reason.    
 
  The methods promise.then(), promise.catch(), and promise.finally() are used to associate further action with a promise that becomes settled.   
 
* ***Are all callback functions considered to be Asynchronous? Why or Why Not?***

  no , Argument function can be called synchronously , function is asynchronous when it perform an asynchronous operation( incorporate the argument callback in handling the results of this asynchronous operation).

- - - 
