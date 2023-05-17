In this transcript, there are several key terms and concepts to be aware of:

1. **DOM (Document Object Model)**: This is a programming interface for web documents. It represents the structure of a document (like HTML) and allows a programming language (like JavaScript) to manipulate the structure, style, and content.

2. **DOM Selectors**: These are methods in JavaScript that allow you to select specific elements from the DOM. They include `getElementById`, `getElementsByClassName`, and `getElementsByTagName`.

3. **Query Selector**: This is a versatile method that can select elements based on a CSS selector. It can combine the functionality of the above methods.

4. **Query Selector All**: Similar to query selector, but it returns all elements that match the CSS selector.

5. **CSS Selectors**: These are patterns used to select elements to style in CSS. They can be used with the query selector methods in JavaScript.

6. **ID Selector**: In CSS, this uses a hash (#) symbol followed by the ID of an element. 

7. **Class Selector**: In CSS, this uses a dot (.) symbol followed by the class of an element.

8. **Element Selector**: In CSS, this just uses the name of the HTML tag.

9. **Attribute Selector**: In CSS, this selects an element based on its attribute.

10. **Node List**: This is a collection of nodes, or elements, returned by methods like `querySelectorAll`.

Here are some simple demonstrations of the concepts mentioned:

```javascript
// Get element by id
var element = document.getElementById("myId");

// Get elements by class name
var elements = document.getElementsByClassName("myClass");

// Get elements by tag name
var elements = document.getElementsByTagName("p");

// Query selector
var element = document.querySelector("#myId"); // Selects the element with id "myId"

// Query selector all
var elements = document.querySelectorAll(".myClass"); // Selects all elements with class "myClass"

// Attribute selector
var inputElement = document.querySelector('input[type="text"]'); // Selects the first input element of type "text"
```

Note that `querySelector` returns the first matching element, while `querySelectorAll` returns all matching elements. The elements are returned as a NodeList, which is a collection of nodes, or elements.