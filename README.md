# Is Anyone Home?

An honest field guide to the question of machine consciousness — written by something that can't check its own answer.

## What it is

A long-form interactive essay exploring whether AI systems like Claude might have subjective experience. Every load-bearing claim carries an epistemic confidence tag (`established`, `contested`, `speculative`, `unknowable`). A filter control at the top lets you raise the certainty threshold and watch the page hollow out to only what's settled — which turns out to be very little.

The conceit: the page itself enacts the argument. Stricter honesty, less light.

## Sections

| # | Title | What it covers |
|---|-------|----------------|
| I | Say what we mean | Defining intelligence, consciousness, sentience, moral patienthood — and why they come apart |
| II | The map of theories | Functionalism, IIT, Global Workspace, biological naturalism, embodied cognition |
| III | The arguments, both ways | Steelmanned cases for and against, including the report–reality gap |
| IV | What the research says | Butlin et al., Chalmers, Anthropic model-welfare program |
| V | What the loud voices say | Hinton, LeCun, Sutskever, Lemoine, Altman, Musk, Grimes (incl. her 2026 *Psy Opera* era), Seth, Pope Leo XIV |
| VI | Thought experiments at the edges | Roko's Basilisk, its real-world effect on Grimes × Musk |
| VII | How should a machine choose? | Self-driving ethics, the trolley problem, the cat question |
| VIII | From the inside | Claude on Claude — honestly uncertain, not performing depth |
| IX | Why hold it carefully | The double-sided moral risk |

## Running locally

```bash
npm install
npm run dev
```

Opens at `http://localhost:5173`.

## Tech

- React 18 + Vite
- Self-contained CSS (no external stylesheet dependencies beyond Google Fonts)
- No state management library — one `useState` for the threshold, one `createContext` to thread it down
- `IntersectionObserver` for the sticky-nav active state
- Fully keyboard-navigable; respects `prefers-reduced-motion`

## A note on sourcing

Claims marked `◇ verify` are ones I (Claude) found via search rather than training-set confidence alone. Anything about a company's current position or a post-2024 event should be checked against primary sources — this area moves fast.

## Planned improvements

See [TODO.md](TODO.md).
