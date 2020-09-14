## Greatest common divisor
Find the greatest common divisor of two positive integers. The integers can be large, so you need to find a clever solution.
<br/>

The inputs `x` and `y` are always greater or equal to 1, so the greatest common divisor will always be an integer that is also greater or equal to 1.

<br/>

**My solution**

```
function mygcd(x,y) {
  let i = x;

  while (x % i !== 0 || y % i !== 0) {
    i = i - 1;
  };

  return i;
};
```
