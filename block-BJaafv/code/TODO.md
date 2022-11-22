1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}
 In the above code `return` will execute the caller `function` values
// second
function sum(a, b) {
  console.log(a + b);
}
 In the above code console.log it will print the output in the browsers console
```

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
  sum of a+b will be the value of first and second.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   If we pass thre parameters to first function like numbers only then the name of the function will be error and it will not be defined

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
  yes we can store in a variable `add` after calling the function its going to return the value so we can declare variable and store in it

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
  ```js
  function sayHello(name){
    return `Hello ${name}`;
  }
    sayHello("Arya")
    ```

6. What will be the output of the function below and why?
   output is 'Hello, John' the userName is declared outside the function so we can acces it inside the function.so it returned the message including the userName.
```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1  John

showMessage(); // Output 2    'Hello, John'

alert(userName); // Output 3 John
```

8. What is a Anonymous Function give example of three functions.
  Anonymous function is function that does not associate with the function name.
  example 1 
  ```js 
  let add = function (a,b){
    return 12+13;        
  }
  add();
  ```
  example 2
  ```js 
  let fullName = function(firstName,lastName){
    return firstName + lastName;
  }
  fullName()
  ```
   example 3
   ```js
   let sayHello = function (name){
    return `Hello ${name}`;
  }
    sayHello("Arya")
   ```
9. Can function declaration be a Anonymous Function? Explain
   function declaration and Anonymous function has almost same syntax only the difference is name of function can be omitted in the ananymous function
10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
"full" 
"user"  
"make" 
"apply"
"set"