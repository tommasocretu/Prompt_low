# Wayfinder Map: Simple Platformer (v3)

## Destination

A playable HTML platformer with basic mechanics: player movement (left/right + jump), collision detection, multiple levels, and a simple win condition.

## Notes

- Canvas API for rendering
- Class-based level definition
- Vanilla JavaScript only
- Browser-only deployment
- Jump buffering implemented (ticket resolved)
- One-way platforms added (ticket resolved)

## Decisions so far

- **Rendering engine**: [Canvas API](link): Chosen over DOM-based for performance and full control. Decision made on session #0.
- **Game loop structure**: [Single phase (update+draw)](link): Using requestAnimationFrame with combined update and render phases.
- **Jump buffering**: [Implemented](link): Player can jump if they were grounded within 150ms of stepping off a platform. Makes game feel much more responsive. Decision made on session #1.
- **One-way platforms**: [Implemented](link): Orange platforms you can stand on top but fall through from below. Decision made on session #2.

## Not yet specified

3. Player animation (squash/stretch on jump/land)
4. Input smoothing for movement
5. Particle effects on flag reach
6. Background decoration/particles
7. Additional level variety
8. Score tracking (time, distance, etc.)
9. Camera scrolling for wider levels

## Out of scope

- Sound effects, music
- Multiplayer
- Save/load system
- Complex animations
- Particle effects
- Level editor tool
