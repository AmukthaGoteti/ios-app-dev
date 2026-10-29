## Phase 6: watchOS Development
**Objective:** Designing for "glanceable" interactions on the wrist.

### Module 6.1: watchOS Architecture & UI
*   **Difficulty:** Intermediate
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Phase 3
*   **Learning Outcomes:** Creating high-impact, low-friction interfaces for a tiny screen.
*   **Syllabus:**
    *   Watch-specific Layouts: Vertical paging and the Digital Crown.
    *   The "Glance" Mindset: Designing for 2-second interactions.
    *   Navigation: Simple stacks and the "Back" button.
    *   The Digital Crown: Using `digitalCrownRotation` for input.
*   **Core Concepts:**
    *   *Information Density:* Balancing the need for data with the physical limits of the screen.
    *   *Haptics:* Using the Taptic Engine to provide non-visual feedback.
*   **Guided Exercise:** Build a "Pomodoro Timer" that uses the Digital Crown to set the duration.
*   **Independent Assignment:** Create a "Health Dashboard" that displays 3 key metrics in a compact, readable grid.
*   **Common Mistakes:** Trying to put too much text on a screen; neglecting the "crown" for scrolling long lists.
*   **Practical Assessment:** Design a screen that passes a "Glance Test" (information is understood within 3 seconds).
*   **Completion Criteria:** UI is responsive and utilizes the Digital Crown correctly.
*   **Next Module:** 6.2 Complications & Connectivity.

### Module 6.2: Complications & Connectivity
*   **Difficulty:** Advanced
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Module 6.1
*   **Learning Outcomes:** Integrating the watch app into the watch face and the iPhone ecosystem.
*   **Syllabus:**
    *   WidgetKit for watchOS: Creating complications for various watch face styles.
    *   Watch Connectivity: `WCSession` for sending data between iPhone and Watch.
    *   Independent vs. Companion Apps: Understanding the deployment models.
    *   Background Refresh: Updating complication data efficiently.
*   **Core Concepts:**
    *   *The Timeline:* How the watch predicts what the complication should show for the next 24 hours.
    *   *Session States:* Managing the connection state (reachable vs. unreachable).
*   **Guided Exercise:** Build a complication that shows the current temperature, updated via the iPhone app.
*   **Independent Assignment:** Implement a "Remote Control" app where a button on the watch triggers an action on the iPhone (e.g., taking a photo).
*   **Common Mistakes:** Attempting to send large files over `WCSession`; ignoring battery constraints for background updates.
*   **Practical Assessment:** A complication that updates correctly in the background without draining the battery.
*   **Completion Criteria:** Successful data transfer between iOS and watchOS; complication renders on a real watch face.
*   **Next Module:** Phase 7: visionOS and Spatial Computing.

---

## Phase 7: visionOS and Spatial Computing
**Objective:** Transitioning from 2D screens to immersive 3D experiences.

### Module 7.1: Spatial UI & Windows
*   **Difficulty:** Intermediate
*   **Duration:** 1 Week (15 hours)
*   **Prerequisites:** Phase 3
*   **Learning Outcomes:** Designing interfaces that exist in the user's physical room.
*   **Syllabus:**
    *   The visionOS Environment: Windows, Volumes, and Immersive Spaces.
    *   Spatial Layout: Using `ZStack` for depth and `RealityView` for 3D content.
    *   Interaction: Gaze-and-Pinch, Hand Gestures, and Keyboard/Mouse support.
    *   Glassmorphism: Understanding the system materials and lighting.
*   **Core Concepts:**
    *   *The Z-Axis:* Adding depth to UI elements.
    *   *Ornaments:* Placing controls around the edge of a window to maximize content space.
*   **Guided Exercise:** Create a "Spatial Gallery" window that displays a grid of 3D images.
*   **Independent Assignment:** Build an "Immersive Space" that changes the user's environment to a stylized 3D room.
*   **Common Mistakes:** Placing UI too close to the user (causing discomfort); ignoring the "Safe Zone" for gaze interaction.
*   **Practical Assessment:** A windowed app that correctly utilizes "Ornaments" for primary navigation.
*   **Completion Criteria:** App runs in the visionOS simulator/device with fluid gaze-based interaction.
*   **Next Module:** 7.2 RealityKit & 3D Content.

### Module 7.2: RealityKit & 3D Content
*   **Difficulty:** Advanced
*   **Duration:** 2 Weeks (25 hours)
*   **Prerequisites:** Module 7.1
*   **Learning Outcomes:** Creating interactive, physics-based 3D experiences.
*   **Syllabus:**
    *   RealityKit Entities: Components, Systems, and Scenes.
    *   Materials & Lighting: PBR (Physically Based Rendering) and environmental lighting.
    *   Reality Composer Pro: Preparing USDZ assets and creating prototypes.
    *   Physics & Collisions: Making objects interact with each other.
    *   Spatial Audio: Positioning sound in 3D space for immersion.
*   **Core Concepts:**
    *   *The Entity-Component-System (ECS):* How RealityKit manages 3D objects efficiently.
    *   *USDZ:* The industry standard for 3D assets on Apple platforms.
*   **Guided Exercise:** Create a "Virtual Pet" that follows the user's gaze and reacts to a pinch gesture.
*   **Independent Assignment:** Build an "Interactive Solar System" where users can click planets to see info and orbit them in 3D.
*   **Common Mistakes:** Using too many high-poly models (killing performance); failing to set up correct collision shapes.
*   **Practical Assessment:** A spatial app where a 3D object is placed on a real-world table and interacts with the environment.
*   **Completion Criteria:** Stable 90 FPS performance with interactive 3D entities.
*   **Next Module:** Phase 8: Shared Services.
