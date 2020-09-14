## Find The Duplicated Number in a Consecutive Unsorted List
You are given an array of `n+1` integers `1` through `n`. In addition there is a single duplicate integer.
<br/>

The array is unsorted.
<br/>

An example valid array would be `[3, 2, 5, 1, 3, 4]`. It has the integers `1` through `5` and `3` is duplicated. `[1, 2, 4, 5, 5]` would not be valid as it is missing `3`.
<br/>

You should return the duplicate value as a single integer.

<br/>

**My solution**

```
function findDup( arr ){
  arr.sort();
  let duplicateValue;

  for (let i = 0; i < arr.length - 1; i++) {
      if (arr[i + 1] === arr[i]) {
          duplicateValue = arr[i];
      };
  };

  return duplicateValue;
};
```
