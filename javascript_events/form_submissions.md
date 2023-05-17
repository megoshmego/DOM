The important terms and concepts discussed in the transcript are:

1. **HTML forms**: A web page component that collects user input. It can include various types of input elements, like text fields, checkboxes, radio buttons, submit buttons, etc. 

```html
<form>
  <input type="text" placeholder="Input something">
  <button type="submit">Submit</button>
</form>
```

2. **Form submission**: The process of sending form data to a server. By default, submitting a form triggers a page refresh as the browser makes a new request to the server.

3. **JavaScript Event Listener**: A function in JavaScript that waits for a specific event to occur (like a button click, form submission, etc.) and then runs some code.

```javascript
const button = document.querySelector("button");
button.addEventListener("click", () => {
  console.log("Button clicked!");
});
```

4. **JavaScript Form Submission Event**: A specific event that is triggered when a form is submitted. This can be listened to using the `addEventListener` method and the `"submit"` event.

```javascript
const form = document.querySelector("form");
form.addEventListener("submit", (event) => {
  console.log("Form submitted!");
});
```

5. **Event.preventDefault()**: A JavaScript method that stops the default action of an event from happening. For a form, the default action is to send the data and refresh the page. Using `preventDefault` in a form's submit event listener will stop the page from refreshing.

```javascript
form.addEventListener("submit", (event) => {
  event.preventDefault();
  console.log("Form submitted, but page did not refresh!");
});
```

6. **Single-page applications (SPAs)**: Web apps that load a single HTML page and dynamically update that page as the user interacts with the app. SPAs use JavaScript to handle user interactions and avoid page refreshes.

7. **Form action attribute**: This attribute specifies where to send form data when a form is submitted. For example, `<form action="https://example.com">` will send the form data to `https://example.com`.

8. **JavaScript access to form data**: In the form submission event listener, you can access the form data entered by the user.

```javascript
form.addEventListener("submit", (event) => {
  event.preventDefault();
  let input = form.querySelector("input").value;
  console.log("Form submitted with input: ", input);
});
```

In the transcript, the speaker walks through creating an HTML form and attaching a JavaScript event listener to intercept the form submission event. They demonstrate how to prevent the form from causing a page refresh using `event.preventDefault()` and highlight how this approach is used in single-page applications to handle form submissions without navigating away from the current page.