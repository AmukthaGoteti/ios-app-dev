# Project Portfolio Specifications

This document defines the eight progressive projects required to complete the Apple Ecosystem Engineering Masterclass. Each project is designed to prove mastery of specific phases of the curriculum.

---

## Project 1: Swift Fundamentals CLI (The "Logic Engine")
**Goal:** Prove mastery of the Swift language without the distraction of a UI.
*   **Problem Statement:** Build a Command-Line Interface (CLI) tool that manages a personal finance ledger.
*   **Functional Requirements:**
    *   Add, remove, and categorize transactions.
    *   Calculate total balance and spending per category.
    *   Export a summary report to a `.txt` file.
*   **Technical Requirements:**
    *   Use a `struct` for Transactions and an `enum` for Categories.
    *   Implement a `Protocol` for "Exportable" data.
    *   Use Generics to handle different currency types.
*   **Definition of Done:** CLI runs without crashes; all calculations are mathematically correct; export file is generated correctly.

## Project 2: Polished SwiftUI Productivity App (The "UI showcase")
**Goal:** Demonstrate mastery of declarative UI, state management, and adaptive layout.
*   **Problem Statement:** Create a "Focus Timer & Task Tracker" app.
*   **Functional Requirements:**
    *   Customizable Pomodoro timer with visual progress.
    *   Task list with priority levels and checkboxes.
    *   Settings page for timer durations and notification preferences.
*   **Technical Requirements:**
    *   Use the `@Observable` framework for state.
    *   Implement custom animations for the timer transition.
    *   Ensure full Accessibility (VoiceOver) support.
*   **Definition of Done:** UI matches a high-fidelity design; timer runs accurately in the background; accessible to screen readers.

## Project 3: API-Driven iOS App (The "Production Ready")
**Goal:** Implement a full-stack mobile experience with networking and persistence.
*   **Problem Statement:** Build a "Movie Discovery App" using a public API (e.g., TMDB).
*   **Functional Requirements:**
    *   Search for movies and browse "Trending" lists.
    *   "Favorites" list that persists offline.
    *   User authentication (Sign up / Log in).
*   **Technical Requirements:**
    *   Generic `NetworkManager` using `async/await`.
    *   `SwiftData` for local favorites storage.
    *   MVVM Architecture.
*   **Definition of Done:** App fetches and renders real API data; favorites are saved across app restarts; authentication flow is secure.

## Project 4: Adaptive iPad App (The "Canvas")
**Goal:** Mastery of multitasking and large-screen interaction.
*   **Problem Statement:** Build a "Digital Notebook" with a split-pane interface.
*   **Functional Requirements:**
    *   Sidebar for notebook organization.
    *   Main area for rich-text editing.
    *   Detail pane for note metadata (date, tags).
*   **Technical Requirements:**
    *   `NavigationSplitView` for adaptive layout.
    *   Keyboard shortcut support (Cmd+N for new note).
    *   Drag and Drop for rearranging notes.
*   **Definition of Done:** App functions correctly in Split View and Slide Over; keyboard shortcuts work; layout adapts to orientation changes.

## Project 5: Native macOS App (The "Desktop Powerhouse")
**Goal:** Implement native desktop conventions.
*   **Problem Statement:** Build a "System Resource Monitor & Process Manager."
*   **Functional Requirements:**
    *   Live CPU/RAM usage graphs.
    *   List of running processes with the ability to "Kill" a process.
    *   Menu bar utility for quick-glance usage.
*   **Technical Requirements:**
    *   `NSViewRepresentable` for custom graph drawing.
    *   `NSOpenPanel` for selecting log files.
    *   App Sandbox configuration for system access.
*   **Definition of Done:** App follows macOS HIG; menu bar item works independently; process killing is functional.

## Project 6: watchOS Companion (The "Wrist Extension")
**Goal:** Designing for extreme constraints and device connectivity.
*   **Problem Statement:** Build a "Fitness Tracker Companion" for the iOS app.
*   **Functional Requirements:**
    *   Start/Stop workout from the watch.
    *   Real-time heart rate display (via HealthKit).
    *   Push notifications for workout milestones.
*   **Technical Requirements:**
    *   `WCSession` for bi-directional sync with iPhone.
    *   Custom Complication for the watch face.
    *   Efficient background refresh for the complication.
*   **Definition of Done:** Workout state is synced between iPhone and Watch; heart rate is read correctly; complication updates every 15 mins.

## Project 7: visionOS Spatial Experience (The "Immersive")
**Goal:** Mastering 3D interaction and spatial UI.
*   **Problem Statement:** Create a "Virtual Museum of Art."
*   **Functional Requirements:**
    *   Immersive space with 3D gallery.
    *   Interactable 3D artifacts (zoom, rotate, info).
    *   Adaptive UI windows that float in the room.
*   **Technical Requirements:**
    *   `RealityKit` for 3D entities and lighting.
    *   USDZ asset pipeline using Reality Composer Pro.
    *   Gaze-and-pinch interaction for artifact selection.
*   **Definition of Done:** App maintains 90 FPS; 3D assets are placed correctly in the room; spatial audio works as the user moves.

## Project 8: The Capstone (The "Unified Ecosystem")
**Goal:** The ultimate proof of mastery: one codebase, multiple native experiences.
*   **Problem Statement:** Build a "Personal Knowledge Base" (similar to Notion or Obsidian).
*   **Functional Requirements:**
    *   Shared business logic for note synchronization.
    *   **iOS:** Mobile capture and quick-read.
    *   **macOS:** Full-featured editor and organizational tool.
    *   **watchOS:** Quick-view of "Top Tasks" and reminders.
    *   **visionOS:** Immersive "Mind Map" of connected notes.
*   **Technical Requirements:**
    *   **SPM Modularization:** `CoreLogic`, `CoreUI`, `PlatformiOS`, `PlatformmacOS`, etc.
    *   **Persistence:** SwiftData + CloudKit for cross-device sync.
    *   **Architecture:** Advanced MVVM or TCA.
    *   **Quality:** >80% Unit Test coverage.
*   **Definition of Done:** One codebase producing 4 distinct, high-quality apps; data syncs perfectly across all four devices; project is modularized and documented.
