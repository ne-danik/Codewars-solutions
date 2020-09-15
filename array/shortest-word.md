## Shortest Word
Simple, given a string of words, return the length of the shortest word(s).
<br/>

String will never be empty and you do not need to account for different data types.

<br/>

**My solution**

```
function findShort(s) {
  return s.split(' ').sort((a, b) => a.length - b.length).shift().length;
};
```
