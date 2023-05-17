Sure, I'd be happy to provide some code snippets to demonstrate these concepts.

1. **HTML Element Selection**:

    ```javascript
    let h1 = document.querySelector('h1');  
    let paragraphs = document.getElementsByTagName('p');  
    ```

2. **DOM Properties - `innerText` and `textContent`**:

    ```javascript
    // using innerText
    let h1 = document.querySelector('h1');
    h1.innerText = 'New Text';  

    // using textContent
    let p = document.querySelector('p');
    p.textContent = 'New Text';
    ```

3. **DOM Manipulation**:

    ```javascript
    let h1 = document.querySelector('h1');
    h1.innerText = 'New Text';  
    ```

4. **CSS Selection**:

    ```html
    <h4 style="display: none;">This text is hidden</h4>
    ```

5. **querySelectorAll**:

    ```javascript
    let paragraphs = document.querySelectorAll('p');
    ```

6. **getElementById, getElementsByClassName**:

    ```javascript
    let elementById = document.getElementById('myId');
    let elementsByClass = document.getElementsByClassName('myClass');
    ```

7. **innerHTML and style property**:

    ```javascript
    let div = document.querySelector('div');
    div.innerHTML = '<h2>New Heading</h2>';
    div.style.backgroundColor = 'lightblue';
    ```

8. **setAttribute and createElement, appendChild**:

    ```javascript
    let newDiv = document.createElement('div');
    newDiv.setAttribute('id', 'newId');
    document.body.appendChild(newDiv);
    ```

9. **CSS Classes, className, classList**:

    ```javascript
    let h1 = document.querySelector('h1');
    h1.className = 'newClass';
    h1.classList.add('anotherClass');
    h1.classList.remove('anotherClass');
    ```

10. **Nodes and DOM traversal**:

    ```javascript
    let parent = document.querySelector('div').parentElement;
    let children = document.querySelector('div').children;
    let firstChild = document.querySelector('div').firstElementChild;
    ```

11. **console.dir**:

    ```javascript
    console.dir(document.querySelector('h1'));
    ```

12. **Event Listeners**:

    ```javascript
    document.querySelector('button').addEventListener('click', function() {
        console.log('Button clicked!');
    });
    ```

13. **Styling using JavaScript**:

    ```javascript
    let h1 = document.querySelector('h1');
    h1.style.color = 'red';
    ```

14. **Inline Styles**:

    ```javascript
    let h1 = document.querySelector('h1');
    h1.style = 'color: red; background-color: black';
    ```

15. **Camel Case for CSS Properties in JavaScript**:

    ```javascript
    let h1 = document.querySelector('h1');
    h1.style.backgroundColor = 'blue';
    ```
