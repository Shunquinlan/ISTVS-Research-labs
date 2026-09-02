# Design system — ISTVS Research Labs

The site should feel like an appropriate collaboration between ISTVS and Iowa
State University: a professional academic/research directory, not a startup
landing page. Restraint is the whole aesthetic.

## Visual references

Look at these for tone and structure. **Do not copy either exactly.**

- <https://www.istvs.org/> — ISTVS identity, earth/gold feel, academic society tone.
- <https://www.grad-college.iastate.edu/programs/agricultural_and_biosystems_engineering>
  — Iowa State academic-program layout, typography, spacing.

Target: the readability and calm of a university department page, with ISTVS's
earthy palette and a restrained Iowa State cardinal/gold accent.

## Colour

Use a small palette. One primary, one accent, a short neutral ramp. Do not
introduce colours ad hoc per page.

Starting values — confirm against the official ISTVS and Iowa State brand
guidelines before launch:

| Role | Value | Use |
|---|---|---|
| Primary (ISTVS earth) | `#5B4A2F` warm brown / `#7A6A45` | headings, header/footer, primary text accents |
| ISTVS gold | `#C89B3C` | secondary accent, rules, hover states |
| ISU cardinal | `#C8102E` | sparing accent — key links, active nav, primary buttons |
| ISU gold | `#F1BE48` | sparing highlight — never as body background |
| Ink | `#1F1B16` | body text |
| Muted | `#6B6459` | secondary text, captions |
| Line | `#E4DFD6` | borders, dividers, card edges |
| Surface | `#FFFFFF` | cards, content background |
| Page | `#FAF8F4` | page background |

Rules:

- Cardinal and ISU gold are **accents**, used sparingly — a button, an active
  link, a thin top rule. They should never dominate a page or fill large areas.
- Every text/background pair must meet **WCAG AA** (4.5:1 for body, 3:1 for large
  text). Check cardinal-on-white and gold combinations explicitly — ISU gold on
  white fails for text.
- No gradients. Flat fills only.

## Typography

- One serif or humanist sans for headings, one highly readable sans for body.
  Reasonable choices: **Source Serif / Charter / Georgia** for headings,
  **Source Sans / Inter / system-ui** for body. Pick one pairing and keep it
  everywhere.
- Prefer web-safe or GitBook-supported fonts. Do not load multiple decorative
  fonts. No "random" font per section.
- Body text ~16–18px, line-height ~1.6, measure ~65–75 characters.
- A clear type scale (e.g. 1.25 ratio). Headings get weight and spacing, not
  colour tricks.

## Spacing and layout

- Generous whitespace. Consistent spacing scale (4 / 8 / 12 / 16 / 24 / 32 / 48 /
  64). Don't use off-scale one-off margins.
- Content max-width ~720–900px for reading pages; the directory grid can be wider.
- Consistent page rhythm: same header, same footer, same vertical spacing between
  sections on every page.

## Components — keep them consistent

Define each once and reuse. Same padding, radius, border, and hover treatment
everywhere.

- **Cards** (lab entries): surface background, 1px `Line` border, small radius
  (4–6px), consistent internal padding, title + institution + location + a short
  descriptor + one clear link. No drop shadows, or one subtle shadow used
  identically everywhere.
- **Buttons:** one primary style (cardinal fill, white text) and one secondary
  (outline). Visible hover and focus states. Real `<button>`/`<a>` elements.
- **Links:** underlined or clearly coloured in body text; consistent hover.
- **Headings:** consistent hierarchy, never skip levels for styling.
- **Navigation:** same position and order on every page; the current
  section/filter is visibly marked.

## Responsive

Layouts must work on desktop, tablet, and mobile.

- Fluid layouts; the directory grid collapses 3 → 2 → 1 column.
- No horizontal scrolling or overflow at 320px width.
- Tap targets ≥ 44px. Navigation stays usable on small screens.

## Accessibility (not optional)

- Semantic HTML: `<header> <nav> <main> <footer>`, real headings, `<ul>` for
  lists, `<button>` for actions, `<a>` for navigation.
- Visible focus states on every interactive element — do not remove outlines
  without replacing them with something equally visible.
- Colour contrast AA across the board.
- Every image has meaningful `alt` text (or `alt=""` if purely decorative).
- Filter controls are real form controls with labels.

## Avoid

- Generic "AI-generated" look: heavy gradients, glassmorphism, glowing borders,
  purple-to-blue everything, giant hero with a vague tagline.
- Unnecessary animation. Small, purposeful transitions only (hover colour,
  focus). No scroll-triggered reveals, parallax, or bouncing.
- Flashy startup effects, oversized rounded corners, neon.
- Inconsistent colours or fonts between pages.
- Dashboards, charts, or "analytics" UI the project doesn't need.
- Extra dependencies for effects that plain CSS handles.
