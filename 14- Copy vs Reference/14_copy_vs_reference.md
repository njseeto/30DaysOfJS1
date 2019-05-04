### COPY vs REFERENCE (for arrays and objects)
4 ways to ensure you do not mutate the original ARRAY:
- `slice()` takes a copy of the array, meaning the original object is not mutated.
- `[].concat(array)` this creates a new array and concats the old one
- `[...players]`
- `Array.from(array)`

Ways to ensure you do not mutate the original OBJECT:
- `Object.assign({}, object, key : value)` 
- `{...object, key : value }`

The 2 above solutions only clone an object one level deep.

- `JSON.parse(JSON.stringify(object))` This is a hacky solution to do a deepClone. `JSON.stringify()` takes the object, converts it to a string and `JSON.parse()` converts it back into an object.