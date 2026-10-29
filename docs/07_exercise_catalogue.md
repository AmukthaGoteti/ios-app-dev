# Hands-on Exercise Catalogue: Apple Ecosystem Engineering

This catalogue provides a structured set of coding exercises to reinforce the theoretical knowledge from the Master Syllabus. Exercises are categorized by difficulty and linked to specific phases.

## Phase 0: Foundations
### Level: Beginner
*   **EX-0.1: The Algorithm Architect:** Write a pseudocode algorithm for a "Smart Coffee Machine" that handles different bean types and water levels.
*   **EX-0.2: Logic Gate Simulator:** Create a simple truth table for a "Home Security System" (If Sensor A OR Sensor B is triggered AND System is Armed $\rightarrow$ Alarm).
*   **EX-0.3: The Contact Manager (Pseudo):** Implement a mock data structure in pseudocode for a contact list with Search and Delete functionality.
*   **EX-0.4: Git Branching Challenge:** Create a repository, branch a "feature/ui-update", commit changes, and merge it back to main while resolving a simulated conflict.

## Phase 1: Swift Programming
### Level: Beginner to Intermediate
*   **EX-1.1: The Safe Parser:** Write a function that takes a `String?` and returns a `Bool`, safely unwrapping the string to check if it contains a specific keyword.
*   **EX-1.2: Grade Book Logic:** Create a system that calculates an average of `[Double?]` grades, ignoring the `nil` values.
*   **EX-1.3: The State-Machine Enum:** Build a `GameCharacterState` enum with associated values for `attacking(power: Int)` and `healing(amount: Int)`.
*   **EX-1.4: Value vs Reference Test:** Create a Struct and a Class with the same properties; pass both to a function that modifies them, and print the results to prove the difference.

### Level: Advanced
*   **EX-1.5: The Protocol-Based Drawer:** Define a `Drawable` protocol. Implement it for `Circle` and `Square`. Create a function that takes `[any Drawable]` and "renders" them to the console.
*   **EX-1.6: Generic Data Store:** Build a `Storage<T: Codable>` class that can save any Codable object to a local file.
*   **EX-1.7: The Leak Hunter:** Write a class with a closure that captures `self` strongly. Use the Xcode Memory Graph to prove the leak, then fix it using `[weak self]`.
*   **EX-1.8: Async Image Fetcher:** Use `async/await` to fetch three images from different URLs concurrently using a `TaskGroup`.
*   **EX-1.9: The Actor Cache:** Create a `ThreadSafeCache` actor that stores key-value pairs and prevents data races.

## Phase 2 & 3: Xcode & SwiftUI
### Level: Intermediate
*   **EX-2.1: Scheme Switcher:** Configure an app to use two different `Info.plist` values based on whether the "Dev" or "Prod" scheme is selected.
*   **EX-3.1: Layout Challenge:** Build a "Profile Page" using only `VStack`, `HStack`, and `Spacer` that looks identical on iPhone and iPad.
*   **EX-3.2: The Observable Store:** Create a `@Observable` class for a "Todo List" and bind it to a SwiftUI `List` and a `TextField`.
*   **EX-3.3: Programmatic Navigator:** Implement a `NavigationPath` that allows the app to "Jump" to the third screen in a stack from a home button.
*   **EX-3.4: Physics-Based Animation:** Create a button that "pops" and "bounces" using a `.spring()` animation when pressed.
*   **EX-3.5: VoiceOver Audit:** Add accessibility labels and hints to a complex form and verify it with the Accessibility Inspector.

## Phase 4-7: Platform Specialization
### Level: Intermediate to Advanced
*   **EX-4.1: Lifecycle Guard:** Implement a system that saves the app state to `UserDefaults` exactly when the app enters the `.background` scene phase.
*   **EX-4.2: UIKit Bridge:** Wrap a `UITextView` in `UIViewRepresentable` to implement a custom "Mention" system (@user) in SwiftUI.
*   **EX-5.1: Menu Bar Utility:** Build a macOS app that lives only in the menu bar and shows the current CPU usage.
*   **EX-5.2: Sandbox File Picker:** Use `NSOpenPanel` to let a user pick a file and then save a `Security-Scoped Bookmark` to access it after a restart.
*   **EX-6.1: Digital Crown Scroller:** Create a watchOS view where the Digital Crown adjusts the opacity of an image.
*   **EX-6.2: WCSession Sync:** Send a "Ping" from the Watch to the iPhone and receive a "Pong" response in under 1 second.
*   **EX-7.1: Spatial Window:** Create a visionOS window that uses an "Ornament" to switch between 2D and 3D modes.
*   **EX-7.2: RealityKit Entity:** Spawn a 3D cube in a `RealityView` that changes color when the user pinches it.

## Phase 8-11: Engineering & Distribution
### Level: Advanced
*   **EX-8.1: The Generic API Client:** Build a `NetworkClient<T: Decodable>` that handles all HTTP methods and returns a `Result<T, NetworkError>`.
*   **EX-8.2: CloudKit Sync:** Implement a "Shared Note" where changes made on one device appear on another within 5 seconds.
*   **EX-9.1: TDD Component:** Use the Swift Testing framework to build a "Currency Converter" logic, writing the tests before the implementation.
*   **EX-9.2: Mocking Service:** Create a `MockNetworkService` that conforms to the same protocol as the real one, allowing UI tests to run without an internet connection.
*   **EX-10.1: MVVM Refactor:** Take a "Massive View" and move all logic into a `ViewModel` and all data into a `Model` struct.
*   **EX-10.2: SPM Modularization:** Split a project into `Core`, `UI`, and `App` modules using local Swift Packages.
*   **EX-11.1: IAP Flow:** Implement a "Pro" upgrade using StoreKit 2 with a successful "Purchase $\rightarrow$ Entitlement" flow.
