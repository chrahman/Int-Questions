# Frontend Int Questions

## HTML questions

1. Symentic Elements?

    **Answer:** Symentic elements are the elements that describes its own value or purpose. Like `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`. These elements are directly understandable by Developer and search engines.
    
2. New Tags in HTML?

    **Answer:** HTML5 introduced several new tags, including `<article>`, `<aside>`, `<audio>`, `<datalist>`, `<details>`, `<embed>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<source>`, `<summary>`, `<time>`, `<track>`, and `<video>`.
    
3. Legend tag?

    **Answer:** The `<legend>` tag is used to provide a caption or title for a `<fieldset>` element, which is a grouping of related form controls.
    
4. pre tag?

    **Answer:** The `<pre>` tag is used to define preformatted text, It is mostly used for displaying code snippets or other content where formatting is important.
    
5. Block level elements in HTML

    **Answer:** Block level elements are those elements that starts from new line by defualt and that take up the full width available to them and create a line break. like `<div>`, `<p>`, `<h1> to <h6>`, `<ul>`, `<ol>`, `<table>` and `<form>`.
    
6. What is the difference between the  `<b>` and `<strong>` tags?

    **Answer:** The `<b>` tag is used to apply bold formatting to text, while the `<strong>` tag is used to indicate that the text is of particular importance or significance. The `<strong>` tag is semantically more meaningful than the `<b>` tag and may be given more weight by search engines and other user agents.

## CSS Questions

1. Positions,diffrences like parent child
2. Difference between, inline-block & block
3. Difference between, overflow:hidden & block
4. Mobile 1st approach &  responsivnesss
5. Why we use css framworks rather than Grid system

## JavaScript Questions

1. Is JS single threaded or multi threaded?

   **Answer:** JavaScript is single-threaded, and all the JavaScript code executes in a single thread.
   
2. Is JS synchronous or asynchronous?

   **Answer:** By default, JavaScript is a synchronous, single-threaded, and blocking programming language.
   
3. How can we make a function that works like multithreading?

   **Answer:** We can use JS as multithreading using Web Workers API, or asynchronous programming using promises.
   
4. How many versions are introduced in JS?

   **Answer:**
   - ES1 (released in 1997)
   - ES2 (released in 1998)
   - ES3 (released in 1999)
   - ES4 (never released)
   - ES5 (released in 2009)
   - ES6/ES2015 (released in 2015)
   - ES7/ES2016 (released in 2016)
   - ES8/ES2017 (released in 2017)
   - ES9/ES2018 (released in 2018)
   - ES10/ES2019 (released in 2019)
   - ES11/ES2020 (released in 2020)
   - ES12/ES2021 (released in 2021)
   
5. What is the difference between var, let, and const?

   **Answer:**
   - In `var`, we can redeclare the same variable and reassign its value.
   - In `let`, we cannot redeclare the same variable but can reassign its value.
   - In `const`, we cannot redeclare the same variable and cannot reassign its value.
   
6. What are the scopes in JS (Local and Global Scope)?

   **Answer:**
   - The scope in which variables are declared in a code block or function is called the local scope. 
   - The scope in which a variable is declared outside of a function is called the global scope. This variable is accessible throughout the program.
7. What is hoisting in JS?

   **Answer:** Hoisting is a mechanism in JS where functions and variables are moved to the top of their respective scopes before runtime.
   
8. What is the difference between an Arrow Function and a Simple Function, and how does `this` work in them?

   **Answer:** A simple/regular function can bind its own `this`. However, an arrow function in ES6 cannot bind its own `this`.
   
9. What is a callback function?

   **Answer:** A callback function is a function that is passed as an argument to another function and is called when that function is executed.
   ``` javascript
   function doSomethingAsync(callback) {
     // simulate an asynchronous operation
     setTimeout(function() {
       console.log("Async operation done.");
       callback();
     }, 1000);
   }

   function callbackFunction() {
     console.log("Callback function executed.");
   }

   doSomethingAsync(callbackFunction);
   ```
   
10. What are Promises?

    **Answer:** A Promise is an object that represents a value that may not be available yet, but will be at some point in the future. Promises are commonly used to handle network requests. A Promise has three states: pending, fulfilled, or rejected.
    
