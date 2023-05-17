Here are some condensed code snippets based on the information you provided:

1. Using Local Storage:

```javascript
// Store data in local storage
localStorage.setItem('key', 'value');

// Retrieve data from local storage
let data = localStorage.getItem('key');

// Remove data from local storage
localStorage.removeItem('key');

// Clear all data in local storage
localStorage.clear();
```

2. Using Session Storage:

```javascript
// Store data in session storage
sessionStorage.setItem('key', 'value');

// Retrieve data from session storage
let data = sessionStorage.getItem('key');

// Remove data from session storage
sessionStorage.removeItem('key');

// Clear all data in session storage
sessionStorage.clear();
```

3. Converting objects to strings and vice versa:

```javascript
let obj = {name: "John", age: 30, city: "New York"};

// Convert object to string
let myJSON = JSON.stringify(obj);

// Convert string to object
let myObj = JSON.parse(myJSON);
```

4. Event handling in JavaScript:

```javascript
let button = document.querySelector('button');

// Handle 'click' event
button.addEventListener('click', function() {
  alert('Button Clicked!');
});
```

5. DOM Manipulation:

```javascript
// Change text content of an element
document.querySelector('h1').textContent = 'Hello, World!';

// Add a class to an element
document.querySelector('body').classList.add('dark');

// Remove a class from an element
document.querySelector('body').classList.remove('dark');
```

6. Implementing a dark mode toggle feature:

```javascript
// Store dark mode preference
localStorage.setItem('darkMode', 'enabled');

// Check if dark mode is enabled
let darkMode = localStorage.getItem('darkMode');

// Add or remove dark mode based on preference
if (darkMode === 'enabled') {
  document.querySelector('body').classList.add('dark');
} else {
  document.querySelector('body').classList.remove('dark');
}

// Add event listener to toggle dark mode
document.querySelector('.dark-mode-toggle').addEventListener('click', function() {
  if (document.querySelector('body').classList.contains('dark')) {
    document.querySelector('body').classList.remove('dark');
    localStorage.setItem('darkMode', 'disabled');
  } else {
    document.querySelector('body').classList.add('dark');
    localStorage.setItem('darkMode', 'enabled');
  }
});
```

I hope these snippets will be helpful in understanding these web development concepts!