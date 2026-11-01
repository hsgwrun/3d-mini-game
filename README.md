# DOWNHILL — Touge Time Attack

A browser-based 3D downhill skateboard time-attack prototype set on a fictional Japanese mountain pass.

## Play locally
Run a static server from the repository root:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000. The game loads Three.js from jsDelivr, so an internet connection is required.

## Controls
- W / Up Arrow: accelerate
- S / Down Arrow: brake
- A / Left Arrow and D / Right Arrow: steer
- Space: restart the run
- Camera button: cycle chase, wide, and first-person views
- Touch devices: on-screen steering and throttle/brake controls

## Included in this prototype
- Procedural mountain-pass scenery and road
- Arcade-style downhill skateboard movement
- Timer, speed display, and local personal best
- Restart and selectable camera views
- Responsive desktop/mobile layout

## Roadmap
- Improve rider and skateboard animation
- Add proper checkpoints and course progression
- Add deterministic ghost replay
- Add more courses and visual polish
- Add online leaderboard only with a trusted backend that validates runs server-side and rate-limits submissions

## Notes
This is an early prototype. Physics, course visuals, collision handling, and ghost replay are still being developed. Online leaderboard is not connected yet.
