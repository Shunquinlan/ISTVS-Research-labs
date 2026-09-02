# Browser QA checklist

Run this before reporting any visual or interactive change complete, when
Playwright (or similar browser tooling) is available. If browser tooling is not
available, still open the page yourself and check what you can, and say what you
could not verify.

## Steps

1. **Launch the site** — open the page(s) affected by the change. Prefer the
   GitBook preview when the change involves GitBook-specific rendering; otherwise
   open the local HTML.
2. **Test every link** — click each navigation link and in-content link. Confirm
   each goes where its text implies. Note any 404s or dead anchors.
3. **Test every button and control** — filters, category nav, calls to action,
   any toggles. Confirm each does what it says.
4. **Test forms** if any exist — valid input, empty input, obviously invalid
   input. Confirm labels and focus order.
5. **Check for broken links** — including external `website`/`contact` links on
   lab pages if they're in scope for the change.
6. **Desktop layout** — check at a typical desktop width (~1280px). Spacing,
   alignment, the card grid, header/footer.
7. **Mobile layout** — check at ~375px. No horizontal scroll, nav still usable,
   grid collapses to one column, tap targets big enough.
8. **Tablet** — ~768px, mainly that the grid and nav transition cleanly.
9. **Overflow and spacing** — long lab names, long descriptions, long
   capability lists. Nothing clips, overlaps, or pushes the layout sideways.
10. **Browser console** — check for JavaScript errors and failed requests on
    each page touched.
11. **Screenshots** — capture the key pages (directory, a lab profile, mobile
    directory) and include them in the report.
12. **Compare to requirements** — hold the result against the design system and
    the maintainer's stated goals. Note gaps.
13. **Fix obvious issues** — spacing, alignment, contrast, broken links, console
    errors — before saying the change is done.

## Reporting

Report what you checked, what passed, what you fixed, and anything still open —
with screenshots. Don't claim "tested and working" without the evidence behind it.
