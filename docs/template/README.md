# Lab page template (DRAFT, not approved)

Week 2 deliverable: one reusable lab page, designed before any automation.

| File | What it is |
|---|---|
| `lab-template.md` | The reusable template. Each `{{field_name}}` matches a column in the proposed master spreadsheet (see `docs/data/knack-review-2026-10-10.xlsx`, "Proposed Master" tab). |
| `isu-smd-lab.md` | The template filled in by hand for one representative lab: Iowa State's Soil Machine Dynamics Laboratory. |
| `isu-smd-lab-preview.html` | A rough browser preview of the example page. Double-click it to open it. The real look comes from GitBook's theme. |

## Rules the template follows

- Same section order on every lab page: details table, buttons, Overview, Facilities, Soils, Services, Publications, Highlights, Contact.
- If a lab has no information for a section, the section is left out, not shown empty.
- Only GitBook-native Markdown: a table, buttons, figures, and one info hint. No custom code.
- Images currently point at Knack's servers. Before launch they get downloaded (see `docs/data/knack-assets-list.csv`) and moved into `.gitbook/assets/`.

## Status

- [ ] Shun reviews the draft
- [ ] Tried in a GitBook **change request** (a draft that is not published)
- [ ] Shown to Dr. Tekeste and Massimo
- [ ] Revised and approved. Only after this: build the other pages and the automation.
