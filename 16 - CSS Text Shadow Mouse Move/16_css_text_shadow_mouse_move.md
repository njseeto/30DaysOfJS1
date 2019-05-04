### HTML Elements

- [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement) for info on offsetHeight, offsetTop etc
- `offsetX` and `offsetY` can be used to get the position of the cursor
- However, if there are nested elements, the position co-ordinates will restart when entering a new element.

<br>

Since (x , y) co-ordinates will restart when in a new element, in this case in the `h1` element rather than the parent `div`, the below bit of code addas the co-ordinates of the child element onto the co-ordinates of the parent element. Rather than having the co-ordinates go to (0,0) when at the top left corner of the `h1` element.

```
   if(this != e.target){
      x = x + e.target.offsetLeft
      y = y + e.target.offsetTop
    }
```


<br>

`walk` - in the tutorial this is referring to the amount of stretch in the shadow. So the top left hand corner should be one end of the scale and the bottom right the other end. Eg: 50 to -50; the walk in this case would be 100. This is done through the code below.

```
  const xWalk = ( x / width * 100 ) - walk / 2
  const yWalk = ( y / width * 100 ) - walk / 2
```