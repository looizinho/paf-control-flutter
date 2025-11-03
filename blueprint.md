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

## Plan for Current Request: Create UI from Image

The user has requested to create a UI based on an image. The following steps will be taken:

1.  **Update Theme:** Set the default theme to dark mode to match the image's aesthetic. Modify the dark `ThemeData` to use a black background and `robotoMono` as the primary font.
2.  **Create New UI in `MyHomePage`:**
    *   Replace the existing content of `MyHomePage` with a new layout.
    *   Add an `AppBar` with the title "Memorial PAF - Controle".
    *   The body will contain three columns for "O PEDRO", "LINHA DO TEMPO", and "MULTIPLIQUE-SE".
3.  **Create Reusable Widgets:**
    *   `CategoryCard`: A widget to display a column with a title and two buttons.
    *   `LanguageButton`: A styled button with a flag emoji and text ("Português" or "Inglês").
4.  **Styling:**
    *   Use a dark theme with a black background.
    *   Apply borders and rounded corners to cards and buttons to match the visual design in the image.
    *   Use the `robotoMono` font from `google_fonts` for a consistent look.
5.  **File Updates:** Update `lib/main.dart` with the new UI code and `blueprint.md` with the plan.
