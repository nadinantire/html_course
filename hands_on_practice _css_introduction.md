# CSS Exercises

## Exercise 1: Class Selector

### Objective:
Apply a class-based style to elements.

### Instructions:
1. Create an HTML file.
2. Add a `<style>` block in the `<head>` section.
3. Define a class `.highlight` that sets the background color to yellow.
4. Add a paragraph `<p>` with the class `highlight` and some text.
5. Save and open the HTML file in a browser to see the styling in action.

**Example:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Class Selector Exercise</title>
    <style>
        .highlight {
            background-color: yellow;
        }
    </style>
</head>
<body>
    <p class="highlight">This text is highlighted.</p>
</body>
</html>
```
# CSS Exercises

## Exercise 2: ID Selector

### Objective:
Style a unique element using an ID.

### Instructions:
1. Create an HTML file.
2. Add a `<style>` block in the `<head>` section.
3. Define an ID `#main-header` that sets the background color to black, text color to white, and padding to 10px.
4. Add an `<h1>` with the ID `main-header` and some text.
5. Save and open the HTML file in a browser to see the styling in action.

### Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ID Selector Exercise</title>
    <style>
        #main-header {
            background-color: black;
            color: white;
            padding: 10px;
        }
    </style>
</head>
<body>
    <h1 id="main-header">Welcome to My Website</h1>
</body>
</html>
```
## Exercise 3: Universal Selector

### Objective:
Apply a universal style to all elements.

### Instructions:
1. Create an HTML file.
2. Add a `<style>` block in the `<head>` section.
3. Define the universal selector `*` to set margin and padding to 0, and box-sizing to border-box.
4. Add various HTML elements (`<h1>`, `<p>`, `<div>`) to the body with different content.
5. Save and open the HTML file in a browser to see the effects of the universal styling.

### Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Universal Selector Exercise</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
    </style>
</head>
<body>
    <h1>Heading</h1>
    <p>This is a paragraph.</p>
    <div>Content in a div.</div>
</body>
</html>
```

## Exercise 4: Combining Selectors

### Objective:
Apply the same styles to multiple selectors.

### Instructions:
1. Create an HTML file.
2. Add a `<style>` block in the `<head>` section.
3. Define styles for `h1`, `h2`, and `h3` to set color to navy and font-weight to bold.
4. Add elements `<h1>`, `<h2>`, and `<h3>` with different content to the body.
5. Save and open the HTML file in a browser to see the combined styling.

### Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Combining Selectors Exercise</title>
    <style>
        h1, h2, h3 {
            color: navy;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Main Heading</h1>
    <h2>Subheading</h2>
    <h3>Smaller Heading</h3>
</body>
</html>
```
## Exercise 5: Descendant Selector

### Objective:
Style elements nested inside other elements.

### Instructions:
1. Create an HTML file.
2. Add a `<style>` block in the `<head>` section.
3. Define a descendant selector `div p` to set the text color to red.
4. Add a `<div>` with a nested `<p>` element in the body.
5. Save and open the HTML file in a browser to see the descendant styling.

### Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Descendant Selector Exercise</title>
    <style>
        div p {
            color: red;
        }
    </style>
</head>
<body>
    <div>
        <p>This text inside the div is red.</p>
    </div>
</body>
</html>
```

These exercises are designed to help you practice and understand the application of various CSS selectors and styling techniques.
