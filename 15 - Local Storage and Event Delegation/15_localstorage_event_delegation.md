### Local Storage

Local storage is a list of items which are saved to your browser. This can be seen in the _Application_ tab of your devTools.
You can only use strings in your local storage - so we need to `JSON.stringify()` your arrays / objects to be able to store them as stirngs in local storage.

This line allows the localStorage to persist on refresh if there are items present on page load..
`const items = JSON.parse(localStorage.getItem('items')) || [];`

This adds the item to localStorage:
`localStorage.setItem('items', JSON.stringify(items))`


`preventDefault` stops the page from refreshing.


### Event Delegation
Listen to events on a higher level (parent element) and inside of this parent element we check it is for the events we want inside it.