# Dots Knowledge Resources

**Knowledge resources** for Dots: data structures, competitive research, and positioning material as static, self-contained HTML documents. No build step, no dependencies.

## Contents

| File | Title | Purpose |
|---|---|---|
| `index.html` | Why Dots: Product Benchmarking | Competitive positioning page — where Dots sits vs. adjacent tool categories, capability comparison matrix, and a decision guide for "is Dots right for you." |

More resources will be added here over time — see [Adding a new resource](#adding-a-new-resource).

## Tech stack

- Plain HTML5 + CSS (custom properties for theming, CSS Grid/Subgrid)
- Vanilla JS only where needed — no frameworks, no bundler
- Google Fonts (`DM Sans`, `DM Serif Display`) via CDN

## Running locally

No server or build step required:

```bash
open index.html
```

## Editing content

All copy and ratings are hardcoded in the HTML — no CMS or data file behind it. Each section is marked with a numbered comment (`<!-- 1. HERO -->`, `<!-- 2. CATEGORY MAP -->`, `<!-- 3. CAPABILITY MATRIX -->`, etc.) — search for the comment to jump to the section you need to edit.

## Adding a new resource

1. Drop the new `.html` file in the repo root (or a subfolder if things grow, e.g. `/competitive/`, `/onboarding/`).
2. Add a row for it in the Contents table above.
3. Keep pages self-contained (inline `<style>`/`<script>`) unless the team introduces a shared template.
4. Reuse the `:root` CSS variables at the top of `index.html` for a consistent look.

## Notes

- Competitor names, comparisons, and claims reflect internal research — verify against current competitor offerings before external distribution.
