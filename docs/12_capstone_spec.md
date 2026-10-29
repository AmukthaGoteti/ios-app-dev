# Capstone Project: The Unified Knowledge Ecosystem

The Capstone Project is the ultimate validation of your journey. You will design and build a professional-grade, multi-platform application that leverages a shared business logic layer to provide native experiences across four different Apple platforms.

## 1. The Vision
Create a **"Personal Knowledge Base"** (similar to Notion or Obsidian) that allows users to capture, organize, and visualize information across their entire device ecosystem.

## 2. Platform-Specific Experiences
The core business logic is shared, but the UI must be native to each platform:

### iOS (The Capture Tool)
*   **Focus:** Speed and mobility.
*   **Key Features:** Quick-entry notes, voice-to-text capture, and a simplified "reading mode."
*   **Specialization:** Use a specialized "Quick Capture" widget for the home screen.

### macOS (The Powerhouse)
*   **Focus:** Organization and depth.
*   **Key Features:** Multi-column layout, advanced search, bulk editing, and a dedicated "Graph View" for visualizing note connections.
*   **Specialization:** Implement a Menu Bar utility for quick-notes and a native "File-based" import/export system.

### watchOS (The Reminder)
*   **Focus:** Glanceability.
*   **Key Features:** View "Top 3" tasks for the day, mark tasks as complete, and set quick reminders.
*   **Specialization:** A watch-face complication that shows the current active focus task.

### visionOS (The Mind-Map)
*   **Focus:** Spatial visualization.
*   **Key Features:** An immersive 3D "Brain" where notes are nodes in space. Users can move notes and connect them physically.
*   **Specialization:** A "Volumetric Window" that allows users to see their knowledge graph in 3D and "jump" into a specific note.

---

## 3. Technical Requirements (The Engineering Standard)

### Architecture & Modularization
*   **SPM Structure:** The project MUST be split into modules:
    *   `KBCore`: Pure Swift logic, Models, and Protocol-based services.
    *   `KBNetworking`: API clients and CloudKit logic.
    *   `KBUIComponents`: Shared SwiftUI views and design system.
    *   `KB-iOS`, `KB-macOS`, etc.: Platform-specific app targets.
*   **Pattern:** Use MVVM or TCA to ensure unidirectional data flow.

### Persistence & Sync
*   **Database:** Use **SwiftData** for local storage.
*   **Synchronization:** Use **CloudKit** for real-time sync across all four platforms.
*   **Offline-First:** The app must be fully functional offline and sync seamlessly when online.

### Quality & Engineering
*   **Testing:** 
    *   Unit tests for all `KBCore` logic (Target: >80% coverage).
    *   Integration tests for the CloudKit sync flow.
    *   UI tests for the primary "Create Note" flow on iOS and macOS.
*   **Concurrency:** 100% Swift 6 strict concurrency compliance. Zero data races.
*   **Accessibility:** Full VoiceOver and Dynamic Type support on all platforms.

---

## 4. Definition of Done
1.  **Multi-Platform:** All 4 apps build and run without crashes.
2.  **Seamless Sync:** A note created on the Watch appears on the Mac and Vision Pro in under 5 seconds.
3.  **Native UX:** Each app follows its respective platform's HIG (e.g., Mac has a menu bar, Watch has a complication).
4.  **Professional Code:** The project is modularized via SPM and passes the "Senior Standard" code review.
5.  **Documentation:** A complete `README.md` explaining the architecture and a "Case Study" documenting one major technical challenge and its solution.
