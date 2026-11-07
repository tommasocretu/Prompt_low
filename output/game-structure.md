# Ticket: Core Game Structure

## Question

Design the main game architecture for a simple HTML platformer using Canvas API. The structure should include:

1. **Game class** - manages the main loop, state machine (menu → playing → level complete), and level loading
2. **Player class** - handles movement, physics (gravity, velocity, jumping), input handling, collision detection
3. **Level class** - defines platforms, obstacles, player spawn point, win flag position
4. **Input handler** - keyboard events mapped to action states

### Technical constraints:
- Single HTML file architecture (no build step)
- Vanilla JavaScript only
- Canvas API for rendering
- Class-based level definition
- Browser-only
