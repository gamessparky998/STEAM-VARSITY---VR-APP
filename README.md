# STEAM-VARSITY - Interactive 3D Exploded-View Machinery WebXR Laboratory

A high-tech, interactive WebXR virtual training and engineering inspection laboratory built in **A-Frame**. Users can explore heavy industrial machinery, inspect internal sub-assemblies (pumps, impellers, motors, hydraulic manifolds, engines, and titanium pressure hulls) in real time with continuous 0–100% exploded-view cutaways, proximity-triggered disassembly, and 3D technical callout annotations.

---

## 🚀 Features

- **500HP Industrial Centrifugal Pump & Drive Motor**:
  - Volute casing cutaway with fluid flow redirection.
  - Dynamically rotating CNC-machined bronze impeller with backward-curved vanes (1750 RPM).
  - Hardened steel drive shaft with dual mechanical seal packs.
  - 500 HP induction motor with copper stator windings and laminated rotor core.
  - Invisible interactive hitboxes (`opacity="0"`) updating live `#info-panel` technical specs.
- **Triton Deep-Sea Submersible**:
  - Lateral hull fairing expansion revealing the Grade-5 Titanium Pressure Sphere.
  - Solid-state Lithium-ion battery power banks (120 kWh).
  - Twin 25 kW brushless DC vector propulsion thrusters.
- **JCB Heavy Excavator Powertrain**:
  - Operator cabin and hood separation revealing the 4.8L Turbocharged Diesel Engine Block.
  - Dual axial piston hydraulic pumps delivering 350 bar (5,075 PSI).
  - Multi-spool hydraulic control valve manifolds.
- **WebXR & Meta Quest 3S Support**:
  - Gaze and laser raycaster pointing and hover interactions.
  - Teleportation locomotion and snap turning.
  - Desktop keyboard and mouse fallback.
- **Procedural Web Audio Engine**:
  - Zero external `.mp3`/`.wav` assets. Synthesizes mechanical servo disassembly whines and component scanning tones in real time via Web Audio API.

---

## 🛠️ How to Run

1. Open `index.html` directly in any WebGL/WebXR-compatible browser, or host with a local static HTTP server:
   ```bash
   npx http-server -p 8080 .
   ```
2. Navigate to `http://localhost:8080/index.html`.
3. In Meta Quest 3S, click the **VR** button in the lower right corner to enter immersive virtual reality.

---

## 🎮 Controls

- **Desktop**:
  - `W` `A` `S` `D`: Move camera
  - `Mouse`: Look around and hover/click parts
  - `Space`: Toggle 0% / 100% Exploded View
  - `1`: Jump to Centrifugal Pump Station
  - `2`: Jump to JCB Excavator Station
  - `3`: Jump to Triton Submersible Station
  - `0`: Central Laboratory Overview
  - `H`: Toggle Operating Guide Modal
- **VR (Meta Quest 3S)**:
  - `Trigger`: Select / interact with 3D buttons and parts
  - `Thumbstick`: Teleport locomotion and snap turning
  - `Proximity`: Walking near any machine automatically initiates its exploded-view animation!
