# AWS Certified Cloud Practitioner (CLF-C02) Exam Simulator Suite

**Live Demo:** [AWS CLF-C02 Prep Suite](https://chinmay-aws-prep.netlify.app/)

---

## Overview

This project is a comprehensive, client-side web application designed to assist candidates in preparing for the AWS Certified Cloud Practitioner (CLF-C02) exam. It consists of **three distinct study modules**: a full-featured Exam Simulator for timed practice, an instant-feedback Practice Mode, and an interactive Flashcard application for concept reinforcement.

The suite is built with a modern, responsive design utilizing Glassmorphism aesthetics and supports both desktop and mobile environments. It comes pre-loaded with a question bank of 265 high-quality practice questions covering all exam domains.

## Features

### 1. Mock Exam Simulator (`mock.html`)
* **Realistic Exam Environment:** Simulates the actual testing interface with a global timer and optional per-question timers.
* **Review System:** Users can flag questions for review before submitting.
* **Navigation & Tracking:** Features a sidebar navigation grid to jump between questions, track answered status, and identify visited items.
* **Instant Feedback:** Provides a detailed results summary upon completion, including score percentage and pass/fail status.
* **Customizable Settings:** Users can define the number of questions per session and time limits.

### 2. Practice Mode (`practice.html`)
* **Instant Validation:** Immediate feedback on every question (Green for correct, Red for incorrect).
* **Drill-Style Learning:** Auto-advances after a correct answer to maintain flow.
* **Smart Scoring:** Calculates score based on visited questions only, allowing for casual, drop-in study sessions.
* **Domain Context:** Displays the specific exam domain (e.g., "Security", "Billing") for every question to help categorize knowledge.

### 3. Flashcard Study Mode (`flashcard.html`)
* **Spaced Repetition:** Users can mark difficult cards as "Favorites" to filter and focus on specific weak points.
* **Interactive Interface:** Features 3D card flip animations for an engaging study experience.
* **Mobile-Optimized:** A layout specifically designed for mobile devices with thumb-friendly controls.

### General Application Features
* **Modern UI/UX:** A polished interface featuring Glassmorphism, smooth transitions, and animated backgrounds.
* **Theme Support:** Fully supported Light and Dark modes with persistent user preference storage.
* **Data Flexibility:** Supports Drag & Drop functionality to load custom Question Bank JSON files.
* **Zero Dependencies:** Built entirely with vanilla HTML, CSS, and JavaScript. No external libraries or backend servers are required.

## File Structure

* **index.html**: The main Landing Page/Hub to access all tools.
* **mock.html**: The Exam Simulator application.
* **practice.html**: The Practice Mode application with instant feedback.
* **flashcard.html**: The Flashcard application.
* **schema.html**: Documentation and AI prompt generator for creating compatible Question Bank JSON files.
* **style.css**: Global stylesheet containing variables, themes, and layout definitions for all pages.
* **script.js**: The core logic engine handling the Exam Simulator functionality.
* **questions.json**: The internal data file containing the 265 practice questions.

## Getting Started

### Prerequisites
A modern web browser (Chrome, Firefox, Safari, or Edge).

### Installation and Usage

1.  **Download:** Clone the repository or download the source files to your local machine.
2.  **Running the Application:**
    * **Basic Usage:** Open `index.html` directly in your browser to access the suite. Note that strictly local file access (`file://` protocol) may restrict the "Use Internal Bank" button due to browser CORS security policies.
    * **Recommended Usage:** For full functionality, including the ability to fetch the internal `questions.json` file via the button click, serve the folder using a local development server.
        * If using VS Code, right-click `index.html` and select **"Open with Live Server"**.
        * Alternatively, using Python: run `python -m http.server` in the directory and navigate to `localhost:8000`.

3.  **Loading Data:**
    * Click "Use Internal Bank" (or "Load" in Practice Mode) to load the pre-configured 265 questions.
    * Alternatively, drag and drop a valid `questions.json` file onto the upload zone.

## Customizing Question Banks

You can extend the application by creating your own JSON question files. The application accepts an array of objects adhering to a specific schema.

To learn more about the required data structure or to generate new questions using AI tools, open **schema.html** in your browser (or access it via the "Data & AI" card on the home page). This page provides:
* A detailed table of the JSON schema requirements.
* Example JSON code blocks.
* A pre-written prompt optimized for Large Language Models to generate valid question datasets.

## License

This project is available for educational and personal use.