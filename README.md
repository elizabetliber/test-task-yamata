### 1.

1 решение:

```
function splitTheString(str){
let string = str.length % 2 === 0 ? str : str + '_'
let arr = [];

for (var i = 0; i < string.length; i+=2) {
    arr.push(string.slice(i, i + 2));
}

return arr
}
console.log(splitTheString('55346'))

```

2 решение:

```
function splitTheString(str) {
  let string = str.length % 2 === 0 ? str : str + '_';
  return string.match(/.{1,2}/g);
}
console.log(splitTheString('55346'));

```

### 2.

```
function arrFunction (n, x) {
  let array = []
  for(let i = n; i <= new Array(x).length; i+=n){
    array.push(i);
  };

  return array
}
console.log(arrFunction(3, 10))

```

### 3.

```
function century(year) {
    let century = year % 100 === 0 ? year/100 : Math.floor(year/100) + 1;
    return century; 
}
console.log(century(1600))

или

const century = (year) => Math.floor((year - 1)/100) + 1

console.log(century(1600))

```
