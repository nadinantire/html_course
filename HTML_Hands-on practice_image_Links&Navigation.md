# Exercise: Build a Simple Webpage

## Objective:
Create a basic webpage that includes the following elements :

- A favicon.
- A heading and a paragraph.
- A list (both ordered and unordered).
- A table with some data.
- Links (text and image links).
- Use of `div` and `class` to structure the content.
- Inline styles to add color.

## Instructions:

### 1. Create the HTML file
Create a new file named `index.html`.

### 2. Add a Favicon
Place an image named `download.jpg` in the same directory as your HTML file. This will be used as the favicon.

### 3. Write the HTML Code

Here’s a template you can use, but make sure to understand it as you go along:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Practical HTML Exercise</title>
    <!-- Favicon -->
    <link rel="icon" href="download.jpg" type="image/jpeg">
</head>
<body>

    <!-- Header Section -->
    <div class="header" style="background-color: #f0f0f0; padding: 10px;">
        <h1 style="color: #333;">Welcome to My Webpage</h1>
        <p>This is a simple webpage created as part of an HTML exercise.</p>
    </div>

    <!-- Navigation Section -->
    <div class="nav" style="background-color: #e0e0e0; padding: 10px;">
        <h2>Navigation</h2>
        <ul>
            <li><a href="#section1">Section 1</a></li>
            <li><a href="#section2">Section 2</a></li>
            <li><a href="#section3">Section 3</a></li>
        </ul>
    </div>

    <!-- Content Section -->
    <div class="content" style="padding: 10px;">
        <!-- Section 1 -->
        <div id="section1">
            <h3>Section 1: List and Links</h3>
            <p>Below is an unordered list:</p>
            <ul>
                <li>Item 1</li>
                <li>Item 2</li>
                <li>Item 3</li>
            </ul>

            <p>And an ordered list:</p>
            <ol>
                <li>First</li>
                <li>Second</li>
                <li>Third</li>
            </ol>

            <p>Visit <a href="https://www.example.com" style="color: blue;">Example Website</a> for more information.</p>
            <p>Or click on this image link:</p>
            <a href="https://www.example.com">
                <img src="download.jpg" alt="Example Image" style="width: 150px;">
            </a>
        </div>

        <!-- Section 2 -->
        <div id="section2">
            <h3>Section 2: Table</h3>
            <p>Here is a table displaying some data:</p>
            <table border="1" cellpadding="5" cellspacing="0" style="width: 100%; border-collapse: collapse;">
                <tr style="background-color: #f0f0f0;">
                    <th>Name</th>
                    <th>Age</th>
                    <th>City</th>
                </tr>
                <tr>
                    <td>John Doe</td>
                    <td>30</td>
                    <td>New York</td>
                </tr>
                <tr>
                    <td>Jane Smith</td>
                    <td>25</td>
                    <td>London</td>
                </tr>
                <tr>
                    <td>Samuel Green</td>
                    <td>40</td>
                    <td>Toronto</td>
                </tr>
            </table>
        </div>

        <!-- Section 3 -->
        <div id="section3">
            <h3>Section 3: Footer</h3>
            <p>This is the end of the content. Thank you for visiting!</p>
        </div>
    </div>

</body>
</html>
```
# Key Points

### Favicon
The `<link rel="icon">` tag is used to specify a favicon for the webpage. The favicon should be named `download.jpg` and placed in the same directory as your HTML file.

### Div and Classes
The content is structured using `div` elements, each with a specific class (`header`, `nav`, `content`). This helps in organizing different sections of the webpage.

### Lists
Both unordered (`<ul>`) and ordered (`<ol>`) lists are used to display items.

### Links
The `<a>` tag is used for creating hyperlinks, including a text link and an image link.

### Table
The `<table>` element is used to display tabular data. The table includes rows (`<tr>`) and cells (`<td>` and `<th>`).

### Inline Styles
Basic inline styles are applied directly to the elements, such as setting background colors and text colors.

## Result
When you load this HTML code in your browser, it will display a simple, structured webpage with different sections, lists, a table, and links, all without using external CSS. This exercise will help you understand how to structure a webpage and use basic HTML elements effectively.
