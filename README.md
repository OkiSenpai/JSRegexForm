# JSRegexForm
# Contact Form Validation with JavaScript

This project demonstrates a simple contact form with client-side validation using JavaScript. The form includes fields for a user's name, first name, email, phone number, and message. Each field is validated using regular expressions (regex) to ensure the input meets specific criteria before submission.

## Features

- **Real-time Validation**: Each input field is validated when the user clicks the submit button.
- **Error Messages**: Displays error messages in red for invalid or empty fields.
- **Regex Validation**: Ensures that inputs match specific patterns for names, email, phone numbers, and messages.
- **User Feedback**: Alerts the user when the form is successfully submitted.

## Form Fields

The form includes the following fields:

1. **Name (Nom)**:
   - Regex: `^[A-Za-zÀ-ÿ\s'-]{2,50}$`
   - Validates that the name contains 2-50 characters, including letters, spaces, hyphens, and apostrophes.

2. **First Name (Prénom)**:
   - Regex: `^[A-Za-zÀ-ÿ\s'-]{2,50}$`
   - Similar validation as the name field.

3. **Email**:
   - Regex: `^[\w.-]+@[\w.-]+\.\w{2,}$`
   - Validates a standard email format.

4. **Phone Number (Téléphone)**:
   - Regex: `^(?:\+32|0)[1-9]\d{7,8}$`
   - Validates Belgian phone numbers, allowing either a `+32` country code or a leading `0`.

5. **Message**:
   - Regex: `^.{5,1000}$`
   - Ensures the message is between 5 and 1000 characters.

## How It Works

1. **HTML Structure**:
   - The form is built using standard HTML elements, with `id` attributes assigned to each input field and corresponding error message spans.

2. **JavaScript Validation**:
   - A `verificationDeInput` function is defined to handle validation.
   - Event listener on the submit button (`btn`) prevents default form submission and validates each field.
   - If a field is empty or does not match its regex, an error message is displayed in red.
   - If all fields are valid, an alert is shown indicating successful submission.

3. **Error Handling**:
   - Each field has a dedicated `<span>` element to display error messages.
   - Error messages are styled in red for better visibility.

## File Structure
