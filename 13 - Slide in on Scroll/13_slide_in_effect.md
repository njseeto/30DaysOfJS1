### Debounce

- Limits the number of times a function will run. This is to limit the number of times the `checkSlide` function is called. 
- Prevents your UI code from needing to process every event and also drastically reduces the number of API calls sent to your server.
- Processing every character as it’s entered could harm performance and add unnecessary load to your server.
- Debouncing is mainly used to improve your application's performance.

Debounce is a higher order function that returns another function.

More notes on [debounce](https://levelup.gitconnected.com/debounce-in-javascript-improve-your-applications-performance-5b01855e086)


[Closures](https://medium.freecodecamp.org/lets-learn-javascript-closures-66feb44f6a44)