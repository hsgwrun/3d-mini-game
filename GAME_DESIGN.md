# DOWNHILL — Game Design

## Concept
A browser-based 3D downhill skateboard time-attack game set on a fictional Japanese mountain pass, with realistic anime-inspired visuals.

## Core gameplay
- Ride a skateboard downhill and reach the finish as quickly as possible.
- Arcade-leaning handling: approachable steering, acceleration, braking, and carving.
- Start with one complete course; design the course system so more routes can be added later.
- Keyboard controls: WASD and arrow keys.
- Camera selection: multiple camera views, including chase and first-person options.

## Time attack and records
- Save a local personal best.
- Record runs for a local ghost replay.
- Add an online leaderboard for global competition.
- Treat online leaderboard scores as untrusted input: validate times server-side, rate-limit submissions, and never trust client-submitted scores.

## Visual direction
- Realistic anime-inspired art direction.
- Japanese mountain pass with hairpin turns, guardrails, road markings, trees, rocks, and distant scenery.
- Clear HUD for timer, speed, checkpoint progress, and restart.

## Technical direction
- Browser game, responsive for desktop and mobile.
- Three.js for 3D rendering.
- Keep gameplay and course data separate from rendering code.
- Build a playable single-player prototype first. Add persistent online rankings after the core driving loop is stable.
- Never embed privileged database or API secrets in client-side code.

## Initial milestones
1. Create the 3D scene and a downhill course.
2. Add a controllable skateboarder and arcade downhill physics.
3. Add checkpoints, finish line, timer, and restart.
4. Add camera selection and local best-time persistence.
5. Add local ghost replay.
6. Design and implement a secure online leaderboard backend.
