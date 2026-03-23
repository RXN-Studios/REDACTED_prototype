# Engineering Breakdown

## 🔳 Raycasting Implementation
The core rendering loop utilizes a Digital Differential Analyzer (DDA) algorithm to calculate wall distances and textures in real-time. This provides a retro-3D perspective without the overhead of a full 3D engine.

## 🤖 AI State Machine
Enemies operate on a tiered logic system:
1. **Patrol:** Random movement within a predefined radius.
2. **Alert:** Triggered by Line-of-Sight (LoS) or sound; enemies begin tracking player coordinates.
3. **Attack:** Distance-based combat engagement with randomized cooldowns.

## 📉 Dynamic Scaling
The engine scales wall height and sprite size based on Z-buffer depth, ensuring that visual fidelity remains consistent even as the player moves at high speeds.
