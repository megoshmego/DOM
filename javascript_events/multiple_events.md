The main concepts discussed in the transcript are:

1. **DOM Manipulation**: This is the process of modifying the Document Object Model (DOM), which is a programming interface for HTML documents. It represents the structure of a webpage and can be manipulated to change the content, structure, and style of the webpage. The `document.querySelector` and `document.querySelectorAll` methods are used to select elements from the DOM.

2. **Event Handling**: This is the process of setting up certain code to be run in response to a specified event, like a user clicking a button. In JavaScript, this can be done using the `addEventListener` method. 

3. **Loops**: The instructor uses a `for...of` loop to iterate over all the buttons and add an event listener to each.

4. **Event Object**: This is the object that gets passed to an event handler when an event occurs. It contains information about the event, such as the element that triggered the event (`event.target`).

5. **Creating and Appending Elements**: The instructor shows how to create new HTML elements (`document.createElement`), set their content (`element.innerText`), and append them to existing elements (`element.appendChild`).

6. **Form Handling**: The transcript explains how to handle form submissions in JavaScript, including how to prevent the default form submission behavior (`event.preventDefault()`), and how to access the value of an input field (`input.value`).

Here is a basic code snippet that demonstrates these concepts:

```javascript
// selecting elements from the DOM
const buttons = document.querySelectorAll('li button');

// using a loop to add an event listener to each button
for (let btn of buttons) {
  btn.addEventListener('click', function(e) {
    // getting the parent element of the clicked button and removing it
    e.target.parentElement.remove();
  });
}

// selecting the form and input from the DOM
const form = document.querySelector('#add-friend');
const input = document.querySelector('#first-name');

// handling form submission
form.addEventListener('submit', function(e) {
  // preventing default form submission behavior
  e.preventDefault();

  // creating a new li and button
  const newFriend = document.createElement('li');
  const removeButton = document.createElement('button');

  // setting the content of the new elements
  newFriend.innerText = input.value;
  removeButton.innerText = 'Unfriend';

  // appending the button to the li
  newFriend.appendChild(removeButton);

  // appending the new li to the ul
  document.querySelector('#friend-list').appendChild(newFriend);

  // clearing the input field
  input.value = '';
});
```

This code will add a remove functionality to all the buttons in a list, as well as allow users to add new items to the list using a form. The newly added items will also have a remove button.