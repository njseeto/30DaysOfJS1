### CANVAS
- [More info on the Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- Uses the HTML `<canvas>` element
- `getContext()` this method gets the element's context - the thing which the drawing will be rendered on.
- There is a suite of methods from the Canvas API,

```
lineTo()
moveTo()
stroke()
 ```

- There are also a number of properties 

```
strokeStyle()
lineWidth()
```

### DESTRUCTURING
[MDN breakdown](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)
- Makes it possible to unpack values from arrays or properties from objects into distinct variables.

EXAMPLE
```
[a, b] = [10, 20];

console.log(a);
// expected output: 10

console.log(b);
// expected output: 20


[a, b, ...rest] = [10, 20, 30, 40, 50];

console.log(rest);
// expected output: [30,40,50]
```

