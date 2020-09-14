## Remove duplicates from list
Define a function that removes duplicates from an array of numbers and returns it as a result.
<br/>

The order of the sequence has to stay the same.

<br/>

**My solution**

```
function distinct(a) {
    return Array.from(new Set(a));
};
```
