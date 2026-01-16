**Welcome to Firefly Rumble!!**

Created by Michael Pettric and Michael Brandmeyer

Video Demo: https://youtu.be/RERmVnLnOac

**Game Description**

Firefly Rumble is a fast-paced, browser-based 2D action game built with JavaScript and HTML5 Canvas. Players control a character tasked with collecting elusive fireflies while avoiding increasingly aggressive enemies. As levels progress, the screen fills with dynamic movement, projectile combat, and emergent AI behavior, creating a chaotic and replayable experience.

The core challenge comes from balancing movement, positioning, and timing while navigating swarming enemies and escalating difficulty. Each level introduces more fireflies, faster enemies, and new threats. This includes periodic boss encounters, which push the player to adapt and survive.

**Technical Overview**

Firefly Rumble was built from the ground up using vanilla JavaScript, with no external game engines. The project focuses heavily on game systems, AI behavior, and real-time simulation, all rendered through the HTML5 Canvas API.

Key Systems & Features
- Custom Game Loop
- - Fixed-timestep rendering targeting high FPS
- - Manual delta-time management for smooth animation and movement
- - Explicit state handling for menus, gameplay, level transitions, and game over
- Sprite & Animation System
- - JSON-driven animation data for all entities
- - Frame-based sprite animations with directional states
- - Shared rendering pipeline for players, enemies, projectiles, and collectibles
- Player Mechanics
- - Keyboard-based movement with collision constraints
- - Mouse-aimed projectile combat
- - Ammo regeneration with cooldown logic to prevent spam abuse
- Enemy AI
- - Spider enemies that track and chase the player using directional movement logic
- - Ant enemies that switch behavior based on screen visibility
- - Boss enemies with higher health pools and persistent pursuit behavior
- Boids / Flocking AI
- - Fireflies and ants use classic Boids algorithms:
- - - Alignment
- - - Cohesion
- - - Separation
- - Emergent swarm behavior creates organic movement patterns and dynamic difficulty
- - Acceleration-based steering with velocity clamping for stability
- Collision Detection
- - Axis-aligned bounding box (AABB) collision checks
- - Differentiated collision responses for:
- - - Player <> enemies
- - - Projectiles <> enemies
- - - Player <> collectibles
- Progression & Difficulty Scaling
- - Procedural level scaling:
- - - Increased enemy count
- - - Faster movement speeds
- - - Periodic boss spawns
- - Randomized backgrounds per level for visual variety

**Collaboration**

The project was built through iterative collaboration, with shared responsibility over design decisions, debugging, and gameplay balance. This teamwork emphasized clear communication, modular code structure, and rapid experimentation.