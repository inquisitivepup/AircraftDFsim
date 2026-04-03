
# Aircraft Vectoring Simulator Mk1
**Lightweight, Browser-Based Tactical Training Environment for Airspace Control**

**Version:** 1.0.0 (Mk1)  
**Platform:** Web Browser (HTML5 / CSS3 / Vanilla JS)

---

##  Overview
The **Aircraft Vectoring Simulator Mk1** is a specialized, zero-risk training environment designed for Air Traffic Control (ATC) and Air Defense operators. Built entirely in-house, it bridges the gap between classroom theory and live-radar console operations. 

By utilizing a lightweight, browser-based architecture, the simulator eliminates the need for expensive, localized simulation software and operates seamlessly within secure, air-gapped military intranets. It focuses on the core fundamentals of vectoring, intercept geometry, standard rate turns, and Direction Finding (DF) homing.

##  Core Features
* **Zero-Install Deployment:** Runs locally in any modern web browser. No external servers, databases, or administrative privileges are required.
* **Dual-Monitor Architecture:** Features an isolated, distraction-free "Trainee Display" that synchronizes seamlessly with the "Instructor Console" via local browser storage.
* **Realistic Aircraft Profiles:** Accurate physics modeling for approach and cruise speeds across Fighter (350/250 kts), Transport (200/165 kts), and Helicopter (120/100 kts) profiles.
* **Dynamic Simulation Engine:** Supports standard rate turns, continuous holding turns, immediate manual overrides ("Fly Level"), and automatic speed reductions upon entering the approach sector.
* **Transient DF Homing:** Simulates real-world radio interactions by flashing homing bearings briefly, forcing trainees to rely on working memory and spatial awareness.
* **Post-Exercise AAR Plotter:** Automatically generates a comprehensive Flight Path Analysis plotting board upon exercise termination for data-driven tactical debriefs.
* **Adaptive "Glass Cockpit" UI:** Professional Slate (Light) and Dark modes to reduce eye strain in various operational lighting environments.

---

##  Installation & Setup
Because the simulator is 100% client-side, setup is instantaneous.
1. Visit https://inquisitivepup.github.io/AircraftDFsim/
2. Use FullScreen Mode
3. **For Dual-Monitor Operations:** * Move the main browser window to the Instructor's monitor.
   * Click **Launch Trainee Display**.
   * Drag the newly opened window to the Trainee's monitor and maximize it.

---

##  Operational Manual

### 1. Initialization
Upon launch, the Instructor will be prompted to select the interface theme and the **Aircraft Type**. This selection sets the underlying speed and physics profile for the target.
* Set the **Runway In Use** and **Spawn Distance**. 
* Access **Other Settings** for manual spawn bearings/headings if a specific intercept scenario is required.

### 2. Instructor Tools
* **Stopwatch:** A dedicated digital instrument for timing outbound legs, base turns, and standard rate intervals.
* **Quick Turn Grid:** Issue immediate heading changes.
  * *Specific Heading:* Enter a value (0-359) and click Turn.
  * *Continuous Turn:* Leave the input box **blank** and click Turn to simulate a continuous holding pattern.
  * *Fly Level:* Instantly halts any turn and establishes the aircraft on its current heading.

### 3. Trainee Interactions (Action Buttons)
* **Transmit for DF:** Calculates the bearing to the aircraft, converts it to a homing heading, and flashes it on the Trainee Display for 4 seconds to simulate a transient radio call.
* **Request Heading/Distance:** Outputs instantaneous target telemetry to the Instructor's single-line output display.

### 4. After Action Review (AAR)
Clicking **Terminate Exercise** halts the physics engine and automatically launches the Flight Path Analysis modal. 
* **Green Dot:** Initial spawn point.
* **Red Dot:** Point of exercise termination.
* **Dashed Line:** Runway final approach track for visual alignment confirmation.

---

## 🗺️ Future Roadmap (Mk2)
The following capabilities are slated for future development:
* **Environmental Variables:** Dynamic wind drift and automatic crosswind correction logic.
* **Complex Airspace:** Multi-target tracking for high-density deconfliction training.
* **Asymmetric Threat Profiles:** Addition of UAS/Drone target profiles for low-speed, low-RCS intercept and detection training within the approach direction.
* **Custom Airspace Boundaries:** Visual overlays for restricted zones and localized base airspace.

---
*Developed for internal tactical training purposes. Not for live operational Air Traffic Control use.*

***

Would you like to add a "Changelog" or "Version History" section to the README to track your future updates?
