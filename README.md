# JS-guide
Guide for most common javascript commands

## Methods of arrays

~~~
let arr = []; // creating new array

let arr = new Array(); // creating new array


arr.push(valuse); // adds a value to arr

arr.reverse(); // reverses 

arr.slice(start, end) // returnes elements from array 

arr.join(sep) // creates a string from array

... arr // [a, b, c] => a, b, c

arr.map(func); // apply functuion to all the elemens of array

array1 = arr.filter(func) // returns an array for which the function returned true

arr.findIndex(func) // returns the index of the element for which f returns true

arr.find(func) // returns value of the element for which f returns true
~~~

## Loops

### Loops for

~~~
for (let i = 1; i <= 10; i++) {
    console.log(i)
    }
~~~

```
for (let i = a.length - 1; i >= 0; i--) { 
    console.log(a[i]);
    }
```

### For of
~~~
let arr = [1,2,3];
for (let i of arr) {
    console.log(i);
}
~~~

### For in
~~~
let obj = { name: 'Harry Smith', age: 42 };
for (const key in obj) {
    console.log(`${key}: ${obj[key]}`);
    }
~~~