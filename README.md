# Flutter Firebase Authentication Application

This is a Flutter-based application that leverages Firebase for robust and secure user authentication. The application allows for user registration, login with email and password, as well as provides the ability to sign out.

## Table of Contents
1. [Features](#features)
2. [Firebase Integration](#firebase-integration)
3. [Project Structure](#project-structure)
4. [Screenshots](#screenshots)

## Features
- **User Registration:** New users can create an account using their email and password. User data is securely stored and managed in Firebase's Firestore database.
- **User Login:** Registered users can log in using their credentials. This application uses Firebase's `signInWithEmailAndPassword` method for secure authentication.
- **User Logout:** Users also have the ability to log out, with their sessions being managed securely.
- **Persistent Authentication State:** The application maintains the user's login state, even after it's closed and restarted.

## Firebase Integration
Firebase plays a crucial role in this application as it handles user registration, authentication, session management, and data storage. Firebase's Firestore database is used for storing user credentials securely. This application utilizes Firebase's Authentication library to facilitate the login and registration process.

## Project Structure
- `main.dart`: The entry point of the application. Firebase is initialized here.
- `AuthPage`: This page checks the user's authentication status. It directs the user to the `HomePage` if they're logged in, or to the `LoginOrRegister` page if they're not.
- `LoginOrRegister`: Here, the user can choose to either log in or register a new account. The page toggles between the `LoginPage` and `RegisterPage`.
- `LoginPage` and `RegisterPage`: These pages contain forms for the user to enter their credentials (email and password). The Register page also ensures password confirmation.
- `HomePage`: After a successful login, the user is redirected to the `HomePage`, which displays the user's email. It also includes a button for signing out.
- Custom Components: These include `MyButton` (a custom styled button), `MyTextField` (a custom text field with consistent styling), and `SquareTile` (a custom widget for displaying images).

## Screenshots
<p float="left">
  <img src="Simulator Screen Shot - iPhone 14 Plus - 2023-05-25 at 15.46.33.png" width="200">
  <img src="Simulator Screen Shot - iPhone 14 Plus - 2023-05-25 at 15.46.49.png" width="200">
  <img src="Simulator Screen Shot - iPhone 14 Plus - 2023-05-25 at 15.47.06.png" width="200">
  <img src="Simulator Screen Shot - iPhone 14 Plus - 2023-05-26 at 16.05.40.png" width="200">
</p>
