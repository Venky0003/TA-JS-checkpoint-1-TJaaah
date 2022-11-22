1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
var nums = new Array(10);
var input = prompt('Enter ' + (nums.length + 1) + ' numbers separated by commas:');
var values = input.split(',');
if (values.length == nums.length){
  
  for (var i = 0; i < nums.length; i++){
    
    nums[i] = new Number(values[i]);
  }
}
let sum = 0;
for(let j=0;j<=nums.length;j++){
  sum += j;
}
console.log(sum/10);
```
2. What will be the output of the code below
 error since the println is not defined.
```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum(max = 10){
  let sum = 0;
  for(let i = 1;i <= max;i++){
    if(i % 2 === 0){
      sum +=i;
    }
    
  }console.log(sum);
}getEvenSum();
```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max = 10){
  let sum = 0;
  for(let i = 1;i <= max;i++){
    if(i % 2 !== 0){
      sum +=i;
    }
    
  }console.log(sum);
}getOddSum();
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.
```js
function getProductOfDigits(num){
  let mul = 1;
  if(num>=1){
  for(let i = 1;i <= num;i++){
   
      mul *=i;
    }
   return mul;
  }
  else {
    return(`not a valid input`);
  }
}getProductOfDigits();
```
- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // output 'Bigger than 5' since the greater than operator has been used and num value is 10 graeter than 5. 
check(1); // output   'Smaller than 5'since the lesser than operator has been used and num value is 1 lesser than 5. 
check(5); // output   5 will be returned since it will not pass above two conditions.
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}
 
getOutput('Arya'); // what will be the output  'You are arya'   condition one passes the value with it triple equals 
getOutput('John'); // what will be the output   'You are john'   condition two passes the value with it triple equals 
getOutput(); // what will be the output          'Who are you'    since it has no value 
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // what will be the output  'You are arya' 'Who are you' here console.log prints and return returns a value
getOutput('John'); // what will be the output   'You are john' 'Who are you' here console.log prints and return returns a value
getOutput(); // what will be the output         'Who are you' it has no value since
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
function can have multiple return satements but only based on conditions it runs
example 1
```js
function EvenOrNot(num){
if(num % 2 === 0){
  return `Number is even`
}
else{
  return `Number is odd`
}
}
```

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
for loop is used when the number of iterations are known and while loop is used when the number of iterations are not known
example 1 
```js
let sum = 0;
for(let i = 0;i <= 10; i++){
    sum += i;
}
while(i<num){
  sum +=i;
  i++;
}
```
