# Practical Exercise: Working with HTML Forms and Elements

## Objective:
Create a user registration form that includes various HTML form elements to collect user information. The form should validate the input using both HTML attributes and basic JavaScript validation.

## Instructions:

### Create the Basic Structure:
1. Create a new HTML file and name it `registration_form.html`.
2. Set up the basic HTML structure with a `<!DOCTYPE html>` declaration, a `<html>` tag, a `<head>` tag, and a `<body>` tag.
3. When all tasks done push your work on github then share me the link.

### Form Creation:
- Inside the `<body>` tag, create a `<form>` element with the following attributes:
  - `action="#"` (for now, we'll not submit it to a server).
  - `method="POST"`.
  - `id="registrationForm"`.

### Form Elements:

#### Text Input:
- Add a `label` and `input` element for the user’s full name.
- Set the `type` attribute of the input to `"text"`.
- Add a `placeholder` attribute with the text "Enter your full name".
- Add a `required` attribute to ensure the field is filled out before submitting.

#### Email Input:
- Add a `label` and `input` element for the user’s email address.
- Set the `type` attribute of the input to `"email"`.
- Add a `placeholder` attribute with the text "Enter your email".
- Add a `required` attribute.

#### Password Input:
- Add a `label` and `input` element for the user’s password.
- Set the `type` attribute of the input to `"password"`.
- Add a `placeholder` attribute with the text "Create a password".
- Add a `required` attribute.

#### Radio Buttons:
- Add a `label` element with the text "Gender".
- Add three `input` elements with the `type="radio"` for Male, Female, and Other.
- Ensure each radio button has the same `name` attribute (`name="gender"`).

#### Checkboxes:
- Add a `label` element with the text "Hobbies".
- Add three `input` elements with the `type="checkbox"` for hobbies such as Reading, Traveling, and Gaming.

#### Dropdown (Select):
- Add a `label` and `select` element to allow the user to choose their country.
- Add a few `option` elements for different countries.

#### Text Area:
- Add a `label` and `textarea` element for additional comments or a bio.
- Set a `placeholder` with the text "Tell us more about yourself".
- Add attributes `rows="4"` and `cols="50"`.

#### Submit Button:
- Add an `input` element with `type="submit"` and `value="Register"` to create a submit button.

### HTML Form Validation:
- Ensure that all required fields are validated by HTML. For instance, the email field should use the correct email format.

### Adding Basic JavaScript Validation:
- Below the form, add a `<script>` tag.
- Write a JavaScript function that checks if the password is at least 8 characters long before allowing the form to be submitted. If not, display an alert and prevent form submission.

```html
<script>
  document.getElementById("registrationForm").onsubmit = function(event) {
    var password = document.querySelector("input[name='password']").value;
    if (password.length < 8) {
      alert("Password must be at least 8 characters long.");
      event.preventDefault();
    }
  };
</script>
