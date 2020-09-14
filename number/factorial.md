## Factorial
In mathematics, the factorial of a non-negative integer n, denoted by n!, is the product of all positive integers less than or equal to n. For example: 5! = 5 * 4 * 3 * 2 * 1 = 120. By convention the value of 0! is 1.
<br/>

Write a function to calculate factorial for a given input. If input is below 0 or above 12 throw an exception of type `RangeError`.

<br/>

**My solution**

```
function factorial(n) {
  let factorial = 1;

  if (n < 0 || n > 12) { throw new RangeError() };

  for(let i = n; i > 0; i-- ) {
    factorial *= i; 
  };

  return factorial ;
};
```
