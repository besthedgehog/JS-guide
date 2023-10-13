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

### find
~~~
[4, 5, 1, 8, 2, 0].find(x => x > 3); // 4
~~~
```
[4, 5, 1, 8, 2, 0].findIndex(x => x > 3); // 0
```

## Methods of strings

~~~
"SoloLearn".includes("loLe"); // true
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

## Methods of classes

### Getter
(call a method like a property)
~~~
class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
  get area() {
    return this.calcArea();
  }
  calcArea() {
    return this.height * this.width;
  }
}
const square = new Rectangle(5, 5);
console.log(square.area); // 25
~~~

### Static method
(cannot be called through a class _instance_)

~~~
class Point {
  constructor(x, y) {
    this.x = x;
    this.y = y;
  }
  static distance(a, b) {
    const dx = a.x - b.x;
    const dy = a.y - b.y;
    return Math.hypot(dx, dy);
  }
}
const p1 = new Point(7, 2);
const p2 = new Point(3, 8);

console.log(Point.distance(p1, p2));
~~~