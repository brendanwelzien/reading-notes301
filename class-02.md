# JS and JQuery (293 - 301, 306-331, 354-357)
- jQuery offers tasks for JS
    - it is simpler to access elements using jQuery selectors rather than to use DOM queries
    - lets you update the DOM tree, animate elements in and out of view, and can loop through a set of elements in one line of code
    - handles events through methods 
1. find elements using css style selectors
    a. $() often used as a shorthand... $('li.hot')
    b. selects `li` elements with a class of `hot`
2. Do something with the elements using Jquery methods
    a. $('li.hot').addClass('complete');
- in order to use Jquery, you first must include in the script
- benefits of cross-browser comptability

Single Element
- if a selector returns just one element `$('ul')`, the JQuery object contains a reference to one node

Multiple Elements
- if a selector returns several elements, the JQuery object contains references to each element `$('li')`... if there were 4 list elements, you would have to select li instead of ul.

*Getting Information*
- using the *.html()* method gets info from an element, use *.each()* to retrieve content of all elements
- if you are setting information it will apply it to all elements unless distinctly targeting index#
    - JQuery also only stores references, not copies

*Creating a JQuery Object*
1. find matching nodes in DOM tree
2. create the JQuery object
3. store references to the nodes in JQuery object
    - `$groceryItems = $('li');`

*Looping*
- the ability to update all elements in the JQuery selection is known as **implicit iteration**

*Chaining*
- if you want to use more than one method, use dot notation to separate each one
- `$('p[id!="two"]').hide().delay(500).fadeIn(1400);`
- if one method does not work, the rest will not run

- to check if a page is ready to work with the code use...
```js
$(document).ready(function()){
//script goes here
});
```
- the shorthand for this is...
```js
$(function() {
    //script goes here
});
```
*Getting Element Content*
- .html() (only retrieves first element)
- .text() (retrieves text of element)
- .append() (lets you add content to page)

*Updating Elements*
- .replaceWith() / .remove()

*Inserting Elements*
1. create new elements in a JQuery object
    a. var $newPiece = $('li');
2. Use a method to insert the content into the page
    a. use a method...
- .before() (puts before selected element)
- .prepend() (puts content inside element after opening tag)
- .after() (inserts after element)
- .append() ( inserts content inside element before closing tag)

*Getting and Setting Attribute Values*
- .attr() can get or set an attribute and value
- .addClass() adds a new value to existing class att
- .removeAttr() removes attr and value
- .removeClass() removes just value

- the .css() method lets you set properties to JQuery objects

## Pair Programming
- pair programming is the practice of two developers sharing a workstation to tackle coding tasks together.
- involves two roles: Driver and Navigator
    - driver is typing and only one whose hands are on the keyboard (mechanics)
        - includes text editor, switching files, version control, and writing code
    - navigator thinks about big picture, algorithmic thinking, scans for typos
- fundamental skills to learning the language are...
1. Listening
2. Speaking
3. Reading
4. Writing

*The advantages*
- pair programming takes longer, but identifies a higher rate of mistakes
- reaches solutions faster
- working together allows for students to learn different approaches and may be inspired to absorb such approaches
- social skills improve... You are working with someone else and communicating constantly together
- for job interviews, each person can practice prep exercises, whiteboard interviews, etc.
- after this, these people are more prepared for the work environment, paired programming is a commonly seen setting professionally, so practicing this through Code Fellows will help indefinitely.

[<=Back](README.md)