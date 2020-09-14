## Palindrome Strings
A palindrome is a word, phrase, number, or other sequence of characters which reads the same backward or forward. This includes capital letters, punctuation, and word dividers.<br/>

Implement a function that checks if something is a palindrome.

<br/>

**Examples**

```
isPalindrome("anna")   ==> true
isPalindrome("walter") ==> false
isPalindrome(12321)    ==> true
isPalindrome(123456)   ==> false
```
<br/>

**My solution**

```
function isPalindrome(line) {
  String(line);
  const lengthText = line.length - 1;
  let reverse = '';

  for (let i = lengthText; i >= 0; i--) {
    reverse = `${reverse}${line[i]}`;
  }
  
  return (line === reverse) ? true : false;
};
```
