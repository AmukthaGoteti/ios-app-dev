# Platform Competency Matrix

This matrix serves as the definitive guide to the skills required across the Apple ecosystem. It helps learners identify where they can reuse knowledge and where they must specialize.

## 1. Core Engineering Layer (Shared Across All Platforms)
These skills are the "Baseline." You cannot effectively develop for any Apple platform without these.

| Skill | Description | Level Required | Relevance |
| :--- | :--- | :--- | :--- |
| **Swift Syntax** | Type safety, Optionals, Control Flow | Expert | All |
| **Modern Concurrency** | async/await, Actors, Sendable | Expert | All |
| **ARC & Memory** | Strong/Weak/Unowned, Retain Cycles | Proficient | All |
| **SwiftUI Basics** | Stacks, State, Bindings, Modifiers | Expert | All |
| **Observation** | `@Observable` macro, data-driven UI | Proficient | All |
| **Xcode Workflow** | Build Settings, LLDB, Instruments | Proficient | All |
| **SwiftData** | Model definitions, Queries, Persistence | Proficient | All |
| **Networking** | URLSession, Codable, API Design | Proficient | All |
| **Swift Testing** | Unit Tests, Mocking, TDD | Proficient | All |

---

## 2. Platform Specialization Layer
These skills are specific to the unique hardware and UX patterns of each platform.

### iOS & iPadOS (The Mobile Standard)
| Skill | Description | Level Required | Focus |
| :--- | :--- | :--- | :--- |
| **App Lifecycle** | ScenePhase, Backgrounding, Restoration | Proficient | Lifecycle |
| **UIKit Interop** | `UIViewRepresentable`, Coordinators | Proficient | UI |
| **System Integration** | Widgets, Live Activities, App Intents | Proficient | Ecosystem |
| **Hardware APIs** | Camera, Photos, CoreLocation | Proficient | Device |
| **Adaptive Layout** | Size Classes, Multitasking (iPad) | Expert | UX |

### macOS (The Power User Experience)
| Skill | Description | Level Required | Focus |
| :--- | :--- | :--- | :--- |
| **AppKit Interop** | `NSViewRepresentable`, AppKit APIs | Proficient | UI |
| **Windowing** | Multi-window, Menu Bar, Toolbars | Expert | UX |
| **File System** | Security-Scoped Bookmarks, Sandbox | Expert | System |
| **Desktop UX** | Keyboard Shortcuts, Pointer Interaction | Proficient | UX |
| **Notarization** | Developer ID signing, Hardened Runtime | Proficient | Distribution |

### watchOS (The Glanceable Experience)
| Skill | Description | Level Required | Focus |
| :--- | :--- | :--- | :--- |
| **Complications** | WidgetKit for Watch Faces | Expert | Ecosystem |
| **Watch Connectivity** | `WCSession`, iPhone-Watch Sync | Proficient | Connectivity |
| **HealthKit** | Heart Rate, Workout Sessions, Privacy | Proficient | Device |
| **Crown Input** | Digital Crown integration | Proficient | UX |
| **Power Mgmt** | Background refresh, Battery efficiency | Expert | System |

### visionOS (The Spatial Experience)
| Skill | Description | Level Required | Focus |
| :--- | :--- | :--- | :--- |
| **Spatial UI** | Windows, Volumes, Immersive Spaces | Expert | UX |
| **RealityKit** | Entities, Components, Systems (ECS) | Expert | 3D |
| **3D Asset Pipeline** | USDZ, Reality Composer Pro | Proficient | Assets |
| **Gaze & Pinch** | Spatial interaction patterns | Expert | UX |
| **Spatial Audio** | 3D sound positioning | Proficient | Device |

---

## 3. Competency Progression Path

1.  **Foundational:** Can build a basic app on one platform using tutorials.
2.  **Proficient:** Can implement custom features, handle concurrency, and use persistence without guidance.
3.  **Expert:** Can architect a multi-platform system, optimize performance with Instruments, and design for accessibility/internationalization.
