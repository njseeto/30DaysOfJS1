## **JAVASCRIPT METHODS**
```
filter()
map()
sort()
reduce()
```

`filter()`
- A predicate that tests each element in an array. If it returns true it is kept
- This method returns an array

SYNTAX
```
const newArray = arr.filter(callback(element[, index[, array]])[, thisArg])
```

EXAMPLE
```
const arr = [ 1, 2, 3, 4, 5, 6]
const isEven = arr.filter(x => x % 2 == 0)

```

`map()`
- Creates a new array with the results of calling a provided function on every element in the calling array.
- This method returns a new array with each element being the result of the callback function.

SYNTAX
```
const new_array = arr.map(function callback(currentValue[, index[, array]]) {
    // Return element for new_array
}[, thisArg])
```

EXAMPLE
```
const array1 = [1, 4, 9, 16]
const map1 = array1.map(x => x * 2)
```

`queryselectorAll`
- produces a NodeList, this means you cannot do any of the above methods on the results unless you convert it into an array.
```
    const links = [...category.querySelectorAll('a')]
    const de = links.map(link => link.title)
```


`sort()`
- Uses a comparator function/callback to sort numbers, compares 'a' and 'b' which returns a 1, -1 or 0.

SYNTAX
```
const newArray = array.sort(callback(a, b))
```

EXAMPLE
```
const sort = inventors.sort((a, b) => a.year > b.year ? 1 : -1)
```

`reduce()`
- Executes a function on each element of the array
- Results in a single value
- [Medium article on reduce()](https://medium.freecodecamp.org/reduce-f47a7da511a9)

SYNTAX
```
arr.reduce(callback[, initialValue])
```

EXAMPLE
```
    const transport = data.reduce((obj, item) => {
      if (!obj[item]) {
        obj[item] = 0
      } obj[item]++
      return obj
    },
      {}
    )
```


#### OTHER LEARNINGS:
`deepEqual` is the same as ===

EXAMPLE:
```
a = '12345'
b = 12345

a == b
true

a === b
false

+a === b
true

```


#### Converting an Object into an Array
[Medium article](https://medium.com/chrisburgin/javascript-converting-an-object-to-an-array-94b030a1604c)
- Essentially you can use `Object.value()` or `Object.keys()`
- `Object.value()` is supported in newer JavaScript and can be used if you are using babel
- Otherwise use `Object.keys()`

#### `Object.keys(obj)`

[MDN breakdown](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)

- This returns an array of the objects keys.


#### Converting an Array of Objects to an Object
- [Medium article](https://medium.com/dailyjs/rewriting-javascript-converting-an-array-of-objects-to-an-object-ec579cafbfc7)
- Use `reduce()`