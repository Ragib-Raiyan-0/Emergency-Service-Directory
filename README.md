1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
   answer: The difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll are given below,
        (1) getElementById = It returns one element with the given ID.
        (2) getElementsByClassName = It returns all elements with the given class as an HTML_collection.
        (3) querySelector = It returns the first element that matches a CSS selector.
        (4) querySelectorAll = It Returns all elements that match a CSS selector as a NodeList.  
2. How do you create and insert a new element into the DOM?
  answer: Steps to create and insert a new element into the DOM:
          (1) Create the element – Use document.createElement() to make a new element.
           (2) Add content or attributes – Set the text or any attributes for the new element.
           (3)  Select the parent element – Choose the element in the DOM where you want to insert the new element.
           (4)  Insert the element into the DOM – Use appendChild() or insertBefore() to add it to the selected parent.

3. What is Event Bubbling and how does it work?
  answer: Event Bubbling and how it works:

     (1) Definition :Event bubbling is when an event triggered on a child element propagates (moves up) to its parent elements
     (2) How it works : The event starts at the innermost element where it occurred and then bubbles up through all ancestor elements until it reaches the document root.
      (3) Example : If you click a button inside a div, the click event first triggers on the button, then on the div, and then on the body, and so on.
     (4) Usage : Useful for handling events on parent elements instead of adding listeners to multiple children.

4. What is Event Delegation in JavaScript? Why is it useful?
  answer: Event Delegation and its usefulness:

      (1) Definition – Event delegation is a technique where you attach a single event listener to a parent element instead of adding listeners to multiple child elements.
      (2) How it works – The parent catches events from its children using event bubbling, and you can determine which child triggered the event.
    (3) Why it’s useful –
     i. Reduces the number of event listeners, saving memory and improving performance.
     ii. Works for dynamic elements added to the DOM later.

5. What is the difference between preventDefault() and stopPropagation() methods?
  answer: Difference between preventDefault() and stopPropagation():
    (1) preventDefault() – Stops the default browser behavior of an element.
        Example: Preventing a link from navigating or a form from submitting.

    (2) stopPropagation() – Stops the event from bubbling up (or capturing down) the DOM tree.
        Example: Preventing a click on a button from triggering a click handler on its parent.
insort we can say, preventDefault() → stops default action, stopPropagation() → stops event flow.
