# Wayfinder Map: Simple Platformer Game (v1)

## Destination

A playable HTML platformer with basic mechanics: player movement (left/right + jump), collision detection, multiple levels, and a simple win condition.

## Notes

- Canvas API for rendering
- Class-based level definition
- Vanilla JavaScript - no frameworks
- Browser-only deployment
- 1-2 levels initially

## Decisions so far

- **Rendering engine**: [Canvas API](link): Chosen over DOM-based for performance and full control. Decision made on session #0.

## Not yet specified

1. Player class design (physics, state machine, input handling)
2. Platform/level entity classes
3. Collision detection algorithm
4. Input system (keyboard vs touch/mouse)
5. Win condition implementation (flag at end of level?)
6. Game loop structure (requestAnimationFrame vs setTimeout)

## Out of scope

- Sound effects, music
- Multiplayer
- Save/load system
- Complex animations
- Particle effects
- Level editor tool
