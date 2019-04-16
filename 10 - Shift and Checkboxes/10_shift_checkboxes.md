### Using a flag variable and a variable that keeps state

To complete this exercise, we need a way to track which items have been checked and whether there are any items in between any two checked items.


`let lastChecked`

This keeps track of the last checked item.

`let inBetween = false`

This flag variable lets us know where to start checking the boxes and when to stop.


Flip the flag variable to true when we check the first item, then back to false when we hit the last item.
```
          if(checkbox === this || checkbox === lastChecked){
            inBetween = !inBetween
            }
```


Check those boxes whose inBetween flag is true.
```
if(inBetween){
    checkbox.checked = true
}
```


NOTES
`let` can be used when the value of the variable will be changing. A `let` variable is constrained to whichever scope it is declared in.