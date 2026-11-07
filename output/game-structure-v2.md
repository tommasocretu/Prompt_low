# Ticket: Refine Collision Detection & Add Game Polish

## Question

The basic collision system works, but we should refine it for better gameplay feel. Decisions needed:

1. **Collision response**: Should platforms have different properties (solid vs one-way)? Currently everything is solid.
2. **Jump buffering**: When a player jumps slightly after stepping off a platform edge, should they still jump? This makes the game feel more responsive.
3. **Air control**: Can the player change horizontal direction while in the air? Currently yes, but we could limit this to make physics feel tighter.
4. **Visual feedback**: Add subtle effects like:
   - Player squash/stretch when jumping or landing
   - Particle effect on flag reach
   - Screen shake on collision with walls

## Constraints
- Keep performance high (no heavy calculations)
- Maintain single HTML file architecture
- Canvas API only