11. What is a Generator Function, and how does `yield` work in it?

    **Answer:** A generator function is a special type of function in JavaScript that allows you to pause and resume the execution of a function. When you use the yield keyword inside a generator function, it pauses the execution of the function and returns a value to the iterator. The next time you call the next() method on the iterator, the function resumes execution from the point where it left off.
    ``` javascript
    function* numberGenerator() {
      yield 1;
      yield 2;
      yield 3;
    }

    const iterator = numberGenerator();

    console.log(iterator.next()); // { value: 1, done: false }
    console.log(iterator.next()); // { value: 2, done: false }
    console.log(iterator.next()); // { value: 3, done: false }
    console.log(iterator.next()); // { value: undefined, done: true }
    ```
    
12. Aysnc & await?

    **Answer:** Async is used to behave a function like Asyncronus, await is used for waiting a process.

13. Closure?

    **Answer:** Return a Function from inside function is called Closure and the inner function has access to the outer function's variables and parameters. A closure allows the inner function to "remember" the environment in which it was created, even after the outer function has returned.
    ``` javascript
    function outerFunction() {
      const message = "Hello, ";

      function innerFunction(name) {
        console.log(message + name);
      }

      return innerFunction;
    }

    const helloFunction = outerFunction();
    helloFunction("John"); // "Hello, John"
    helloFunction("Jane"); // "Hello, Jane"

    ```
    
14. Event Loop? 

    **Answer:** Event Loop has a one simple job to moniter the Global execution stack and message queue.
    
15. Event Queue?

    **Answer:** Event Queue is responsible for sending new functions to the stack for processing.
    
16. Stack, Hash, Map?

    **Answer:** Stack, Hash, and Map are data structures commonly used in JavaScript for storing and manipulating data.
	- A `Stack` is a data structure that follows the Last-In-First-Out (LIFO) principle. It is similar to a stack of plates, where the last plate you put on top is the first one you take off. In JavaScript, you can implement a stack using an array and the built-in methods push() and pop().
	- A `Hash` is a data structure that maps keys to values. It is also known as a hash table or a dictionary. Hashes are commonly used for fast data lookup and retrieval. In JavaScript, you can implement a hash using an object literal, where the keys represent the data you want to store, and the values represent the corresponding values.
	- A `Map` is a data structure that also maps keys to values, but it allows any type of key, not just strings. It is similar to a Hash, but with more flexibility. Maps are commonly used for complex data structures and algorithms. In JavaScript, you can implement a Map using the built-in Map object.
    ``` javascript
    // Stack
    const stack = [];
    stack.push(1);
    stack.push(2);
    stack.push(3);
    console.log(stack.pop()); // 3
    console.log(stack.pop()); // 2
    console.log(stack.pop()); // 1

    // Hash
    const hash = {
      name: "John",
      age: 30,
      gender: "Male"
    };
    console.log(hash.name); // "John"
    console.log(hash.age); // 30
    console.log(hash.gender); // "Male"

    // Map
    const map = new Map();
    map.set("name", "John");
    map.set("age", 30);
    map.set("gender", "Male");
    console.log(map.get("name")); // "John"
    console.log(map.get("age")); // 30
    console.log(map.get("gender")); // "Male"
    ```
    
    
## HTML Questions

Index | Question      | Answer |
------| ----------- | ----------- |
1     | Symentic Elements      | Symentic elements are the elements that describes its own value or purpose. Like `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`. These elements are directly understandable by Developer and search engines.       |
2     | New Tags in HTML   | HTML5 introduced several new tags, including `<article>`, `<aside>`, `<audio>`, `<datalist>`, `<details>`, `<embed>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<source>`, `<summary>`, `<time>`, `<track>`, and `<video>`.        |
3     | `<legend>`  tag   | The `<legend>` tag is used to provide a caption or title for a `<fieldset>` element, which is a grouping of related form controls.       |
4     | `<pre>` tag  | The `<pre>` tag is used to define preformatted text, It is mostly used for displaying code snippets or other content where formatting is important.    |
5     | Block level elements in HTML   | Block level elements are those elements that starts from new line by defualt and that take up the full width available to them and create a line break. like `<div>`, `<p>`, `<h1> to <h6>`, `<ul>`, `<ol>`, `<table>` and `<form>`.        |
6    | Difference between the  `<b>` and `<strong>` tags   | The `<b>` tag is used to apply bold formatting to text, while the `<strong>` tag is used to indicate that the text is of particular importance or significance. The `<strong>` tag is semantically more meaningful than the `<b>` tag and may be given more weight by search engines and other user agents.        |

