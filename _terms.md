Condensed Information for Flashcards:

1. **DOM (Document Object Model):** A programming API for HTML and XML documents representing the structure of the documents and allowing manipulation of the content and visual presentation.

2. **Style Property:** A JavaScript property used to get, set, and modify the CSS of an HTML element.

3. **QuerySelector:** A JavaScript method for selecting the first HTML element that matches a specific CSS selector.

4. **Inline Styles:** CSS styles applied directly to HTML elements using the 'style' attribute.

5. **Specificity:** A set of rules in CSS that determine which style declarations are applied to an element when there is a conflict between styles.

6. **Camel Case:** A coding convention in JavaScript where multi-word variable or function names begin with a lowercase letter, and each new word starts with a capital letter.

7. **Accessing HTML Elements:** The process of selecting HTML elements in the DOM using methods such as `querySelector`.

8. **Getting and Setting the Style Property:** The process of reading and modifying CSS properties of an HTML element using the `style` property in JavaScript.

9. **Distinction between Inline Styles and External Styles:** Inline styles are declared in the HTML document itself, whereas external styles are defined in separate CSS files. The `style` property in JavaScript only accesses inline styles.

10. **JavaScript vs CSS Property Names:** JavaScript uses camelCase for CSS properties (backgroundColor), while CSS uses kebab-case (background-color).

11. **Setting Multiple CSS Properties with JavaScript:** It involves assigning new styles to multiple CSS properties of an HTML element using JavaScript.

12. **Modifying CSS Properties for Multiple Elements:** The process of changing the CSS properties of several HTML elements at once using JavaScript.

13. **HTML Elements & CSS Classes:** HTML elements can have one or more classes, which can be styled in CSS.

14. **JavaScript DOM Manipulation:** The process of dynamically changing the content, structure, or style of HTML elements using JavaScript.

15. **JavaScript setInterval Function:** A built-in JavaScript function that executes a specific function or code snippet repeatedly at fixed time intervals.

16. **JavaScript Conditionals and String Manipulation:** The use of conditional statements in JavaScript to control the flow of code execution and manipulate strings.

Certainly! Here's a refresher on common JavaScript event listeners:

1. **click**: Fires when an element is clicked.

```javascript
element.addEventListener('click', function() {
  // Event handling code here
});
```

2. **mouseover**: Fires when the mouse pointer enters an element.

```javascript
element.addEventListener('mouseover', function() {
  // Event handling code here
});
```

3. **mouseout**: Fires when the mouse pointer leaves an element.

```javascript
element.addEventListener('mouseout', function() {
  // Event handling code here
});
```

4. **keydown**: Fires when a key on the keyboard is pressed.

```javascript
element.addEventListener('keydown', function(event) {
  // Event handling code here
});
```

5. **keyup**: Fires when a key on the keyboard is released.

```javascript
element.addEventListener('keyup', function(event) {
  // Event handling code here
});
```

6. **submit**: Fires when a form is submitted.

```javascript
element.addEventListener('submit', function(event) {
  // Event handling code here
});
```

7. **change**: Fires when the value of an input element changes (e.g., on checkbox selection, dropdown selection).

```javascript
element.addEventListener('change', function(event) {
  // Event handling code here
});
```

8. **load**: Fires when an element, such as an image or the entire page, finishes loading.

```javascript
window.addEventListener('load', function() {
  // Event handling code here
});
```

These are just a few examples of common event listeners in JavaScript. Event listeners allow you to respond to user interactions and other events in your web applications. Remember to replace "element" in the code snippets with the appropriate DOM element to attach the event listener to.