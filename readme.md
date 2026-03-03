# 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

### getElementById() is used to select one element by its id. Since id is always unique, it returns only one element.getElementsByClassName() is used to select elements by their class name. It can return multiple elements because many elements can have the same class. It returns an HTMLCollection.querySelector() is used to select the first element that matches a CSS selector. We can use id, class, or even tag name inside it.querySelectorAll() is similar to querySelector(), but it returns all matching elements. It returns a NodeList.

# 2.How do you create and insert a new element into the DOM?
### create a new element, we use document.createElement().we insert it into the DOM using methods like appendChild() or append().
document.body.appendChild(p);

# 3 What is Event Bubbling? And how does it work?

### Event bubbling is a process where an event starts from the target element and then moves upward to its parent elements.

For example, if we click a button inside a div, the click event first happens on the button. Then it moves to the div, and then to the body, and so on.

So the event “bubbles up” from the child element to the parent elements. This is called event bubbling.

# 4. What is Event Delegation in JavaScript? Why is it useful?

Event delegation is a technique where we add an event listener to a parent element instead of adding it to many child elements.

Because of event bubbling, the parent can detect events that happen on its children.

This is useful because:

It improves performance.

We don’t need to add many event listeners.

It also works for dynamically added elements.

# 5. What is the difference between preventDefault() and stopPropagation() methods?

preventDefault() is used to stop the default action of an element.

For example, if we click a link, it normally goes to another page. But if we use preventDefault(), the link will not open.

stopPropagation() is used to stop the event from moving to parent elements.

So, preventDefault() stops the default behavior, and stopPropagation() stops event bubbling.

