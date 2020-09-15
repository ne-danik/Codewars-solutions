## Square Every Digit
Square every digit of a number and concatenate them.
<br/>

For example, if we run `9119` through the function, `811181` will come out, because 9<sup>2</sup> is 81 and 1<sup>2</sup> is 1.
<br/>

*Note:* The function accepts an integer and returns an integer

<br/>

**My solution**

```
function squareDigits(num){
  return Number(String(num).split('').map((a) => Math.pow(a, 2)).join(''));
}
```
