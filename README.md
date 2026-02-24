1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Ans:
Here are differences between getElementById, getElementsByClassName, and querySelector / querySelectorAll :
getElementById() :
a. it selects an element using an ID only.
b. it returns only one element.
c. it returns a single DOM element.

getElementsByClassName() :
a. it selects elements using a class name.
b. it can return multiple elements.
c. it returns an HTMLCollection (live collection).

querySelector() / querySelectorAll() :
a . it use CSS selectors (id, class, etc.)
b . querySelector() returns the first matching element and
querySelectorAll() returns all matching elements.
c . it returns a NodeList (static collection).


2. How do you create and insert a new element into the DOM?
Ans :
First,  need to create a new element with document.createElement().
Then  need to add text or content to it and append() it.

3. What is Event Bubbling? And how does it work?
Ans :
Event Bubbling is a process where when an event occurs on a child element, that event goes upwards from child to parent to parent.
If a button is inside a div. When you click on the button, the button event will be triggered first and then the div event will be triggered. Here the button is the child and the div is the parent.

4. What is Event Delegation in JavaScript? Why is it useful?
Ans :
Event Delegation is the process of handling events of child elements by setting an event listener on the parent element. This is possible due to Event Bubbling. 
Its advantages are:
a. You don't have to set a separate event listener on each child.
b. Even if a new element is added, you don't have to give a separate event.
c. The code becomes cleaner.

5. What is the difference between preventDefault() and stopPropagation() methods?

Ans :
preventDefault() :
a. It only affects the default behavior of that specific element.
b. It stops the browser's default behavior.
c. Using this will not cause the page to reload.

stopPropagation() :
a. Stops the event from reaching the parent or upper element.
b. Stops the bubbling of the event.
c. If you use this on a child button, the click event of the parent div will not work.
