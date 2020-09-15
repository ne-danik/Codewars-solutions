## Regexp Basics - is it a letter?
Complete the code which should return `true` if the given object is a single ASCII letter (lower or upper case), `false` otherwise.

<br/>

**My solution**

```
String.prototype.isLetter = function() {
  return this.match(/^[a-zA-Z]/) && this.length === 1 ? true : false;
}
```