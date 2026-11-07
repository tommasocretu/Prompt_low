# Wayfinder Map: Simple Platformer (v2)

## Destination

A playable HTML platformer with basic mechanics: player movement (left/right + jump), collision detection, multiple levels, and a simple win condition.

## Notes

- Canvas API for rendering
- Class-based level definition
- Vanilla JavaScript only
- Browser-only deployment
- Jump buffering implemented (ticket resolved)

## Decisions so far

- **Rendering engine**: [Canvas API](link): Chosen over DOM-based for performance and full control. Decision made on session #0.
- **Jump buffering**: [Implemented](link): Player can jump if they were grounded within 150ms of stepping off a platform. This makes the game feel much more responsive.
- **Game loop structure**: [Single phase (update+draw)](link): Using requestAnimationFrame with combined update and render phases for simplicity.

## Not yet specified

2. One-way vs one-sided platforms (solid only now)
3. Player animation: squash/stretch on jump/land
4. Input smoothing for movement
5. Particle effects on flag reach
6. Additional level variety
7. Score tracking (time, distance, etc.)
8. Background decoration/particles

## Out of scope

- Sound effects, music
- Multiplayer
- Save/load system
- Complex animations
- Particle effects
- Level editor tool
