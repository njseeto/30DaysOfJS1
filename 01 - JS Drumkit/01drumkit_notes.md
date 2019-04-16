## **Event Listeners**
- `addEventListener()` attaches an event handler to a specified element
- You can add event listeners to any DOM object not only HTML elements. i.e the window object.
- You cannot listen to an array, Node list. This will require a `forEach()`
- Syntax: `element.addEventListener(event, function, useCapture)`

Example
```
element.addEventListender('click', myFunction)
    function myFunction(){
        DoSomething
    }
```

__Bubbling vs Capturing__
- The difference between these terms is how they deal with events at different layers of the HTML.
- Bubbling: deals with the event at the innermost layer first
- Capturing: deals with the event at the outer most layer first.
- the `useCapture` argument is set to _false_ by default, which will use _bubbling_

__Listening for Transition End Events__
- This is used in the project to remove the CSS class of `playing` once the transition has ended.
Code snippet:
```
    function removeTransition(e) {
      if (e.propertyName != 'transform')
        return
      this.classList.remove('playing')
    }
    
    const key = document.querySelectorAll('.key')
    key.forEach(key => key.addEventListener('transitionend', removeTransition))
```