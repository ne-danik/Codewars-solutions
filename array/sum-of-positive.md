## Sum of positive
You get an array of numbers, return the sum of all of the positives ones.
<br/>

Example `[1,-4,7,12]` => `1 + 7 + 12 = 20`
<br/>

*Note:* if there is nothing to sum, the sum is default to `0`.

<br/>

**My solution**

ver.1
```
function positiveSum(arr) {
  let newarr = [];

  for(let i = 0; i < arr.length; i++) {
    if(arr[i] > 0 ) {
      newarr.push(arr[i]);
    };
  };

  let sum = 0;
  for (let index of newarr) {
    sum += index;
  };
  
  return sum;
};
```

ver.2
```
function positiveSum(arr) {
   return arr.reduce((a,b)=> a + (b > 0 ? b : 0),0);
};
```
