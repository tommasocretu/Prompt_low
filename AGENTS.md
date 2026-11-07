# Working in Prompt_low

This workspace is designed for local LLM (2/12B) coding of an HTML game. The directory structure is intentionally minimal — follow it to avoid confusion.

## Directory layout (per README.md)

- `prompts/` → Reusable prompts: system, task, corrections
- `contesto/` → Project rules and context injected into model input
- `gioco/`   → Game files only: HTML page, JS/CSS scripts, assets
- `valutazioni/` → Manual tests, checklists, output comparisons
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
