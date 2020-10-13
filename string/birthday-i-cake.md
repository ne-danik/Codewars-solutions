## Birthday I - Cake
It's your Birthday. Your colleagues buy you a cake. The numbers of candles on the cake is provided (x). Please note this is not reality, and your age can be anywhere up to 1,000. Yes, you would look a mess.
<br/>

As a surprise, your colleagues have arranged for your friend to hide inside the cake and burst out. They pretend this is for your benefit, but likely it is just because they want to see you fall over covered in cake. Sounds fun!
<br/>

When your friend jumps out of the cake, he/she will knock some of the candles to the floor. If the number of candles that fall is higher than 70% of total candles (x), the carpet will catch fire.
<br/>

You will work out the number of candles that will fall from the provided string (y). You must add up the character ASCII code of each even indexed (assume a 0 based indexing) character in y, with the alphabetical position of each odd indexed character in y to give the string a total.
<br/>

**Example**: 'abc' --> a=97, b=2, c=99 --> y total = 198.
<br/>

If the carpet catches fire, return 'Fire!', if not, return 'That was close!'.

<br/>

**My solution**

```
function cake(x, y) {
 
  const sortLetter = y.split("");
  let arr = [];
  sortLetter.forEach((element, index) => {
    const numberASC = element.charCodeAt(0);
    if (index % 2 === 0) {
      arr.push(numberASC);

    } else {
      arr.push(numberASC - 96);

    }
  });
  const sum = arr.reduce((acc, value) => acc + value,0);

  if ((sum / x) * 100 >= 70) {
    return "Fire!";
  }
  return "That was close!";
}

cake(56, 'ifkhchlhfd');
```
