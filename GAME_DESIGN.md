# DOWNHILL v2.0 — Game Design

## Vision
A browser-based 3D arcade skateboard game set in a fictional Japanese downtown entertainment district. The visual style balances grounded urban detail with anime-like color and expressive comedy. Fun, readable gameplay takes priority over strict realism.

## Core decisions
- Setting: Japanese繁華街 (busy shopping and entertainment streets), fictionalized.
- Visual direction: a midpoint between realistic 3D and anime/stylized art.
- Handling: responsive arcade physics with a hybrid weight-shift and steering model.
- Mist allowance: 3 mistakes per run; the third mistake ends the run.
- Tone: comedic crashes, expressive reactions, playful props and visual gags.
- Core loop: avoid obstacles, use ramps, perform tricks, chain combos, reach the finish, improve score and time.
- Single-player first. Online ranking and ghost sharing remain future features until a trusted backend exists.

## Gameplay
- Keyboard: WASD / arrow keys; touch controls on supported devices.
- Acceleration, braking, steering, controlled drift, jumping and landing.
- Tricks: ollie, aerial tricks, grind and combo scoring.
- Obstacles: traffic cones, cardboard boxes, construction barriers, signs and moving hazards.
- Ramps: standard, large, chained and trick-focused ramps.
- Mistakes include obstacle collisions, failed landings and leaving the course. A mistake counter allows three mistakes.
- Recovery after a mistake should return the rider to a safe, nearby course position with a brief comedic reaction.

## Course direction
1. Shopping street: introduce steering and basic obstacle avoidance.
2. Construction zone: ramps, barriers and alternate lines.
3. Office / entertainment district: rails, larger jumps and advanced combo opportunities.

## Phase 0 — Foundation fixes
- Align the start position with the course centerline and forward tangent.
- Use one consistent heading convention for movement and visual orientation.
- Apply board roll around the board's longitudinal local axis, matching the steering/lean direction.
- Keep rider pose and board pose synchronized.
- Validate statically before moving to new course content.

## Implementation roadmap
1. **Phase 0 — Foundation fixes:** start alignment, board lean direction, camera and ground alignment.
2. **Phase 1 — Arcade physics:** responsive steering, inertia, drift, jump/air/landing states and three-mistake system.
3. **Phase 2 — Urban course:** fictional Japanese downtown streets, buildings, sidewalks, street props, obstacles and ramps.
4. **Phase 3 — Tricks:** ollie, aerial tricks, grind, landing checks, combos and score multipliers.
5. **Phase 4 — Presentation:** comedic crash/reaction animations, NPC reactions, sound, music, HUD and results.
6. **Phase 5 — Expansion:** more courses, difficulty settings, deterministic ghosts and online features.

## Technical and safety notes
- Three.js browser prototype; keep privileged secrets out of client code.
- Online features are not connected. Never imply otherwise.
- Any future online leaderboard must validate runs server-side and rate-limit submissions.
- Local name and record data may be lost when browser storage is cleared or on another device.
