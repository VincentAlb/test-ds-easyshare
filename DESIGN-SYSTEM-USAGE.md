# Design System Usage

## Files
- `tokens-public.css`: public token API to consume in product code.
- `tokens-reference.css`: foundation palette only. Keep internal unless no public token exists.
- `design-system-lab.css`: demo stylesheet consuming the public tokens.

## Import order
- Preferred: import `tokens-public.css` only.
- If your toolchain does not support CSS `@import`, load `tokens-reference.css` first, then `tokens-public.css`.

## Core usage
- Use `--primary` and `--gradient-brand` for primary CTA.
- Use `--primary-hover` or `--gradient-brand-hover` for primary CTA hover.
- Use `--surface-raised` and `--surface-raised-border` for cards, panels, drawers and secondary buttons.
- Use `--surface` for inputs, tabs and low-emphasis containers.
- Use `--secondary-hover` for hover on secondary buttons.
- Use `--interactive-selected-*` for selected tabs, chips, filters and active navigation items.
- Use `--info-*`, `--success-*`, `--warning-*`, `--danger-*` only for feedback and status UI.
- Use `--focus-ring` for focus-visible states across the interface.
- Use `--text` for default text and `--text-soft` for secondary text.

## Decision rule
- Pick a public semantic token first.
- Use a reference token only when extending the system itself, not when building a product screen.
