## DEVTOOLS

**'Break on -> attribute modifications'**

This is like a breakpoint for the front end. It pauses on the line of code that causes a particular attribute.

<br>

`console.group()`

EXAMPLE
```
    dogs.forEach( dog => {
      console.groupCollapsed(`${dog.name}`)
      console.log(`This is ${dog.name}`),
      console.log(`${dog.name} is ${dog.age} years old`)
      console.groupEnd(`${dog.name}`)
    })
```
The example above allows you to group by dog name. This command can let you see a whole lot of information without having to `console.log()` a whole lot of times.

<br>

`console.time()`

EXAMPLE
```
    console.time('fetching data')
    fetch('https://api.github.com/users/njseeto')
    .then(data => data.json())
    .then(data => {
      console.timeEnd('fetching data')
      console.log(data)
    })
```

This allows you to see how long a fetch request takes and hence can see whta's holding up our requests. 