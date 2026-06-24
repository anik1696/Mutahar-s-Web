# QuizForge Platform

QuizForge is a comprehensive, front-end only Learning Management System (LMS) and Quiz Platform built with vanilla Javascript, ES modules, and modern CSS architecture. Designed as a seamless Single Page Application (SPA), it provides an immersive educational experience without the overhead of heavy frameworks.

This repository contains the complete frontend architecture, mock-data integrations, and interactive UI components.

---

## 🌟 Elaborated Feature List

Below is a highly detailed breakdown of the features, systems, and interfaces currently implemented in this repository.

### 1. Core Architecture & UI/UX Systems
*   **Single Page Application (SPA) Routing**: Custom, lightweight vanilla JS router that seamlessly transitions between 14+ unique views without page reloads.
*   **Stateful Theme Engine**: Fully integrated Light and Dark modes. The application dynamically swaps color palettes, background gradients, and text contrast rules based on user preference, with choices persisting across sessions via `localStorage`.
*   **Modern CSS & Glassmorphism**: Utilizes advanced CSS variables, Flexbox, CSS Grid, frosted glass effects (backdrop-blur), and pill-shaped UI components (`card-pill`) for a premium, modern aesthetic.
*   **Responsive Scaling**: Mobile-first design that effortlessly scales. Features include a bottom-sheet mobile navigation menu, a collapsible desktop sidebar, and fluid grid layouts.
*   **Custom Print Media Queries**: Dedicated `@media print` CSS logic that automatically strips away navigation bars, dark backgrounds, and interactive buttons, ensuring documents (like invoices or quiz results) look clean and professional on physical paper.

### 2. Public & Monetization Pages
*   **Dynamic Landing Page**: A marketing-focused hero section featuring custom SVG wavy dividers, dynamic gradient background meshes, and high-conversion call-to-action buttons.
*   **Authentication Flows**: Mock interfaces for Student and Educator Login and Registration, maintaining the core design language.
*   **Tiered Pricing Page**: A robust pricing table offering 4 distinct tiers (Basic, Silver, Gold, Premium). Includes dynamic UI highlighting (scaling, glowing borders) for the "Most Popular" Gold tier, and a secondary grid showcasing unlockable Premium Courses based on subscription level.
*   **Secure Checkout System**: A split-screen checkout flow that securely collects personal details (Name, Email, Phone) and mock payment information (Card, Expiry, CVC), paired with a sticky, real-time Order Summary sidebar.
*   **Digital Invoice Generator**: Upon successful checkout, the system generates a printable digital receipt containing randomized Order IDs, mapped customer details, and an itemized purchase breakdown.

### 3. Student & Educator Dashboards
*   **Student Learning Hub**: A personalized dashboard that tracks active learning progress. Features include a dynamic level indicator, XP counters, login streak trackers, a list of upcoming scheduled quizzes, and a GitHub-style heatmap displaying recent activity.
*   **Educator / Admin Overview**: A high-level control panel providing critical platform statistics (total quizzes, average platform scores, active students). Includes a responsive table monitoring recent quiz deployments and quick-action shortcuts for course management.

### 4. Interactive Quiz Engine
*   **Pre-Quiz Lobby**: An interstitial preparation screen that informs users of the quiz parameters (total questions, time limits, difficulty) before the timer begins.
*   **Immersive Quiz Player**: A distraction-free interface for taking assessments. Features include:
    *   A live, ticking countdown timer.
    *   A dynamic progress bar indicating completion percentage.
    *   Support for multiple question formats (Multiple Choice, True/False).
    *   Interactive, selectable answer cards with hover states.
*   **Detailed Results Breakdown**: A post-assessment screen that calculates the final score and XP earned. It provides a question-by-question review, highlighting correct/incorrect answers and providing detailed explanations for each topic.

### 5. Content Management System (CMS)
*   **Quiz Library Explorer**: A visual grid of all available quizzes across the platform, complete with difficulty badges, user counts, and descriptive metadata. Includes layouts intended for search and filtering.
*   **Quiz Builder Interface**: A mock authoring tool for educators to construct new quizzes, configure time limits, and append questions.
*   **Centralized Question Bank**: A powerful data-table interface for managing a global repository of questions. Displays question types, assigned subjects, difficulty levels, usage counts, and historical pass rates.

### 6. Platform Mechanics & Administration
*   **Gamification Hub**: A dedicated page for user engagement, featuring a global XP leaderboard comparing peer performance, unlockable achievement badges (e.g., "Speed Demon", "Perfect Score"), and visual progression tracking.
*   **Analytics & Reporting**: Visual data representations using mock charts that track weekly student activity, subject-specific performance metrics, and platform-wide score distributions.
*   **User Management Console**: Administrative tools for viewing, editing, and suspending user accounts. Displays active/inactive statuses, assigned roles (Admin, Instructor, Student), and engagement metrics.
*   **System Settings**: A centralized configuration menu allowing users to edit profile details, toggle email notification preferences, and manage third-party LMS integrations (e.g., Canvas, Moodle, Google Classroom).

---

## 💻 Running the Project

Because this project utilizes native ES Modules (`import`/`export`), the files must be served over a local HTTP server rather than opening the HTML file directly in a browser.

**Using Node.js:**
\`\`\`bash
npx serve .
\`\`\`
Then navigate to \`http://localhost:3000\` in your browser!
