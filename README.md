## How to add JavaScript to a webpage

### Add JavaScript code inside a Script tag

You can use the `<script>` tag to execute JavaScript from inside the markup of an HTML document.

### Add an external JavaScript file using a Script tag

You can use the `<script>` tag to execute JavaScript from an external file outside of the markup of an HTML document.

You do this by putting the name of the script in the `src` (source) attribute.

This approach is generally preferred because it separates your HTML markup from your JavaScript making your code clean and easy to read.

## Where to add JavaScript to a webpage

### Add a Script tag to the Head

You can add the `<script>` tag to the `<head>` of your HTML document to keep it separated from the content of your webpage, but this location should be avoided because of:

1. Render blocking
2. DOM manipulation errors

#### Render blocking

Render blocking is when the browser has to wait for a script to load before it can render the HTML and CSS required to display a webpage to a user.

#### DOM manipulation errors

DOM (Document Object Model) manipulation errors are caused when a script that contains code that alters HTML loads before the HTML.

### Add a Script tag to the Body

You can add the `<script>` tag to the `<body>` of your HTML document.

However, it is best practice to add scripts right before `</body>` to avoid render blocking and DOM manipulation errors.
