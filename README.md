# Prompt_low - Simple Platformer Game

A minimal workspace for working with a local LLM (2/12B) to create an HTML game.

## Directory layout

- `prompts/` → Reusable prompts: system, task, corrections
- `contesto/` → Project rules and context injected into model input
- `gioco/` → Game files only: HTML page, JS/CSS scripts, assets
- `valutazioni/` → Manual tests, checklists and output comparisons
- `output/` → LLM-generated drafts needing human revision

## How to work with the model

1. Read `contesto/*.md` first — these contain project rules and must be injected as context/prompt input.
2. Pick a prompt from `prompts/`:
   - **system** → core behavior (keep this unchanged)
   - **task**    → specific work goal
   - **corrections** → fix previous output errors
3. Run the model locally with those prompts to generate drafts.
4. Review and revise every output in `output/` manually — the LLM is a suggestion engine, not an authority.

## Key principles

- Treat `contesto/` as executable truth; it overrides prose if they conflict.
- Never commit raw draft text from the model into the game folder (`gioco/`).
- Use `valutazioni/` to compare outputs and verify correctness before committing.

## Current Project: Simple Platformer

A simple HTML platformer with:
- Canvas API rendering
- Player movement (left/right + jump) with jump buffering for responsiveness
- Collision detection with solid and one-way platforms
- Multiple levels with win condition (reach the flag)
- Player animation (squash/stretch on jump/land)

The game is implemented in `output/platformer-v4.html` as a single HTML file.
Run it by opening the file in a browser or using a local server.

## Next steps (optional)

- Background decoration/particles
- Additional level variety (level 3 with obstacles/enemies)
- Score tracking (time, distance, etc.)