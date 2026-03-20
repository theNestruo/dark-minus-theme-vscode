[github.com/mkhamat/shhhed](https://github.com/mkhamat/shhhed)

## Design

Five brightness tiers, assigned by how much each token matters when scanning code:

| Tier | OKLCH L | Examples | Role |
|------|---------|----------|------|
| Canvas | — | Editor ![#1e1e22](https://placehold.co/10x10/1e1e22/1e1e22) `#1e1e22`, chrome ![#1a1a1e](https://placehold.co/10x10/1a1a1e/1a1a1e) `#1a1a1e` | Background |
| Recede | 0.56–0.60 | Comments ![#797981](https://placehold.co/10x10/797981/797981) `#797981`, Punctuation ![#74747a](https://placehold.co/10x10/74747a/74747a) `#74747a` | Present but not competing |
| Structural | 0.62–0.67 | Operators ![#929296](https://placehold.co/10x10/929296/929296) `#929296`, Keywords ![#918699](https://placehold.co/10x10/918699/918699) `#918699`, Attributes / properties / parameters / member vars ![#909094](https://placehold.co/10x10/909094/909094) `#909094` | Scaffolding |
| Semantic | 0.68–0.71 | Types ![#60b1b1](https://placehold.co/10x10/60b1b1/60b1b1) `#60b1b1`, Functions ![#729bcf](https://placehold.co/10x10/729bcf/729bcf) `#729bcf`, Strings ![#c48d2f](https://placehold.co/10x10/c48d2f/c48d2f) `#c48d2f`, Numbers ![#ca8489](https://placehold.co/10x10/ca8489/ca8489) `#ca8489` | Meaning |
| Reading | 0.76–0.79 | Variables ![#b8b8bc](https://placehold.co/10x10/b8b8bc/b8b8bc) `#b8b8bc`, Constructors ![#c6a6be](https://placehold.co/10x10/c6a6be/c6a6be) `#c6a6be`, Variants ![#c6a6be](https://placehold.co/10x10/c6a6be/c6a6be) `#c6a6be` | What you're reading |

- Near-neutral canvas with blue undertone. Compatible with Night Shift / f.lux.
- Palette computed in [OKLCH](https://oklch.com). Same-tier tokens differ by hue, not brightness.
- Saturation under 50% HSL (most under 40%) to reduce strain on dark backgrounds.
- Structural tokens clear 4.5:1 against the canvas (WCAG AA). Recede tokens sit at 3.5–4.1:1 — legible but not competing.

## Palette

| Token | Color | Hex |
|-------|-------|-----|
| Types | ![#60b1b1](https://placehold.co/16x16/60b1b1/60b1b1) | `#60b1b1` |
| Functions | ![#729bcf](https://placehold.co/16x16/729bcf/729bcf) | `#729bcf` |
| Strings | ![#c48d2f](https://placehold.co/16x16/c48d2f/c48d2f) | `#c48d2f` |
| Numbers | ![#ca8489](https://placehold.co/16x16/ca8489/ca8489) | `#ca8489` |
| Keywords | ![#918699](https://placehold.co/16x16/918699/918699) | `#918699` |
| Background | ![#1e1e22](https://placehold.co/16x16/1e1e22/1e1e22) | `#1e1e22` |
