## Is a number prime?
Define a function that takes one integer argument and returns logical value `true` or `false` depending on if the integer is a prime.
<br/>

Per Wikipedia, a prime number (or a prime) is a natural number greater than 1 that has no positive divisors other than 1 and itself.
<br/>

**Requirements**

You can assume you will be given an integer input.
You can not assume that the integer will be only positive. You may be given negative numbers as well (or `0`).
*NOTE on performance*: There are no fancy optimizations required, but still the most trivial solutions might time out. Numbers go up to 2^31 (or similar, depends on language version). Looping all the way up to `n`, or `n/2`, will be too slow.

**Example**

```
is_prime(1)  /* false */
is_prime(2)  /* true  */
is_prime(-1) /* false */
```

<br/>

**My solution**

1.
```
function isPrime(num) {
  for(let i = 2, s = Math.sqrt(num); i <= s; i++) {
    if(num % i === 0) {
      return false;
    }
  }
  return num > 1;
}
```

2.
```
function isPrime(num) {
  let j = 0;
  let i = 2;

  while(((i * i) <= num) && j !== 1) {
      if (num % i === 0) { 
        j = 1;
        i += 1;
      } else {
        i += 1;
      }
  }

  if(j === 1) {
    return `i ${i} j ${j} ${num} is not prime`;
  } else {
    return `i ${i} j ${j} ${num} is prime`;
  }
}

isPrime(2);
```
