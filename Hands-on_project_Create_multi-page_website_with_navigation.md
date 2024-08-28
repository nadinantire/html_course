
# Exercise: Building an Online Registration System

## Objective:
Create a basic online registration system using multiple HTML pages styled with CSS. The system should include:

- A homepage introducing the registration system.
- A registration page with a form for user input.
- A confirmation page to display the user's input details.

## Step-by-Step Instructions:

### 1. Create a Homepage (index.html):

- This page should introduce the registration system.
- Include a brief description of the registration process.
- Add a navigation bar with links to the "Home" and "Registration" pages.
- Include a button or link to the "Registration" page.

### 2. Create a Registration Page (register.html):

- Design a form that asks for basic user information, such as:
  - First Name
  - Last Name
  - Email Address
  - Password
  - Gender (Radio Buttons)
  - Country (Dropdown)
- Include a "Submit" button.
- The form should be styled with CSS to be user-friendly and visually appealing.

### 3. Create a Confirmation Page (confirmation.html):

- This page should display a message like "Thank you for registering!"
- Include a summary of the user's information that was submitted.
- Provide a link to return to the homepage.

### 4. Add Styling with CSS (styles.css):

- Use external CSS to style all the pages consistently.
- Add a simple color scheme, fonts, padding, and margins to enhance the visual appeal.
- Style the form elements (input fields, buttons) to make them look neat and modern.
- Create a responsive layout that adjusts to different screen sizes.

## Tips:
- Use the `<nav>` element to create the navigation bar.
- Ensure the links between pages are working correctly using the `<a>` tag.
- Use semantic HTML elements (`<header>`, `<footer>`, `<section>`, etc.) to structure the pages.
- Apply CSS flexbox or grid for the layout to make it responsive.
- Test the form validation with required attributes (`required`) for the input fields.

## Example Folder Structure:

```
/registration-system
  ├── index.html
  ├── register.html
  ├── confirmation.html
  └── styles.css
```

## Additional Challenge:
- Add JavaScript to validate the form inputs before submission.
- Enhance the confirmation page with a summary table of the submitted data.