## CSS Questions
Index | Question      | Answer |
------| ----------- | ----------- |
1    | Positions,diffrences like parent child   | HTML5 introduced several new tags, including `<article>`, `<aside>`, `<audio>`, `<datalist>`, `<details>`, `<embed>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<source>`, `<summary>`, `<time>`, `<track>`, and `<video>`.        |
2   | Difference between, overflow:hidden & block   | HTML5 introduced several new tags, including `<article>`, `<aside>`, `<audio>`, `<datalist>`, `<details>`, `<embed>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<source>`, `<summary>`, `<time>`, `<track>`, and `<video>`.        |
3   | Difference between, inline-block & block   | HTML5 introduced several new tags, including `<article>`, `<aside>`, `<audio>`, `<datalist>`, `<details>`, `<embed>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<source>`, `<summary>`, `<time>`, `<track>`, and `<video>`.        |
4   | Mobile 1st approach &  responsivnesss  | HTML5 introduced several new tags, including `<article>`, `<aside>`, `<audio>`, `<datalist>`, `<details>`, `<embed>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<source>`, `<summary>`, `<time>`, `<track>`, and `<video>`.        |
5   | Why we use css framworks rather than Grid system   | HTML5 introduced several new tags, including `<article>`, `<aside>`, `<audio>`, `<datalist>`, `<details>`, `<embed>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<source>`, `<summary>`, `<time>`, `<track>`, and `<video>`.        |

## Javascript Questions
Index | Question      | Answer |
------| ----------- | ----------- |
1    | Is JS single threaded or multi threaded?   | JavaScript is single-threaded, and all the JavaScript code executes in a single thread.       |
2   | Is JS synchronous or asynchronous?   | By default, JavaScript is a synchronous, single-threaded, and blocking programming language.     |
3   |  How can we make a function that works like multithreading?  | We can use JS as multithreading using Web Workers API, or asynchronous programming using promises.      |
4   | How many versions are introduced in JS? |  <ul><li>ES1 (released in 1997)</li> <li>ES2 (released in 1998)</li> <li>ES3 (released in 1999)</li> <li>ES4 (never released)</li> <li>ES5 (released in 2009)</li> <li>ES6/ES2015 (released in 2015)</li> <li>ES7/ES2016 (released in 2016)</li> <li>ES8/ES2017 (released in 2017)</li> <li>ES9/ES2018 (released in 2018)</li> <li>ES10/ES2019 (released in 2019)</li> <li>ES11/ES2020 (released in 2020)</li><li>ES12/ES2021 (released in 2021)</li></ul>       |
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |
6  | What are the scopes in JS (Local and Global Scope)?   |<ul> <li> The scope in which variables are declared in a code block or function is called the local scope.</li> <li> The scope in which a variable is declared outside of a function is called the global scope. This variable is accessible throughout the program. </li></ul>        |
7 | What is hoisting in JS?   |Hoisting is a mechanism in JS where functions and variables are moved to the top of their respective scopes before runtime.        |
8| What is the difference between an Arrow Function and a Simple Function, and how does `this` work in them?   |A simple/regular function can bind its own `this`. However, an arrow function in ES6 cannot bind its own `this`.       |
9  | What is a callback function?   |A callback function is a function that is passed as an argument to another function and is called when that function is executed. [callback example](#callback-example)|
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |

## Callback example
   ``` javascript
   function doSomethingAsync(callback) {
     // simulate an asynchronous operation
     setTimeout(function() {
       console.log("Async operation done.");
       callback();
     }, 1000);
   }

   function callbackFunction() {
     console.log("Callback function executed.");
   }

   doSomethingAsync(callbackFunction);
   ```
