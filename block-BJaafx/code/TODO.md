1. Using loops take 10 inputs from user and find the average of all the numbers.
let sum=0
for (i=0;i<10;1++){
  ask=Number(prompt("Enter a number"));
  sum=sum+ask
}
avg=sum/10
console.log(avg)

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
No Output printLn is not a standard function is js

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

function getEvenSum(max){
  let sum=0
  for (let i=0;i<max+1;i++){
    if (i%2==0){
      sum=sum+i
    }
  }
  return sum
}


4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

function getOddSum(max){
  let sum=0
  for (let i=0;i<max+1;i++){
    if (i%2!=0){
      sum=sum+i
    }
  }
  return sum
}


5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

function getProductOFDigits(num){
  let mul=1;
  pum=String(num)
  if (pum.length==1 && num>0){
    return num
  }
  else if(num<0){
    return "Not a valid input"
  }
  else if (pum.length>1 && num>0){
    for (i=0;i<pum.length;i++){
      mul=mul*Number(pum[i])
    }
    return mul
  }
}


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

check(10); // Bigger than 5, because num>5.
check(1); // Smaller than 5, because num<5.>
check(5); // Output is 5. it is not bigger or small.
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // You are arya
getOutput('John'); // You are John
getOutput(); // Who are you
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // Who are you
getOutput('John'); // Who are you
getOutput(); // Who are you
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
Yes it can have multiple, if there are mutiple conditions in the function. If any condition is met it would have a specific return.


10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
for loop sets the variable to a value and then executes as long as a condition is met and then increments or decrements value form the variable. While loop just executes as long as a condition is met. For loop is used when we know the value of the end of the process. While loop is used when we dont know what is the end value of the process.

for example:
sum of 1 to 10 would use For loop.
make a loop to count how many phone we can buy as long as the final price is less than 200,000. We would use while loop here.