# Repository Guidelines

## Project Structure & Module Organization

This repository is a dependency-free, single-page academic website served directly by GitHub Pages. `index.html` contains the page content, component markup, and feature-specific inline styles. `jemdoc.css` provides the shared base theme. Store page images in `figs/`; `codeforces.webp` is the existing root-level competitive-programming asset. `.nojekyll` ensures Pages publishes these files without Jekyll processing. There are currently no source-generation, test, or build directories.

## Build, Test, and Development Commands

No install or build step is required. Preview through HTTP so relative assets behave as they do in production:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/`. Before submitting changes, run:

```bash
git diff --check
git status --short
```

The first command catches whitespace errors; the second confirms that only intended files changed. GitHub Pages deploys the repository root as-is.

## Coding Style & Naming Conventions

Preserve the existing XHTML-compatible markup and use entities such as `&amp;` where required. Indent nested HTML and inline CSS with two spaces; do not reformat unrelated legacy rules in `jemdoc.css`. Use lowercase kebab-case for CSS classes (`research-card`, `cp-header`) and short semantic names for section anchors (`publication`, `awards`). Keep asset names lowercase and descriptive, and reference them with relative paths. Reuse the established typography, restrained color palette, `em`-based spacing, and responsive breakpoints before introducing new patterns.

## Testing Guidelines

There is no automated test suite or coverage target. Manually verify the page at desktop and mobile widths, especially the research grid, publication lists, profile image, and competition chart. Check internal anchors, external links, image requests, and browser-console errors. Visual changes should be compared against the deployed layout in both viewport ranges around the `600px` breakpoint.

## Commit & Pull Request Guidelines

Recent history favors short, imperative summaries such as `Fix sidebar bio and update news year`. Use a specific subject instead of a generic `update`, and keep each commit focused on one content or presentation change. Pull requests should explain the user-visible result, list validation performed, and link any relevant issue. Include before/after screenshots for layout or styling changes, with both desktop and mobile views when responsiveness is affected.
