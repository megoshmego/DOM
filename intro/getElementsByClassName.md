The transcript discusses the following main ideas:

1. **Selecting elements using class name**: This is done in JavaScript by using the `document.getElementsByClassName()` method. It returns an HTMLCollection of all elements in the document with the specified class name.

    Code snippet:

    ```javascript
    let elements = document.getElementsByClassName('myClass');
    ```

2. **Multiple classes**: An HTML element can have multiple classes, which are specified by separating them with spaces.

    Code snippet:

    ```html
    <div class="class1 class2 class3">This is a div with multiple classes</div>
    ```

3. **Selecting elements with multiple classes**: To select elements with multiple classes using `getElementsByClassName()`, you need to separate class names by spaces inside the string.

    Code snippet:

    ```javascript
    let elements = document.getElementsByClassName('class1 class2');
    ```
   
4. **HTMLCollection**: `getElementsByClassName()` returns an HTMLCollection, which is an array-like object of all child elements. Even if there's only one match or no matches, it still returns an HTMLCollection (in these cases, the HTMLCollection would contain one element or be empty, respectively).

5. **Other methods of selecting elements**: The transcript mentions `getElementById()` and `getElementsByTagName()`, which select elements by ID and tag name, respectively. It also mentions `querySelector()`, a newer method that is more versatile than the others.

Here are corresponding code snippets for these methods:

   `getElementById()`:

    ```javascript
    let element = document.getElementById('myId');
    ```

   `getElementsByTagName()`:

    ```javascript
    let elements = document.getElementsByTagName('myTag');
    ```

   `querySelector()`:

    ```javascript
    let element = document.querySelector('.myClass');  // Selects the first element with class "myClass"
    let elements = document.querySelectorAll('.myClass');  // Selects all elements with class "myClass"
    ```

These are the primary concepts discussed in the transcript.