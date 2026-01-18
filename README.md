# AWS Certified Cloud Practitioner (CLF-C02) Exam Simulator Suite

**Live Demo:** [Mock Test](https://chinmay-aws-prep.netlify.app/) | [Flashcards](https://chinmay-aws-prep.netlify.app/flashcard/)

---

## Overview

This project is a comprehensive, client-side web application designed to assist candidates in preparing for the AWS Certified Cloud Practitioner (CLF-C02) exam. It consists of two distinct study modules: a full-featured Exam Simulator for timed practice and an interactive Flashcard application for concept reinforcement.

The suite is built with a modern, responsive design utilizing Glassmorphism aesthetics and supports both desktop and mobile environments. It comes pre-loaded with a question bank of 265 high-quality practice questions covering all exam domains.

## Features

### Exam Simulator

- **Realistic Exam Environment:** Simulates the actual testing interface with a global timer and optional per-question timers.
- **Comprehensive Question Bank:** Includes 265 built-in questions covering Cloud Concepts, Security, Technology, and Billing.
- **Navigation & Tracking:** Features a sidebar navigation grid to jump between questions, track answered status, and identify visited items.
- **Review System:** Users can flag questions for review before submitting.
- **Instant Feedback:** Provides a detailed results summary upon completion, including score percentage and pass/fail status.
- **Customizable Settings:** Users can define the number of questions per session and time limits.

### Flashcard Study Mode

- **Interactive Interface:** Features 3D card flip animations for an engaging study experience.
- **Spaced Repetition Tools:** Users can mark difficult cards as "Favorites" to filter and focus on specific weak points.
- **Mobile-Optimized:** A layout specifically designed for mobile devices with thumb-friendly controls.
- **Contextual Learning:** Displays the specific exam domain for every question to help categorize knowledge.

### General Application Features

- **Modern UI/UX:** A polished interface featuring Glassmorphism, smooth transitions, and animated backgrounds.
- **Theme Support:** Fully supported Light and Dark modes with persistent user preference storage.
- **Data Flexibility:** Supports Drag & Drop functionality to load custom Question Bank JSON files.
- **Zero Dependencies:** Built entirely with vanilla HTML, CSS, and JavaScript. No external libraries or backend servers are required.

## File Structure

- **index.html**: The entry point for the Exam Simulator.
- **flashcard.html**: The entry point for the Flashcard Study Mode.
- **schema.html**: Documentation and AI prompt generator for creating compatible Question Bank JSON files.
- **style.css**: Global stylesheet containing variables, themes, and layout definitions for all pages.
- **script.js**: The core logic engine handling the Exam Simulator functionality.
- **questions.json**: The internal data file containing the 265 practice questions.

## Getting Started

### Prerequisites

A modern web browser (Chrome, Firefox, Safari, or Edge).

### Installation and Usage

1. **Download:** Clone the repository or download the source files to your local machine.
2. **Running the Application:**
    - **Basic Usage:** You can open `index.html` or `flashcard.html` directly in your browser. Note that strictly local file access (file:// protocol) may restrict the "Use Internal Bank" button due to browser CORS security policies.
    - **Recommended Usage:** For full functionality, including the ability to fetch the internal `questions.json` file via the button click, serve the folder using a local development server.
        - If using VS Code, right-click `index.html` and select **"Open with Live Server"**.
        - Alternatively, using Python: run `python -m http.server` in the directory and navigate to `localhost:8000`.

3. **Loading Data:**
    - Click "Use Internal Bank" to load the pre-configured 265 questions.
    - Alternatively, drag and drop a valid `questions.json` file onto the upload zone.

## Customizing Question Banks

You can extend the application by creating your own JSON question files. The application accepts an array of objects adhering to a specific schema.

To learn more about the required data structure or to generate new questions using AI tools, open **schema.html** in your browser. This page provides:

- A detailed table of the JSON schema requirements.
- Example JSON code blocks.
- A pre-written prompt optimized for Large Language Models to generate valid question datasets.

## License

This project is available for educational and personal use.
