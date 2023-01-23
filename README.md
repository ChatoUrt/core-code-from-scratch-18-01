# core-code-from-scratch-18-01

## --- Who likes it ---

* [Test]()

Solution / /

``` javascript 
function likes(names) {
  if (names.length == 0) return "no one likes this";
  if (names.length == 1) return `${names[0]} likes this`;
  if (names.length == 2) return `${names[0]} and ${names[1]} like this`;
  if (names.length == 3) return `${names[0]}, ${names[1]} and ${names[2]} like this`;
  return `${names[0]}, ${names[1]} and ${names.length -2} others like this`;
}
```

---
## ---Bit counter---

* [Test](https://www.codewars.com/kata/526571aae218b8ee490006f4/train/javascript)

Solution / /

``` javascript
var countBits = function(n) {
  let txt;
  let binary;
  let arr;
  if (n > 0) {
    txt = n.toString(2);
    binary = txt.replace(/[0]/gi, '');
    arr = binary.split('');
  return arr.length
  } else return n;
}
```

---
## ---Let's order---

* [Test](https://www.codewars.com/kata/55c45be3b2079eccff00010f/train/javascript)

Solution / /

``` javascript
function order(words) {
  let orderW = words.split(' ').sort((a,b) => {
    let a1 = Number(a.replace(/[A-Za-z]/g, ''));
    let b1 = Number(b.replace(/[A-Za-z]/g, ''));
    return a1 - b1;
  });
  return orderW
}
```
