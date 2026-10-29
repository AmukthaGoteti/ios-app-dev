# Testing & Assessment Framework

This document establishes the quality standards and measurement tools used to evaluate progress throughout the Apple Ecosystem Engineering Masterclass.

## 1. Module Completion Standards
A module is not considered "Complete" until the following criteria are met:
*   **Theory:** All syllabus topics read and knowledge-check questions answered.
*   **Practice:** All guided exercises completed and verified.
*   **Output:** The independent assignment is pushed to GitHub with a professional commit history.
*   **Validation:** The practical assessment is passed according to the rubric.

## 2. Code Quality Rubric (The "Senior Standard")
Every project and assignment is graded against these four pillars:

| Pillar | Poor (1-2) | Proficient (3-4) | Expert (5) |
| :--- | :--- | :--- | :--- |
| **Correctness** | App crashes; logic errors; fails basic requirements. | Works as intended; occasional edge-case bugs. | Zero crashes; handles all edge cases; bug-free. |
| **Architecture** | "Massive View"; logic in UI; no separation of concerns. | Clear MVVM/TCA; logic separated from UI. | Fully modularized; dependency inverted; highly testable. |
| **Swift Idioms** | Uses `!` everywhere; ignores `async/await`; legacy patterns. | Correct use of Optionals and Concurrency. | Expert use of Generics, POP, and strict concurrency safety. |
| **User Exp (UX)** | Non-responsive; ignores HIG; no accessibility. | Follows basic HIG; accessible in core areas. | Pixel-perfect; fluid animations; 100% VoiceOver compliant. |

## 3. Project Evaluation Matrix
Projects are evaluated using a weighted score:
*   **Functional Requirements (40%):** Does it do what it's supposed to do?
*   **Technical Implementation (30%):** Is the code professional, safe, and efficient?
*   **UX & Accessibility (20%):** Does it feel like a native Apple app?
*   **Testing & Documentation (10%):** Are there tests? Is the README clear?

## 4. Debugging Exercises (The "Break-Fix" Method)
To ensure deep understanding, learners must complete "Break-Fix" challenges:
1.  **The Memory Leak:** Given an app with a hidden retain cycle $\rightarrow$ Find and fix it.
2.  **The Race Condition:** Given an app that crashes randomly during concurrent writes $\rightarrow$ Fix using Actors.
3.  **The Layout Bug:** Given a UI that clips on iPhone SE but looks fine on iPhone 15 $\rightarrow$ Fix using adaptive layouts.

## 5. Final Competency Exam
The program concludes with a three-part examination:
1.  **Theoretical:** A deep-dive interview on Swift 6 concurrency and ARC.
2.  **Practical:** A 48-hour "Feature Sprint" where the learner must implement a specific feature into an existing codebase.
3.  **Architectural:** A system design session where the learner must map out the modules for a multi-platform app.
