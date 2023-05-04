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
------| ------------- | ------- |
1    | What are CSS Positions   | CSS positions allow you to control the placement and layout of HTML elements on a webpage. There are five different position values that can be used in CSS: `Static`, `relative`, `absolute`, `fixed`, `sticky` |
2   | Position `static`   | This is the default position value for all elements. It means that the element will be positioned in the normal and cannot be moved or manipulated using the other position values. |
3   | Position `relative`   | This position value allows you to position an element relative to its normal position. You can use the `top`, `right`, `bottom`, and `left` properties to adjust the position of the element. |
3   | Position `absolute`   | This position value allows you to position an element relative to its nearest positioned ancestor element. If there is no positioned ancestor, the element will be positioned relative to the body of the document. You can use the `top`, `right`, `bottom`, and `left` properties to adjust the position of the element. |
3   | Position `fixed`   | An element with position: `fixed` is positioned relative to the viewport/browser window, which means it always stays in the same place even if the page is scrolled. The `top`, `right`, `bottom`, and `left` properties are used to position the element. |
3   | Position `sticky`   | An element with `position: sticky;` is positioned based on the user's scroll position. A `sticky` element toggles between `relative` and `fixed`, depending on the scroll position. It is positioned `relative` until a given offset position is met in the viewport - then it **sticks** in place (like `position:fixed`). |
2   | Difference between, `overflow:hidden` & `scroll`   | `overflow: hidden` hides any content that overflows the container and does not provide a scrollbar, while `overflow: scroll` also hides any content that overflows the container but provides a scrollbar for the user to access the hidden content. |
3   | Difference between, `display:inline-block` & `block`  | In `display: block` the element takes up the full width of its container and creates a new line after the element, while `display: inline-block` only takes up as much width as necessary and but not create new line and keeps element inline |
4   | Mobile 1st approach &  responsivnesss  | Mobile-first approach means designing and developing a website for mobile devices first, and then scaling it up for larger screens. while responsiveness refers to a website's ability to adapt and adjust its layout to different screen sizes and resolutions. |
5   | Why we use css framworks rather than Grid system   | CSS frameworks offer more than just a grid system, including pre-designed UI components and styles that can help ensure consistency and speed up development time. |

## Javascript Questions
Index | Question      | Answer |
------| ----------- | ----------- |
1    | Is JS single threaded or multi threaded?   | JavaScript is single-threaded, and all the JavaScript code executes in a single thread.       |
2   | Is JS synchronous or asynchronous?   | By default, JavaScript is a synchronous, single-threaded, and blocking programming language.     |
3   |  How can we make a function that works like multithreading?  | We can use JS as multithreading using Web Workers API, or asynchronous programming using promises.      |
4   | How many versions are introduced in JS? |  <ul><li>ES1 (released in 1997)</li> <li>ES2 (released in 1998)</li> <li>ES3 (released in 1999)</li> <li>ES4 (never released)</li> <li>ES5 (released in 2009)</li> <li>ES6/ES2015 (released in 2015)</li> <li>ES7/ES2016 (released in 2016)</li> <li>ES8/ES2017 (released in 2017)</li> <li>ES9/ES2018 (released in 2018)</li> <li>ES10/ES2019 (released in 2019)</li> <li>ES11/ES2020 (released in 2020)</li><li>ES12/ES2021 (released in 2021)</li></ul> |
5   | What is the difference between var, let, and const?   |<ul> <li> In `var`, we can redeclare the same variable and reassign its value. </li> <li> In `let`, we cannot redeclare the same variable but can reassign its value. </li> <li> In `const`, we cannot redeclare the same variable and cannot reassign its value. </li></ul>        |
6  | What are the scopes in JS (Local and Global Scope)?   |<ul> <li> The scope in which variables are declared in a code block or function is called the local scope.</li> <li> The scope in which a variable is declared outside of a function is called the global scope. This variable is accessible throughout the program. </li></ul>        |
7 | What is hoisting in JS?   |Hoisting is a mechanism in JS where functions and variables are moved to the top of their respective scopes before runtime.        |
8| What is the difference between an Arrow Function and a Simple Function, and how does `this` work in them?   |A simple/regular function can bind its own `this`. However, an arrow function in ES6 cannot bind its own `this`.       |
9  | What is a callback function?   |A callback function is a function that is passed as an argument to another function and is called when that function is executed. [callback example](#callback-example)|
10   | What are Promises?   | A Promise is an object that represents a value that may not be available yet, but will be at some point in the future. Promises are commonly used to handle network requests. A Promise has three states: pending, fulfilled, or rejected.       |
11   | What is a Generator Function, and how does `yield` work in it?  | A generator function is a special type of function in JavaScript that allows you to pause and resume the execution of a function. When you use the yield keyword inside a generator function, it pauses the execution of the function and returns a value to the iterator. The next time you call the next() method on the iterator, the function resumes execution from the point where it left off.  [Generator Function example](#generator-function)    |
12   | Aysnc & await?   | Async is used to behave a function like Asyncronus, await is used for waiting a process. |
13   | What is Closure?   | Return a Function from inside function is called Closure and the inner function has access to the outer function's variables and parameters. A closure allows the inner function to "remember" the environment in which it was created, even after the outer function has returned. [Closure example](#closure-example) |
14   | Event Loop?    | Event Loop has a one simple job to moniter the Global execution stack and message queue. |
15   | Event Queue?  | Event Queue is responsible for sending new functions to the stack for processing. |
16   | Stack, Hash, Map?  | <ul> <li> A `Stack` is a data structure that follows the Last-In-First-Out (LIFO) principle. It is similar to a stack of plates, where the last plate you put on top is the first one you take off. In JavaScript, you can implement a stack using an array and the built-in methods push() and pop(). </li> <li> A `Hash` is a data structure that maps keys to values. It is also known as a hash table or a dictionary. Hashes are commonly used for fast data lookup and retrieval. In JavaScript, you can implement a hash using an object literal, where the keys represent the data you want to store, and the values represent the corresponding values. </li> <li> A `Map` is a data structure that also maps keys to values, but it allows any type of key, not just strings. It is similar to a Hash, but with more flexibility. Maps are commonly used for complex data structures and algorithms. In JavaScript, you can implement a Map using the built-in Map object. </li></ul> [Stack, Hash, Map example](#stack-hash-map)|
17   | `SetTimeOut`  | `SetTimeOut` is web API for setting a timer to execute a code after the timer expires. |
18   | `SetIntervel`  | `SetIntervel` repeatedly calls a function or executes a code snippet with a fixed time delay. |
19   | Destructureing  | Object destructuring is a useful JavaScript feature to extract values from arrays or properties from objects and bind them to variables. |
20   | In JS can we use `map()` on object?  | Yes we can use the `map()` method on an object, but only on its keys or values, not on the object itself. |
21   | Difference between `forEach()` and `map()`  | `forEach()` and `map()` iterate over arrays, but `forEach()` modifies oringnal array & `map()` returns new array. |
22   | Function recursion  | A recursive function is a function that calls itself somewhere within the body of the function. |

### Callback example
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
   
### Generator function
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

### Closure example
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

### Stack, Hash, Map
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
