# Workspace instructions

## Project overview

- This repository is a small static web project. The main deliverable is `/workspaces/codespaces-blank/index.html`.
- The page is Korean-facing and does not require a framework, package manager, build step, or backend.
- Keep the implementation self-contained in `index.html` unless a future request requires separate assets.

## Implementation conventions

- Use semantic HTML and accessible controls.
- Preserve the existing language: user-visible copy, labels, and error messages should be in Korean.
- Use modern, standards-based CSS and vanilla JavaScript.
- Avoid external dependencies and remote assets unless the request explicitly requires them.
- Make layouts responsive and usable on mobile and desktop widths.
- Provide visible keyboard and focus states. Use an appropriate `aria-*` attribute or live region when dynamic results are announced.
- Do not change or add lottery business rules without an explicit request.

## Lottery page behavior

- Generate exactly six unique integers from 1 through 45.
- Sort generated numbers in ascending order.
- Keep the sixth generated result visually distinct as the bonus number.
- When redrawing, replace the full previous result rather than appending to it.
- Preserve enough history only if the UI explicitly provides a history feature.

## Working in this workspace

- Inspect the current file before editing and make surgical changes.
- Prefer `index.html` for shared styles and scripts in this static project.
- Validate changes with a local HTTP server and an available browser or DOM check.
- Test at least:
  1. Exactly six unique main numbers are produced.
  2. Main numbers are ordered from smallest to largest.
  3. Bonus number generation is within 1–45 and does not duplicate a main number.
  4. The page remains usable at narrow viewport widths.

