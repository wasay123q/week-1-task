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

## How to Run

1. **Prerequisites**:
   - [Flutter SDK](https://flutter.dev/docs/get-started/install) installed
   - Android Studio, VS Code, or any preferred IDE
   - An emulator or a physical device for testing

2. **Clone the Repository** (if applicable):
   ```sh
   git clone <repository-url>
   cd login_app
   ```

3. **Install Dependencies**:
   ```sh
   flutter pub get
   ```

4. **Run the App**:
   - For Android/iOS:
     ```sh
     flutter run
     ```
   - For Web:
     ```sh
     flutter run -d chrome
     ```

## Demo Credentials
- **Email:** demo@example.com
- **Password:** password123

## Screenshots

> Add screenshots here if needed (e.g., login screen, home screen)

## Customization
- You can expand this app by adding real authentication, persistent login, or connecting to a backend.
- The UI can be further customized using Flutter's rich widget library.

## License

This project is for educational purposes and does not include any authentication backend. Feel free to use and modify it for your learning needs.
