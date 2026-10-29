## Phase 4: iOS and iPadOS Development
**Objective:** Transform shared SwiftUI knowledge into a production-ready mobile experience.

### Module 4.1: The iOS App Lifecycle & Scene Management
*   **Difficulty:** Intermediate
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Phase 3
*   **Learning Outcomes:** Managing the app's state across foreground, background, and suspended modes.
*   **Syllabus:**
    *   `@main` and the `App` protocol.
    *   `ScenePhase`: Active, Inactive, and Background.
    *   The Windows/Scenes model: Handling multiple windows on iPadOS.
    *   Deep Linking & Universal Links: Bringing users to specific content.
*   **Core Concepts:**
    *   *Suspension:* How iOS kills apps to save memory and how to restore state.
    *   *Scene-based Architecture:* The shift from a single-window app to a multi-window system.
*   **Guided Exercise:** Implement a "Save Progress" feature that triggers exactly when the app moves to the background.
*   **Independent Assignment:** Build an iPad app that supports "Split View" and "Slide Over" with a distinct UI for each.
*   **Common Mistakes:** Assuming the app is always "Active"; failing to handle state restoration after a system-initiated kill.
*   **Practical Assessment:** Create a deep-link handler that opens the app to a specific product page from a web URL.
*   **Completion Criteria:** App correctly handles lifecycle transitions without losing user data.
*   **Next Module:** 4.2 UIKit Interop & Advanced Interaction.

### Module 4.2: UIKit Interop & Advanced Interaction
*   **Difficulty:** Intermediate
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Module 4.1
*   **Learning Outcomes:** Bridging the gap between the modern declarative world and the powerful imperative world.
*   **Syllabus:**
    *   `UIViewRepresentable`: Putting UIKit views in SwiftUI.
    *   `UIViewControllerRepresentable`: Putting UIKit controllers in SwiftUI.
    *   Coordinator Pattern: Handling delegates and data flow between UIKit and SwiftUI.
    *   Advanced Interaction: Context Menus, Drag and Drop, and Swipe Actions.
*   **Core Concepts:**
    *   *The Bridge:* How to wrap a legacy `MKMapView` or `UIImagePickerController` for use in SwiftUI.
    *   *The Coordinator:* Acting as the "middleman" to translate UIKit events into SwiftUI state changes.
*   **Guided Exercise:** Wrap a `UITextView` to create a rich-text editor in SwiftUI.
*   **Independent Assignment:** Implement a "Drag and Drop" feature where users can drag a photo from one folder view to another.
*   **Common Mistakes:** Attempting to manage SwiftUI state inside a UIKit view directly; forgetting to update the Coordinator.
*   **Practical Assessment:** Build a custom camera interface using `AVFoundation` wrapped in a SwiftUI view.
*   **Completion Criteria:** Seamless communication between the UIKit wrapper and the SwiftUI state.
*   **Next Module:** 4.3 Persistence with SwiftData & CloudKit.

### Module 4.3: Persistence with SwiftData & CloudKit
*   **Difficulty:** Advanced
*   **Duration:** 2 Weeks (25 hours)
*   **Prerequisites:** Module 4.2
*   **Learning Outcomes:** Building "Offline-First" apps with seamless cloud synchronization.
*   **Syllabus:**
    *   `Model` and `@Model`: Defining the schema.
    *   `ModelContainer` and `ModelContext`: Managing the data store.
    *   Querying: `@Query` and `FetchDescriptor`.
    *   Relationships: One-to-One, One-to-Many, Many-to-Many.
    *   CloudKit Integration: Enabling synchronization across devices.
    *   Migration: Handling schema changes in production.
*   **Core Concepts:**
    *   *The Model Graph:* How SwiftData tracks changes to objects.
    *   *Automatic Sync:* The magic of CloudKit without writing backend code.
*   **Guided Exercise:** Build a "Note Taking" app with categories, where notes are automatically synced to the user's iCloud.
*   **Independent Assignment:** Implement a "Complex Data Model" (e.g., a Project Manager) with multiple nested relationships and a search filter.
*   **Common Mistakes:** Performing heavy database writes on the main thread; ignoring the "Private Cloud Database" permissions.
*   **Practical Assessment:** Perform a "Schema Migration" on an existing database without losing user data.
*   **Completion Criteria:** Data persists across app restarts and syncs across two different physical devices.
*   **Next Module:** 4.4 System Integrations (Widgets, Intents, Siri).

