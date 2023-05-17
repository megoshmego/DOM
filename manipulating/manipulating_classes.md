The instructor in the transcript is teaching the concept of manipulating classes in JavaScript. Here are the key terms and concepts discussed:

**1. CSS Classes:**
CSS classes are styles that can be applied to multiple elements on a web page. They are usually defined in CSS files and can be applied to HTML elements to control their appearance.

**2. Manipulating Classes:**
JavaScript can be used to add, remove, or toggle CSS classes in HTML elements. This can be used to dynamically change the appearance of elements on a web page.

**3. Methods for manipulating classes:**
   - `getAttribute`: This method is used to get the value of a specified attribute on the element.
   - `setAttribute`: This method adds a new attribute or changes the value of an existing attribute on an HTML element.
   - `className`: This property gets and sets the value of the class attribute of the specified element.
   - `classList`: This read-only property returns a live `DOMTokenList` collection of the class attributes of the element. It provides methods like `add`, `remove`, `toggle`, and `contains`.

**4. Demonstration (Code Snippets):**

Adding, removing, and toggling classes using `classList`:

```javascript
// Selecting an element
let el = document.querySelector('li');

// Adding a class
el.classList.add('new-class');

// Removing a class
el.classList.remove('new-class');

// Toggling a class
el.classList.toggle('new-class');

// Checking if an element contains a certain class
let containsClass = el.classList.contains('new-class'); // returns true or false
```

Selecting all `li` elements and toggling the `completed` class on all of them:

```javascript
function toggleAllTodos() {
    const todos = document.querySelectorAll('li');
    for (let li of todos) {
        li.classList.toggle('completed');
    }
}

toggleAllTodos(); // Toggles the 'completed' class on all 'li' elements
```

This example assumes there's already a CSS class called `completed` defined somewhere in your styles.