# 🐍 Rogue-Snake: Roguelite Web Game

A modern, roguelite twist on the classic arcade game[cite: 6]. The game challenges players to survive on a grid while strategically choosing from a pool of 13 unique modifiers (perks) upon leveling up[cite: 6]. 

This Minimum Viable Product (MVP) was developed strictly with native web technologies (HTML5, CSS3, JavaScript ES6) and the `<canvas>` API, completely eliminating the overhead of external game engines or frameworks[cite: 6].

## 🚀 Key Engineering & Architecture Features

* **Finite State Machine (FSM):** The core logic is built upon a robust FSM, cleanly handling transitions between rendering the 2D physics loop, asynchronous UI interactions (like selecting perks), and kinetic death animations[cite: 6, 7].
* **Input Buffering System:** Implemented a First-In-First-Out (FIFO) queue for player inputs to prevent overlapping commands in grid-based movement, completely eliminating the common issue of instantaneous self-collisions[cite: 6, 7].
* **Procedural Generative Audio:** The project completely abandons static audio files (MP3/WAV)[cite: 6]. Instead, all sound effects and dynamic background music are synthesized in real-time using the native browser `AudioContext` (Web Audio API)[cite: 6, 7].
* **No-Collider Grid Logic:** Collision detection bypasses heavy physics engines by strictly iterating over a mathematical coordinate grid, cross-referencing the snake's segments against walls and AI-controlled enemy nodes[cite: 6].
* **Persistent Meta-Progression:** Integrates browser `localStorage` to save the player's in-game currency across sessions, powering a frictionless UI shop where users can unlock various aesthetic skins[cite: 6, 7].

## 🕹️ Gameplay Mechanics
* **Dynamic AI Enemies:** Features autonomous red snakes with specific movement logic, artificial vision nerfs, and turn-skipping constraints to balance the difficulty[cite: 6, 7].
* **Combo System:** Fast-paced apple gathering activates a visual and auditory score multiplier[cite: 6].
* **Randomized Loot Goblins:** Includes a rare "Mouse" spawn mechanic that freezes the game state and opens a dedicated roulette UI for legendary-tier rewards[cite: 6].
