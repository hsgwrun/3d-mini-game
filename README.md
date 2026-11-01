# DOWNHILL v2.0 — Urban Arcade Skateboarding

A browser-based 3D skateboard arcade game in development. The new direction is a fictional Japanese downtown with a visual style between realistic 3D and anime, comedic presentation, obstacles, ramps, tricks and combo scoring.

## Run locally

From the repository root:

```bash
python -m http.server 8000
```

Then open http://localhost:8000. Three.js is loaded from jsDelivr, so an internet connection is required.

## Controls

- W / Up Arrow: accelerate
- S / Down Arrow: brake
- A / Left Arrow and D / Right Arrow: steer
- Space: restart the run
- Camera button: cycle chase, wide and first-person views
- Touch devices: on-screen steering and throttle/brake controls

## Current prototype

- Three.js single-file browser prototype
- Existing procedural course and skateboard/rider model
- Timer, speed, local best time and camera selection
- Lobby with locally stored player name
- Online menu is a placeholder; no online service is connected

## DOWNHILL v2.0 roadmap

1. Phase 0: fix start position, course heading, board roll axis and lean direction.
2. Phase 1: arcade handling, jumping, landing and a three-mistake limit.
3. Phase 2: Japanese downtown course, buildings, obstacles and ramps.
4. Phase 3: tricks, grinds, combos and scoring.
5. Phase 4: comedic animations, reactions, audio and HUD polish.
6. Phase 5: additional courses, ghosts and secure online ranking.

## Status

Phase 0 foundation corrections have been applied in the current prototype. The new urban course, mistake system, ramps and trick gameplay are not implemented yet. Static source checks are not a substitute for browser playtesting. Online ranking and ghost sharing are not connected.
