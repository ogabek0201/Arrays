# <center>JavaScript lesson#4</center>

<p align="center">

<img src="https://img.shields.io/badge/Made%20by-Ogabek-yellow" >

<img src="https://img.shields.io/badge/Methods-Arrays-brown">

<img src="https://img.shields.io/badge/methods-CallBack-brown">

<img src="https://img.shields.io/badge/Learn-Javascript-black">

</p>

---

 _<center>An array is an object that can store multiple values at once. You can access elements of an array using indices (0, 1, 2 …). Array's index starts with 0, not 1. an array can hold values of mixed types.</center>_

```js
let array=[1,2,3,4,5,6,7,8,9,10]
   //index 0 1 2 3 4 5 6 7 8 9
```

---

# _<center>Array methods</center>_

### PUSH() && UNSHIFT()

```
You can use the built in method push and unshift to add elements to an array
```

#### __push()__

```js
let array=[1,2]
array.push(3)
console.log(array);//[1,2,3]
```

#### __unshift()__

```js
let array=[2,3]
array.unshift(1)
console.log(array);//[1,2,3]
```

### POP() && SHIFT()

```
pop() method to remove the last element from an array and also returns the returned value.
The shift() method removes the first element and also returns the removed element.
```

#### __pop()__

```js
let array=[1,2,3]
array.pop()
console.log(array);//[1,2]
```

#### __shift()__

```js
let array=[1,2,3]
array.shift()
console.log(array);//[2,3]
```

### REVERSE() && CONCAT()

```
The reverse() method returns the array in reverse order.
The concat() method returns a new array by merging two or more values/arrays.
```

#### __reverse()__

```js
let array=[1,2,3]
array.reverse()
console.log(array);//[3,2,1]
```

#### __concat()__

```js
let array=[1,2,3]
let array2=[4,5]
let result=array.concat(array2)
console.log(result);//[1,2,3,4,5]
```

### INDEXOF() && INCLUDES()

```
The indexOf() method returns the first index of occurance of an array element, or -1 if it is not found.
The includes() method checks if an array contains a specified element or not.
```

#### __indexOf()__

```js
let array=[1,2,3]
console.log(array.indexOf(2));//1
```

#### __concat()__

```js
let array=[1,2,3]
console.log(array.includes(2));//true
```

### SPLICE()

```
The splice() method returns an array by changing (adding/removing) its elements in place.
```

## __splice() Parameters__

* _The `splice()` method takes in:_
  * `start` - The index from where the array is changed.
  * `deleteCount` (optional) - The number of items to remove from start.
  * `item1, ..., itemN` (optional) - The elements to add to the `start` index.  If not specified, `splice()` will only remove elements from the array.

#### __splice()__

```js
let array=["JavaScript", "Python", "Java", "Lua", "C++"]
array.splice(-1, 1, "Swift", "Scala", "Go")
console.log(array);//[ 'JavaScript', 'Python', 'Java', 'Lua', 'Swift', 'Scala', 'Go' ]
```

---

# _<center>Array methods callbacks</center>_

### map()

```
The map() method creates a new array with the results of calling a function for every array element.
```

* _Featured:_
  * __`map()` does not change the original array.__
  * __`map()` executes callback once for each array element in order.__
  * __`map()` does not execute callback for array elements without values.__
  * __`map()` assigns undefined to the new array if the callback function returns undefined or nothing.__

```js
let array=["JavaScript", "Python", "Java", "Lua", "C++"]
let result = array.map(a=>a.concat(" language"))
console.log(result);
```

```js
let array=[1,4,9,16,25]
let result=array.map(Math.sqrt)
console.log(result);//[1,2,3,4,5]
```

---
