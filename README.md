# Flutter Login App

This is a simple Flutter application demonstrating the basics of Flutter development, UI building, form validation, and navigation between screens. It is designed as a learning project for beginners to understand how to build responsive user interfaces and handle basic authentication flows in Flutter.

## Features

- **Login Screen**: A user-friendly login form with email and password fields.
- **Form Validation**: Validates email format and ensures the password is not empty and at least 6 characters long.
- **Navigation**: Navigates from the login screen to a home screen upon successful login using `Navigator.push()`.
- **Forgot Password**: A placeholder for forgot password functionality.
- **Responsive UI**: Uses Flutter widgets like `Column`, `Row`, and `Container` for layout.
- **Demo Credentials**: Shows example credentials for testing.

## App Structure

- `main.dart`: Contains the entire app logic, including the login and home screens.
  - **MyApp**: The root widget that sets up the app theme and initial route.
  - **LoginScreen**: A stateful widget with a form for email and password, validation logic, and navigation to the home screen.
  - **HomeScreen**: A simple screen shown after successful login, with a logout button to return to the login screen.

## How It Works

1. **Login Form**: The login screen presents two `TextFormField` widgets for email and password. The form uses a `GlobalKey<FormState>` to manage validation.
2. **Validation**: 
   - The email field checks for a valid email format using a regular expression.
   - The password field checks that it is not empty and is at least 6 characters long.
3. **Login Action**: When the user taps the login button, the form is validated. If valid, the app navigates to the home screen using `Navigator.push()`.
4. **Forgot Password**: Tapping the "Forgot Password?" button shows a temporary message (Snackbar) as a placeholder for future implementation.
5. **Home Screen**: Displays a welcome message and a logout button. Pressing logout returns the user to the login screen.



## Demo Credentials
- **Email:** demo@example.com
- **Password:** password123