### Module 4.4: System Integrations (Widgets, Intents, Siri)
*   **Difficulty:** Intermediate
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Module 4.3
*   **Learning Outcomes:** Extending the app's reach beyond the main UI.
*   **Syllabus:**
    *   WidgetKit: Creating glanceable information for the Home Screen.
    *   App Intents: Defining actions the system can perform on behalf of the user.
    *   Siri & Shortcuts: Integrating the app into the iOS automation ecosystem.
    *   Live Activities: Real-time updates on the Lock Screen and Dynamic Island.
*   **Core Concepts:**
    *   *Timeline Provider:* How widgets decide what to show and when to refresh.
    *   *Intents:* The bridge between the user's intent and the app's code.
*   **Guided Exercise:** Build a "Weather Widget" that updates every hour.
*   **Independent Assignment:** Create a "Siri Shortcut" that allows the user to log a workout with a voice command.
*   **Common Mistakes:** Putting too much logic in the Widget (it must be lightweight); failing to handle "Expired" timelines.
*   **Practical Assessment:** Implement a Live Activity that tracks a delivery progress bar in the Dynamic Island.
*   **Completion Criteria:** Widget and Shortcut function correctly without requiring the main app to be open.
*   **Next Module:** Phase 5: macOS Development.

---

## Phase 5: macOS Development
**Objective:** Adapt the mobile mindset to the power and freedom of the Desktop.

### Module 5.1: Desktop Architecture & User Experience
*   **Difficulty:** Intermediate
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Phase 3
*   **Learning Outcomes:** Designing for a mouse, keyboard, and large screen.
*   **Syllabus:**
    *   Window Management: `WindowGroup`, `Window`, and multi-window support.
    *   The Menu Bar: `CommandMenu`, custom menu items, and status bar utilities.
    *   Toolbars & Sidebars: Using `NavigationSplitView` for desktop-class navigation.
    *   Keyboard Shortcuts: `.keyboardShortcut()` and handling key events.
    *   The App Sandbox: Entitlements, Hardened Runtime, and file system access.
*   **Core Concepts:**
    *   *Pointer-First Interaction:* Designing for hover states and right-clicks.
    *   *The Menu Bar Mindset:* Moving primary actions from buttons to the top menu.
*   **Guided Exercise:** Build a "System Monitor" utility that lives in the macOS Menu Bar.
*   **Independent Assignment:** Create a "Document-Based App" (like TextEdit) that allows opening multiple files in separate windows.
*   **Common Mistakes:** Simply "stretching" an iPhone UI to fit a Mac screen; forgetting to implement keyboard shortcuts for power users.
*   **Practical Assessment:** Implement a "Split View" navigation that allows the user to resize the sidebar and maintain state.
*   **Completion Criteria:** App follows macOS HIG (Human Interface Guidelines) for windowing and menu usage.
*   **Next Module:** 5.2 AppKit Interop & File System.

### Module 5.2: AppKit Interop & File System
*   **Difficulty:** Advanced
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Module 5.1
*   **Learning Outcomes:** Handling the complex file-system interactions unique to macOS.
*   **Syllabus:**
    *   `NSViewRepresentable`: Bringing AppKit components into SwiftUI.
    *   File Access: `NSOpenPanel`, `NSSavePanel`, and Security-Scoped Bookmarks.
    *   Drag and Drop (Desktop): Moving files from Finder into the app.
    *   Background Processes: Login items and helper apps.
*   **Core Concepts:**
    *   *Sandboxing:* Why you can't just read `/Users/name/Documents` without a user-selected panel.
    *   *The AppKit Bridge:* Using `NSWindow` for advanced window controls that SwiftUI doesn't yet offer.
*   **Guided Exercise:** Build a "File Converter" app that allows the user to select a folder of files via `NSOpenPanel`.
*   **Independent Assignment:** Implement a "Drop Zone" that accepts `.png` files dragged from the Mac desktop.
*   **Common Mistakes:** Failing to save "Security-Scoped Bookmarks," causing the app to lose access to files after a restart.
*   **Practical Assessment:** Create a utility that monitors a specific folder for changes and notifies the user.
*   **Completion Criteria:** App correctly handles restricted file system access and manages bookmarks.
*   **Next Module:** Phase 6: watchOS Development.
