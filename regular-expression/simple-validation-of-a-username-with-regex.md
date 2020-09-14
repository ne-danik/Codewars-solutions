## Simple validation of a username with regex
Write a simple regex to validate a username. Allowed characters are:
<br/>

* lowercase letters,
* numbers,
* underscore

Length should be between 4 and 16 characters (both included).

<br/>

**My solution**

```
function validateUsr(username) {
  res =  RegExp('^[a-z0-9_]{4,16}$').test(username);
  return res;
};
```
