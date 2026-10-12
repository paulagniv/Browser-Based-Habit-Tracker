# Browser-Based Habit Tracker

A lightweight, privacy-focused daily habit tracker that runs entirely in your web browser. This project was built to provide a simple, distraction-free way to manage daily goals without requiring user accounts, internet connectivity, or complex setups.

## 🎯 Purpose

**User Functionality:** 
Provides a digital checklist where users can input daily habits, mark them as complete, and delete them when no longer needed. It is designed to be frictionless and instantly accessible.

**Technical Demonstration:** 
Built as a hackathon project to demonstrate how to build a fully interactive, persistent web application using only standard front-end web languages. It achieves data persistence locally without needing a backend server, external database, or internet connection.

## 🏗️ Architecture & Technologies

This project operates on a completely serverless, client-side architecture. All processing and data storage happen locally on the user's device.

*   **User Interface (UI):** Vanilla HTML5 and CSS3. Utilizes CSS variables for easy theming (e.g., expanding to Dark Mode).
*   **Application Logic:** Vanilla JavaScript (ES6+). Handles DOM manipulation, event listening, and state management without the need for heavy frameworks like React or Angular.
*   **Data Storage:** Web Storage API (`localStorage`). State is serialized into JSON and saved directly to the browser's local storage. This ensures that user data persists across page reloads and browser sessions without a database.

### System Flow
1. User enters a habit into the UI.
2. JavaScript captures the input, updates the local state array, and saves the new array to `localStorage`.
3. The DOM is re-rendered to reflect the current state.
4. On subsequent page loads, JavaScript fetches and parses the JSON from `localStorage` to rebuild the user's list.

## ✨ Features

*   **Add Habits:** Quickly add new habits to your daily list using the input field or the `Enter` key.
*   **Toggle Completion:** Click on any habit to strike it through and mark it as completed for the day.
*   **Delete Habits:** Remove habits from your list with a dedicated delete button.
*   **Persistent Data:** Your list automatically saves to your browser. You can safely close the tab and return later without losing your progress.
*   **Zero Dependencies:** No external libraries, packages, or APIs to install or configure.

## 🚀 How to Run

Because this project requires no build tools or servers, running it is incredibly simple:

1. Clone this repository to your local machine (or download the ZIP file):
   ```bash
   git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)