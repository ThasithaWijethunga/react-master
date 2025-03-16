
1. What are the three states of a Promise?

    Pending
    Fulfilled
    Rejected


2. How does the async keyword affect a function's return value?

    When a function is declared with the async keyword, that automatically returns a Promise.
    If the function returns a value, JavaScript wraps it in a resolved Promise. 
    If the function throws an error, JavaScript wraps it in a rejected Promise. 


3. Explain the purpose of the await keyword.

   The await keyword is used inside an async function to pause execution until a Promise resolves.
   
4. What is a callback function and how is it used in asynchronous operations?

   callback function is a function that is passed as an argument to another function and executed later.

5. Describe the role of the event loop in JavaScript.

   An event loop is a mechanism that allows Javascript to handle asynchronous tasks efficiently.

6. Write a function called delayedGreeting that takes a name as an argument and logs a greeting message to the console after a 2-second delay using setTimeout. Use a callback function to   achieve this.

  const delayedGreeting = ( name, callback) => {
    setTimeout( () => {
        callback(name);
    },2000);
  };  
   

  const printName = (name) => {
     console.log(`hello ${name}`);
  };

  delayedGreeting("Thasitha",printName); 

    
   