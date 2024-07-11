**# Only-one-dropdown-opens-at-a-time**

The provided script toggles an "open" class on elements with a data-click="faq" attribute when they are clicked.
If an element does not have the "open" class when clicked, 
the script first removes the "open" class from any other elements that have it, 
then adds the "open" class to the clicked element.
If the clicked element already has the "open" class,
the script removes the class from it.

**Here's a breakdown of how the script works:**
Event Listener: Listens for a click event on any element with the data-click="faq" attribute.
Condition Check: Checks if the clicked element does not have the "open" class.
Close Other Open Items: If the clicked element does not have the "open" class, it finds all other elements with the data-click="faq" attribute that have the "open" class and simulates a click on them to close them.
Toggle Class: Adds the "open" class to the clicked element if it wasn't open. Removes the "open" class if it was already open.
This is useful for creating FAQ sections where only one question can be open at a time, and clicking on an open question closes it.
