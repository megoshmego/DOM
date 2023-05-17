The key concepts here are:

1. **HTML Elements & CSS Classes**: HTML elements (like H1) can be given classes, which determine their appearance via CSS. In the demo, two classes, `big` and `small`, are used.

    HTML:
    ```html
    <h1 class="big">Happy</h1>
    ```

    CSS:
    ```css
    .big {
        transform: scale(2);
        color: green;
    }

    .small {
        transform: scale(0.5);
        color: red;
    }
    ```

2. **JavaScript DOM manipulation**: JavaScript can be used to select HTML elements and modify their properties. Here, the `document.querySelector` function is used to select the `h1` element. The `classList` property of the selected element is then used to add, remove or toggle CSS classes.

    JavaScript:
    ```javascript
    const h1 = document.querySelector('h1');
    h1.classList.toggle('big');
    h1.classList.toggle('small');
    ```

3. **JavaScript setInterval function**: This function is used to repeatedly execute a specified function at fixed time intervals. Here, it's used to toggle the classes `big` and `small` every second.

    JavaScript:
    ```javascript
    setInterval(() => {
        h1.classList.toggle('big');
        h1.classList.toggle('small');
    }, 1000);
    ```

4. **JavaScript conditionals and string manipulation**: Conditional statements (if-else) are used to change the text of the `h1` element based on its current class. The `innerText` property of the `h1` element is used to manipulate the text.

    JavaScript:
    ```javascript
    if (h1.classList.contains('big')) {
        h1.innerText = 'Sad';
    } else {
        h1.innerText = 'Happy';
    }
    ```

5. **CSS Transitions**: CSS transitions provide a way to control animation speed when changing CSS properties. Here, a transition is applied to the `h1` element so that changes in its properties (caused by class toggling) take place smoothly over a duration of one second.

    CSS:
    ```css
    h1 {
        transition: all 1s;
    }
    ```