## Regexp Basics - is it a vowel?
Implement the function which should return `true` if given object is a vowel (meaning `a, e, i, o, u`), and `false` otherwise.

<br/>

**My solution**

```
String.prototype.vowel = function() {
  return this.match(/^[aeiouAEIOU]$/) ? true : false;
};
```