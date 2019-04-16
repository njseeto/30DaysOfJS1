FETCH
- [MDN: Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- Returns a **promise** which you need to call `.then()` to retrieve the blob of data.
- Takes in a mandatory argument (the path to the resource you want to get)


SPREAD OPERATOR
- [MDN: Spread Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)
- [Nice overview of spread operator](https://codeburst.io/javascript-es6-the-spread-syntax-f5c35525f754)
- Allows an iterable to expand in places where 0+ arguments are expected.

EXAMPLE
```
// copying arrarys //

const arr1 = [ 1, 2, 3 ]
const arr2 = arr1  // this assigns arr2 to the same reference of arr1, meaning anything we do to arr2 affects arr1

arr2.push(4)

console.log(arr1)
//output [ 1, 2, 3, 4]


const arr1 = [ 1, 2, 3 ]
const arr2 = ...arr1  // this sets arr2 to equal the value of arr1 rather than referencing arr
```

REGEX
- `RegExp()` this creates a regex object used to match text with the pattern.
SYNTAX
```
new RegExp(pattern[, flags])
```


COOL THINGS:
- Can return html properties
- 