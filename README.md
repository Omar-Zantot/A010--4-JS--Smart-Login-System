# Smart Login System

The Smart Login System is a web application that allows users to register and log in securely. It utilizes HTML, CSS, and JavaScript to handle user registration, login, and welcome features. The system stores user data in the browser's local storage, making it a client-side application with no backend integration.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Function Descriptions](#function-descriptions)
- [License](#license)

## Features

1. **User Registration:** Allows users to create an account by providing their name, email, and password.
2. **Unique Email Check:** Ensures that no two users can register with the same email address.
3. **User Login:** Allows registered users to log in by providing their email and password.
4. **Welcome Message:** Displays a personalized welcome message to the user after successful login.

## Installation

1. Clone the repository or download the ZIP file.
2. Open the `index.html` file in your web browser.

## Usage

1. **Sign Up:**
   - Enter your name, email, and password in the registration form fields.
   - Click the "Sign Up" button to create an account.
   - If the email is already registered, an error message will be displayed.

2. **Sign In:**
   - Enter your registered email and password in the login form fields.
   - Click the "Sign In" button to log in.
   - If the provided credentials are incorrect or the fields are empty, an error message will be displayed.

3. **Welcome Message:**
   - After successful login, you will be redirected to the "home.html" page.
   - The page will display a personalized welcome message with your name.

## Function Descriptions

1. `addUser()`: Handles user registration by validating the input fields, checking if the email is already registered, and adding the user to the local storage.

2. `isRegFormEmpty()`: Checks if the registration form fields are not empty.

3. `isEmailAlreadyTaken()`: Checks if the provided email during registration is already registered by searching the local storage for matching email addresses.

4. `displayMessage(elementId, message, isError)`: Displays messages in the specified target element. It can be used for both success and error messages.

5. `searchUser()`: Handles the login process by checking if the login form fields are not empty, and verifies login credentials using the `login()` function.

6. `isLoginFormEmpty()`: Checks if the login form fields are not empty.

7. `login()`: Searches the local storage for matching email and password during login and returns true if a user is found.

8. `welcome()`: Displays a personalized welcome message on the home page after successful login.

## License

This project is licensed under the [MIT License](LICENSE).
