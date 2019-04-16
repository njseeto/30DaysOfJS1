## **CSS**
__VARIABLES__
- Great to make a change across a different number of elements, eg: if a company's brand colour changes you only ned to change it in one place

__JS and CSS__
- You can use JS to dynamically change CSS properties
- `querySelectorAll` returns a [NodeList](https://developer.mozilla.org/nl/docs/Web/API/NodeList)
- `setProperty` allows you to change CSS variables
- Data attributes can be accessed through `dataset`
- The below allows us to listen for 'change', however, this doesn't change until you let go of the cursor
- So we also need to also listen for 'mousemove'
```
inputs.forEach(input => {
  input.addEventListener('change', handleUpdate);
  input.addEventListener('mousemove', handleUpdate);
}
```
