<div align="center">
  <h1>🚁 AC-130 Gunship: Close Air Support Sim-Game</h1>
  <p><b>Advanced Targeting, Thermal Imaging & Dynamic Destruction Framework</b></p>
  <img src="https://img.shields.io/badge/Unity-6%20LTS-black?style=for-the-badge&logo=unity" alt="Unity 6"/>
  <img src="https://img.shields.io/badge/Language-C%23-blue?style=for-the-badge&logo=c-sharp" alt="C#"/>
  <img src="https://img.shields.io/badge/Graphics-Custom_Shaders-success?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Physics-Dynamic_Deformation-critical?style=for-the-badge"/>
</div>

---

## 📖 About the Project

This Game is a highly technical Close Air Support e.g(AC-130) simulation-like game built to showcase advanced camera systems, custom shader development, and dynamic physics in Unity. 

By abstracting complex flight dynamics into an automated orbit system, the project shifts its focus entirely to the intricacies of aerial gunnery. Players operate high-tech targeting pods, manage multi-caliber weapon systems, and utilize custom Forward-Looking Infrared (FLIR) shaders to engage AI-driven ground threats in a dynamic battlefield.

---

## 🎬 Gameplay Showcase

<p align="center">
  <a href="https://www.youtube.com/shorts/JPgVjzYVN84" target="_blank">
    <img src="https://img.youtube.com/vi/JPgVjzYVN84/maxresdefault.jpg" alt="AC-130 Gunship Sim Gameplay" width="600">
  </a>
</p>
<p align="center"><i>Click the image to watch the full gameplay on YouTube</i></p>

---

## ✨ Core Technical Features

*   **Automated Orbit & Flight Mechanics:** The aircraft maintains a mathematically stable automated orbit around the target vector, allowing the system to dedicate CPU cycles to ground-level physics and AI calculations rather than complex flight surface physics.
*   **Custom Thermal Imaging (FLIR):** Developed a specialized post-processing pipeline for thermal rendering. The system dynamically reads the heat signatures of targeted objects, enabling both Black Hot and White Hot spectrums for realistic night-vision engagements.
*   **Dynamic Terrain & Destruction:** Implemented real-time mesh topology modification upon ballistic impacts, creating permanent craters. This is seamlessly coupled with pre-fractured asset systems for performance-friendly, satisfying structural collapses.
*   **Avionics & HUD Engineering:** Engineered a military-grade user interface that tracks crosshair telemetry, manages active target locks, and monitors internal system health status.
*   **AI Threat Management:** The ground environment is populated by state-driven AI logic, featuring active infantry, dynamic patrol routes, and a layered radio chatter system for an immersive combat audio soundscape.

---

## 📸 Visual Showcase


| Targeting & Avionics (HUD) | Thermal Vision (FLIR) |
| :---: | :---: |
| <img src="Images/tracking.png" width="400"><br><i>Gimbal tracking and weapon telemetry.</i> | <img src="Images/Blckir.png" width="400"><br><i>White Hot / Black Hot dynamic heat detection.</i> |

| Dynamic Destruction | Heat Bar |
| :---: | :---: |
| <img src="Images/destruckiton.png" width="400"><br><i>Real-time terrain deformation with Mesh Deformation.</i> | <img src="Images/GunHeat.png" width="400"><br><i>25mm Heat Bar for Game Balance.</i> |

---


## 🔬 Developer Notes & Architecture

Developing a realistic targeting pod simulation required strict optimization, especially concerning rendering and physics calculations:
*   **Shader Optimization:** The thermal vision is not merely a color filter; it actively isolates objects tagged with specific heat emission layers, ensuring that the shader only processes relevant pixels, saving GPU bandwidth.
*   **Performance-Friendly Deformation:** Real-time terrain deformation can cause heavy CPU spikes. The terrain modification system utilizes localized mesh updating techniques to ensure that altering the geometry at the point of impact does not cause frame drops, even during heavy 105mm artillery bombardment.

---
## Copyright & License

**Copyright (c) 2026 Emir Bekar. All rights reserved.**

This repository is public strictly for portfolio and demonstration purposes. 
The source code, 3D assets, custom shaders, and all related materials may not be copied, distributed, modified, or used for any commercial or non-commercial purposes without explicit written permission.
