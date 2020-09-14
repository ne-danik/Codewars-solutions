## Anagram Detection
An **anagram** is the result of rearranging the letters of a word to produce a new word (see [wikipedia](https://en.wikipedia.org/wiki/Anagram)).
<br/>

*Note:* anagrams are case insensitive
<br/>

Complete the function to return `true` if the two arguments given are anagrams of each other; return `false` otherwise.

<br/>

**Examples**
<br/>

`"foefet"` is an anagram of `"toffee"`

`"Buckethead"` is an anagram of `"DeathCubeK"`

<br/>

**My solution**
```
function isAnagram (test, original) {
  return test.toLowerCase().split("").sort().join("") === original.toLowerCase().split("").sort().join("");
};
```
