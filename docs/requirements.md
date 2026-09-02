# Requirements — ISTVS Research Labs website

Plain-language summary of the two source documents in this project:

- `ISTVS_Research_Labs_GS_20260722.pdf` — proposal from Massimo Martelli,
  ISTVS General Secretary (2026-07-22)
- `ISU-ISTVS WEBSITE MANAGEMENT FOR RESEARCH LABSISU.docx` — ISU student chapter
  project brief

If this summary and a source document disagree, the source document wins — note
the fix here.

## Goal

Replace the ISTVS "Research Facilities" database (currently in Knack, to be
retired) with a simple, public, professional website that lets people browse
terrain-vehicle / terramechanics research laboratories.

## Audience

Academia, industry, students, federal laboratories, and ISTVS members. The site
must be easy for the general public to visualize and, above all, **simple**.

## Platform decisions (from the GS proposal)

- **Publishing:** GitBook (`gitbook.com`), on a subdomain like
  `res-labs.istvs.org`, matching the ISTVS conference sites (`yyyy.istvs.org`).
- **Source control:** a GitHub repository. GitBook has built-in GitHub
  integration; the repository is the "source code" for the site.
- **Access:** anyone with a GitHub account can be given editor/admin access.
  Edits can be made visually in GitBook or directly in the Markdown files on
  GitHub.
- **Data:** for now, a single spreadsheet file (`.xlsx` / `.csv`). The number of
  labs is relatively small. A full database may be adopted later by importing the
  spreadsheet.
- **Automation:** scripts can process the spreadsheet and generate the Markdown
  pages for the site. **A page template must be designed and approved before any
  automation is written.**

## People with intended edit/publish access

From the ISU brief (names as written there):

- Dr. Tekeste — US Secretary and advisor to the ISTVS ISU student chapter
- Shun Quinlan — ISTVS student chapter member
- John Sheriff — President, Iowa ISTVS student chapter
- Jaush Tai — Secretary

Admin access to the wider ISTVS database stays with the ISTVS General
Secretariat.

## What the directory should let people do

Browse labs by information such as: laboratory name, institution, location,
research category, principal investigator, description, capabilities / research
areas, and website / contact.

Planned pages:

- a Research Labs landing / directory page
- a reusable lab profile page (one per lab)
- simple category navigation / filtering
- clear calls to action

Placeholder lab records are used during design until the real spreadsheet
dataset is available.

## Design direction

Professional academic/research appearance; strong readability; clean typography;
generous whitespace; restrained colour (ISTVS earth/gold with sparing Iowa State
cardinal/gold accents); consistent components; responsive; accessible. Visual
references: <https://www.istvs.org/> and
<https://www.grad-college.iastate.edu/programs/agricultural_and_biosystems_engineering>
(do not copy either).

Full design system: `.claude/skills/istvs-research-labs-web/references/design-system.md`.

## Constraints

- Do not over-engineer. Prefer plain HTML, CSS, JavaScript, Markdown, and small
  scripts. Avoid frameworks and dependencies without a clear reason.
- Everything stays GitBook-compatible.
- Keep files and folders organized and obvious to a beginner.
- Maintainability first: a future professor, officer, or student with little
  coding experience must be able to keep the site running and edit content.

## 8-week plan

| Week | Focus |
|---|---|
| 1 | Project setup: GitHub repository, GitBook space, requirements |
| 2 | Clean spreadsheet / database structure |
| 3 | Design and approve the landing page + lab profile template |
| 4 | Build the spreadsheet-to-Markdown automation |
| 5 | Generate and publish lab pages + filtering / navigation |
| 6 | Access setup and maintenance documentation |
| 7 | Review / QA and revisions |
| 8 | Presentation and launch |

Work that runs ahead of the current week should be flagged before it is done.

## Future opportunities (not in the 8-week scope)

- Expand into an "ISTVS Resource Initiative" style professional-services platform.
- A resource library for simulation and modeling / terramechanics virtual tools,
  potentially sponsored by simulation software companies with ISTVS leadership
  approval.
