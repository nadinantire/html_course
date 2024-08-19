# Detailed Introduction to CSS

CSS, or Cascading Style Sheets, is the language used to style an HTML document. It describes how HTML elements should be displayed on the screen, paper, or in other media. CSS saves a lot of work because it can control the layout of multiple web pages all at once.

The "cascading" part of CSS refers to the way that styles can be applied in layers. If there are multiple styles for a single element, the styles will cascade and apply in order of precedence.

## CSS Syntax

A CSS rule consists of a selector and a declaration block.

- **Selector**: The HTML element you want to style.
- **Declaration Block**: Contains one or more declarations separated by semicolons.

Each declaration includes a CSS property name and a value, separated by a colon. A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces `{}`.

**Example:**

```css
h1 {
    color: blue;
    font-size: 24px;
    text-align: center;
}
```
- `h1` is the selector.
- `color`, `font-size`, and `text-align` are properties.
- `blue`, `24px`, and `center` are the corresponding values.

## Ways to Add CSS with Examples

### Inline CSS

Best used for applying a unique style to a single element. Inline CSS can be cumbersome to manage for larger projects but is useful for quick testing or for applying styles dynamically through JavaScript.

```html
<p style="color: green; font-weight: bold;">This is an inline-styled paragraph.</p>
```

## Internal CSS

Useful for applying styles to a single HTML document. Internal CSS is handy when you need to style a page with a unique design. However, it’s not ideal for maintaining consistency across multiple pages.

```html
<html>
<head>
    <style>
        body {
            background-color: lightgray;
        }
        h2 {
            color: darkblue;
            font-family: Arial, sans-serif;
        }
        p {
            color: black;
            line-height: 1.6;
        }
    </style>
</head>
<body>
    <h2>Internal CSS Example</h2>
    <p>This paragraph is styled using internal CSS.</p>
</body>
</html>
```
## External CSS

External CSS is ideal for styling multiple pages from a single file. It keeps your HTML files cleaner and makes updating styles across a website easier. External CSS files are linked to HTML documents using the `<link>` tag.

**HTML:**

```html
<html>
<head>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <h1>External CSS Example</h1>
    <p>This paragraph is styled using external CSS.</p>
</body>
</html>
```
## CSS (`styles.css`):

```css
body {
    background-color: #f0f0f0;
    font-family: 'Helvetica Neue', sans-serif;
}

h1 {
    color: #333;
    text-transform: uppercase;
}

p {
    color: #555;
    font-size: 18px;
}
```
## Advanced CSS Concepts

### Selectors

- **Class Selector (`.`):** Targets elements with a specific class attribute.

    ```css
    .highlight {
        background-color: yellow;
    }
    ```

    ```html
    <p class="highlight">This text is highlighted.</p>
    ```

- **ID Selector (`#`):** Targets a unique element with a specific ID attribute.

    ```css
    #main-header {
        background-color: black;
        color: white;
        padding: 10px;
    }
    ```

    ```html
    <h1 id="main-header">Welcome to My Website</h1>
    ```

- **Universal Selector (`*`):** Applies styles to all elements on the page.

    ```css
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    ```

### Combining Selectors

- **Grouping:** Apply the same styles to multiple selectors.

    ```css
    h1, h2, h3 {
        color: navy;
        font-weight: bold;
    }
    ```

- **Descendant Selector:** Targets elements nested inside other elements.

    ```css
    div p {
        color: red;
    }
    ```

## Conclusion

CSS is a powerful tool for controlling the visual presentation of web content. By separating content (HTML) from design (CSS), you can create cleaner, more maintainable code, and provide a consistent experience across your website.
