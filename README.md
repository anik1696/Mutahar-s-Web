# QuizForge

A lightweight, front-end only quiz and learning management platform built with vanilla JS and modern CSS.

This repository contains the full UI and mock-data implementation. It's built as a Single Page Application (SPA) without heavy frameworks, relying on native ES modules and Vue.js for state management and rendering.

## Current Feature Set

Here is exactly what is currently built and working in the project:

### 1. Core Architecture & UI
*   **Fully Responsive Layout**: Mobile-first design that scales up to desktop with a collapsible sidebar and sticky top navigation.
*   **Theme Engine**: Built-in Light and Dark mode that saves to `localStorage`. Uses custom CSS variables and glassmorphism UI elements (frosted glass effects).
*   **Custom Print Styles**: Dedicated `@media print` CSS that strips out navbars and dark backgrounds for clean, paper-friendly printing.

### 2. Public Pages
*   **Landing Page**: Marketing hero section, wavy SVG dividers, and quick links.
*   **Auth Flow**: Mock Login and Registration pages.
*   **Pricing Page**: 4-tier pricing table (Basic, Silver, Gold, Premium) with dynamic highlighting for the "Popular" tier and a premium course showcase.
*   **Checkout System**: A split-screen checkout form collecting personal and payment details, complete with a live updating order summary.
*   **Invoice Generator**: Upon checkout completion, generates a digital receipt with randomized order IDs that can be saved as a PDF or printed.

### 3. Dashboards
*   **Student Dashboard**: Tracks learning progress, current level, XP, login streaks, upcoming quizzes, and a GitHub-style activity heatmap.
*   **Educator/Admin Dashboard**: High-level stats overview (total quizzes, average scores), recent quiz activity tables, and quick action shortcuts.

### 4. Quiz Engine
*   **Quiz Lobby**: Pre-quiz screen showing total questions, time limits, and instructions.
*   **Active Quiz Player**: Immersive, full-screen quiz interface featuring a countdown timer, progress bar, and support for multiple question types (MCQ, True/False).
*   **Results Page**: Post-quiz breakdown showing the final score, XP earned, and detailed explanations for correct/incorrect answers.

### 5. Content Management
*   **Quiz Library**: Grid view of all available quizzes with search and filter layouts.
*   **Quiz Builder**: Interface for creating new quizzes and adding questions.
*   **Question Bank**: A centralized table managing individual questions, their difficulty, tags, and pass rates.

### 6. Platform Features
*   **Gamification Hub**: Global leaderboards, unlockable achievement badges, and level progression tracking.
*   **Analytics**: Mock charts mapping score distributions and weekly student activity.
*   **User Management**: Admin tables for viewing, editing, and managing active users and their roles.
*   **Settings**: User preferences including profile management, notification toggles, and integration connections.

## Running the Project

No build step required. Just serve the directory locally.

If you use Node:
\`\`\`bash
npx serve .
\`\`\`
Then open `http://localhost:3000`.
