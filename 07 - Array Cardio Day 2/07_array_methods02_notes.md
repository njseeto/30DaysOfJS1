ARRAY METHODS

`some()`
- [MDN breakdown](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/some)
- returns a boolean
- accepts a function
- tests whether at least one element in the array passes the test implemented by the function provided

<br>

`every()`
- Exactly the same as `some()` except it tests _every_ element in the array.

<br>

`find()`
- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find)
- Accepts a function
- Returns the _value_ of the first element in the array that satisfies the testing funciton.
- If nothing is found, it returns `undefined`

<br>

`findIndex()`
- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex)
- Takes a function
- Returns the element of the array that satisfies the funciton
- If the function is not satisfied, -1 is returned

<br>

`slice()`
- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice)
- Returns a shallow copy of an array into a _new array object_
- The original array will not be modified
- `arr.slice([begin[, end]])`

<br>

`splice()`
- WARNING: Mutates the original array
- Probably should be avoided!!
- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)