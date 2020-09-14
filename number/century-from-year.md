## Century From Year
The first century spans from the year 1 up to and including the year 100, The second - from the year 101 up to and including the year 200, etc.
<br/>

Given a year, return the century it is in.

<br/>

**Example**

```
centuryFromYear(1705)  returns (18)
centuryFromYear(1900)  returns (19)
centuryFromYear(1601)  returns (17)
centuryFromYear(2000)  returns (20)
```
<br/>

**My solution**

```
function century(year) {
   return year % 100 === 0 ? parseInt(year / 100) : parseInt(year / 100) + 1; 
};
```
