# Introduction to JavaScript and DOM Manipulation

## Objectives

Write basic JavaScript functions.
Manipulate the DOM dynamically.
Respond to user interactions.

## Instructions

- Create a script.js file and link it to a HTML.
- Structure the document using DOCTYPE, html, head, and body.

>[!NOTE]
>  - Write JavaScript that:
>  - Changes text content dynamically.
>  - Modifies CSS styles via JavaScript.
>  - Adds or removes an element when a button is clicked.


# Tasks
- Create a well-structured HTML5 document.
- Use at least 5 different HTML elements.
- Ensure semantic correctness.

Happy Coding! 💻✨
<!DOCTYPE html>
<html>
<head>
    <title>Basic JavaScript Example</title>
    <script src="script.js"></script>
</head>
<body>
    <h1 id="title">Welcome to my website!</h1>
    <p id="content">This is some example content.</p>
    <button id="add-button">Add Button</button>

    <script>
        // Change text content dynamically
        function updateTitle() {
            document.getElementById('title').textContent = 'Hello, World!';
        }

        // Modify CSS styles via JavaScript
        function changeBackground() {
            document.body.style.backgroundColor = 'lightblue';
        }

        // Add or remove an element when a button is clicked
        function addRemoveButton() {
            var button = document.getElementById('add-button');
            if (button) {
                var newButton = document.createElement('button');
                newButton.textContent = 'New Button';
                document.body.appendChild(newButton);
            } else {
                document.getElementById('content').remove();
            }
        }

        // Respond to user interactions
        document.getElementById('add-button').addEventListener('click', addRemoveButton);
    </script>
</body>
</html>
script.js:
// Change text content dynamically
function updateTitle() {
    document.getElementById('title').textContent = 'Hello, World!';
}

// Modify CSS styles via JavaScript
function changeBackground() {
    document.body.style.backgroundColor = 'lightblue';
}

// Add or remove an element when a button is clicked
function addRemoveButton() {
    var button = document.getElementById('add-button');
    if (button) {
        var newButton = document.createElement('button');
        newButton.textContent = 'New Button';
        document.body.appendChild(newButton);
    } else {
        document.getElementById('content').remove();
    }
}

// Respond to user interactions
document.getElementById('add-button').addEventListener('click', addRemoveButton);
Explain it

