## Fizz Buzz
Return an array containing the numbers from 1 to N, where N is the parametered value. N will never be less than 1 (in C#, N might be less than 1).
<br/>

* C# ONLY: If N is smaller than or equal to 0, throw an ArgumentOutOfRangeException!

Replace certain values however if any of the following conditions are met:
<br/>

* If the value is a multiple of 3: use the value 'Fizz' instead
* If the value is a multiple of 5: use the value 'Buzz' instead
* If the value is a multiple of 3 & 5: use the value 'FizzBuzz' instead
<br/>

C# method calling example:

`string[] result = FizzBuzz.GetFizzBuzzArray(3); // => [ "1", "2", "Fizz" ]`

<br/>

**My solution**

```
function fizzbuzz(n) {
  let str = '';
  let arr = [];

  for(let i = 1;  i < n;  i++) {
    if ((i % 3 === 0) && (i % 5 === 0)) {
      str = 'FizzBuzz';
      arr.push(str);
    } else if (i % 5 === 0) {
      str = 'Buzz';
      arr.push(str);
    } else if( i % 3 === 0) {
      str = 'Fizz';
      arr.push(str);
    } else {
     arr.push(i);
    }
  }

  return arr;
}

fizzbuzz(10);
```