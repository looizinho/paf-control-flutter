# Project Blueprint

## Overview

This document outlines the style, design, and features of the Flutter application. It serves as a single source of truth for the project's current state and future development plans.

## Current Implementation

### Style and Design

*   **UI Framework:** Flutter
*   **Design System:** Material Design 3
*   **Theming:** Centralized `ThemeData` with support for light and dark modes.
*   **Color Scheme:** Generated from a seed color (`Colors.deepPurple`) using `ColorScheme.fromSeed`.
*   **Typography:** Custom typography using the `google_fonts` package.

### Features

*   **Theme Toggle:** Users can switch between light, dark, and system theme modes.
*   **State Management:** `provider` is used for managing the application's theme state.

## Plan for Current Request: Implement Material Design 3

The user has requested to implement Material Design 3 in the project. The following steps will be taken:

1.  **Add Dependencies:** Add the `google_fonts` and `provider` packages to `pubspec.yaml`.
2.  **Create Theme Provider:** Create a `ThemeProvider` class to manage the application's theme state.
3.  **Implement Theme Data:** Define light and dark `ThemeData` using `ColorScheme.fromSeed` and `google_fonts`.
4.  **Update `main.dart`:**
    *   Wrap the application in a `ChangeNotifierProvider` to make the `ThemeProvider` available to the widget tree.
    *   Use a `Consumer` to rebuild the `MaterialApp` when the theme changes.
    *   Add a `MyHomePage` with a theme toggle button in the `AppBar`.
    *   Apply custom text styles and button themes.
5.  **Verify Implementation:** Run the application to ensure the theme is applied correctly and the toggle functionality works as expected.
