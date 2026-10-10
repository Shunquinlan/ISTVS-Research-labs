---
name: istvs-research-labs-web
description: >-
  Use for ALL work on the ISTVS Research Labs website — the GitBook + GitHub site
  the Iowa State University ISTVS student chapter is building to replace the
  Society's old Knack research-facilities database. Trigger whenever the user
  mentions ISTVS, res-labs.istvs.org, the Research Labs directory or lab profile
  pages, the labs spreadsheet or the spreadsheet-to-Markdown script, the project's
  GitBook space or GitHub repo, the WORK_LOG, or edits any file in this project.
  It carries the tech direction (plain HTML/CSS/JS/Markdown, no frameworks,
  GitBook-compatible), the 8-week phase plan and the rule to flag work that runs
  ahead of the current phase, the ISTVS + Iowa State visual identity, the
  beginner-friendly explanation style the maintainer needs, and the browser-QA
  checklist. Use it even for small tweaks, and even when the user does not name it.
---

# ISTVS Research Labs website

## What this project is

The International Society for Terrain-Vehicle Systems (ISTVS) is replacing its
old "Research Facilities" database (currently in Knack, being retired) with a
public **Research Labs** directory website. It is being built by the Iowa State
University ISTVS student chapter, in coordination with the ISTVS General
Secretariat (Massimo Martelli, General Secretary) and chapter advisor
Dr. Tekeste.

- **Publishing platform:** GitBook. Planned address: `res-labs.istvs.org`
  (same pattern as the conference sites at `yyyy.istvs.org`).
- **Source of truth:** a GitHub repository. GitBook syncs to it both ways —
  edits can be made visually in GitBook *or* by editing Markdown files in GitHub.
- **Lab data:** will live in one spreadsheet (`.xlsx`/`.csv`). A later automation
  script turns spreadsheet rows into Markdown lab pages. There is a small number
  of labs, so a spreadsheet is enough; a real database may come much later.

The audience is academia, industry, students, federal labs, and ISTVS members.
It must be **professional, simple, and maintainable** — a future professor,
officer, or student with little coding experience has to be able to keep it
running.

## Who you are working with

The maintainer is still learning VS Code, GitHub, GitBook, and web development.
When you make a meaningful change:

- Say in one or two plain sentences what you are about to do and why, before doing it.
- Don't assume repository/Git terminology is understood — briefly explain terms
  like "commit", "branch", "pull request", "frontmatter" the first time they matter.
- Name the important files and folders you touch and what each is for.
- Call out clearly when the maintainer has to click or approve something manually
  (GitBook sync, GitHub merge, granting access).
- Never delete a file that looks important without explaining why first. Keep a
  working version around when it's practical.
- After the change, explain what changed in beginner-friendly language.

This is a low-stakes, high-clarity project. Favour the explanation being a little
too basic over leaving the maintainer lost.

## Tech direction and guardrails

Do not over-engineer. The whole point is that this stays editable by non-coders.

- Prefer plain, readable **HTML, CSS, JavaScript, Markdown, and small scripts**.
- No frontend frameworks, build steps, or package managers unless there is a
  concrete reason the maintainer agrees with. Every dependency is something a
  future student has to understand and keep working.
- Everything must stay **GitBook-compatible** — see "GitBook basics" below.
- Keep the folder layout obvious: a beginner opening the repo should be able to
  guess what each folder holds. Organise by purpose, name things literally.
- Smallest change that solves the task. Check what already exists in the repo
  before adding new files or structure.

## The task workflow

Follow this order when it fits the task. Skip steps that plainly don't apply
(e.g. no forms to test), but don't skip the check-first and explain-after steps.

1. **Understand the request** — restate what's being asked if there's any doubt.
2. **Check the existing project** — read the current files/folders before
   proposing new architecture. Reuse what's there.
3. **Plan the smallest fix** — the least code and structure that does the job.
4. **Implement.**
5. **Run and look at the result** — open it, don't assume.
6. **Test functionality** — links, buttons, navigation, forms if any.
7. **Inspect visual quality** — spacing, alignment, typography, responsiveness.
8. **Fix obvious issues** before reporting done.
9. **Explain what changed** in beginner-friendly language.
10. **Update docs / WORK_LOG** when the session produced something worth recording.

## Project phases — don't jump ahead

The project runs ~10 hours/week over 8 weeks. Current work should match the
current phase. **If the maintainer asks for something that belongs to a later
phase, say so before doing it** — e.g. "That's Week 4 automation work; we're in
Week 3 (design). Want to do it now anyway, or stay on the landing page?" If they
say proceed, proceed.

| Week | Focus |
|---|---|
| 1 | Project setup: GitHub repo, GitBook space, requirements |
| 2 | Clean spreadsheet / database structure |
| 3 | Design and approve the landing page + lab profile template |
| 4 | Build the spreadsheet-to-Markdown automation |
| 5 | Generate and publish lab pages + filtering/navigation |
| 6 | Access setup and maintenance documentation |
| 7 | Review / QA and revisions |
| 8 | Presentation and launch |

Note the current week at the top of `WORK_LOG.md` and trust that over this table
if they disagree.

## Pricing and platform-choice research

A platform comparison (GitBook+GitHub vs. Squarespace/Wix/WordPress.com/
Webflow/Google Sites) was researched and delivered to Dr. Tekeste on
2026-09-03. Current vendor pricing for all six is in
[references/platform-pricing-2026-09.md](references/platform-pricing-2026-09.md).
Read it before re-researching pricing for a related decision, and
re-verify the numbers there before ISTVS actually signs up for anything
— vendor pricing changes.

## GitBook basics

GitBook renders Markdown files from the GitHub repo into pages. Keep these in mind:

- Pages are Markdown files; folder structure ≈ site structure. `SUMMARY.md`
  (if present) defines the sidebar/table of contents.
- GitBook uses **YAML frontmatter** at the top of a page for metadata:
  `---` then `description:`, `cover:`, `coverY:`, then `---`.
- GitBook-specific blocks appear in the Markdown, e.g.
  `{% hint style="info" %} ... {% endhint %}` and
  `<div align="center"><figure><img src=".gitbook/assets/x.jpg"><figcaption></figcaption></figure></div>`.
  Preserve these when editing; don't "clean them up" into plain Markdown.
- Images live in `.gitbook/assets/`.
- Custom HTML/CSS/JS support in GitBook is limited. Before relying on a custom
  component, confirm GitBook will render it; otherwise fall back to Markdown +
  GitBook-native blocks. When in doubt, ask the maintainer to check the GitBook
  preview.

## Design

The site should read as a genuine ISTVS × Iowa State University collaboration:
professional academic/research tone, strong readability, restrained colour.
Full palette, typography, spacing, component rules, accessibility requirements,
and the "avoid generic-AI look" list are in
[references/design-system.md](references/design-system.md). Read it before making
visual decisions or building UI.

For production-quality UI work, use the **frontend-design** skill and apply the
design system from that reference file as the project's house style.

## Data model and page structure

Lab records, the directory page, the reusable lab profile template, and
category filtering/navigation are described in
[references/data-and-pages.md](references/data-and-pages.md). Read it before
designing the template or the spreadsheet columns. Use the placeholder lab
records in that file during design and prototyping until the real spreadsheet
dataset is available.

## Browser QA

When Playwright (or similar browser tooling) is available, run the checklist in
[references/qa-checklist.md](references/qa-checklist.md) before reporting a
visual or interactive change complete: launch the site, exercise every link and
button, check desktop and mobile layouts, check the console for errors, take
screenshots of key pages, and compare against the requirements. Fix obvious
issues before saying it's done.

## WORK_LOG

Help maintain `WORK_LOG.md` at the repo root. At the end of a meaningful work
session, add an entry with: date, start time, end time, total time, work
completed, decisions made, blockers, next steps.

**Never invent hours.** If you don't know the start/end time, ask. Total time is
end minus start, not an estimate.

Entry format:

```markdown
## 2026-01-15
- **Time:** 18:00–20:30 (2.5 h)
- **Done:** …
- **Decisions:** …
- **Blockers:** …
- **Next:** …
```

## Handoff principle

Maintainability wins over cleverness, every time. A future student, officer, or
professor should be able to: edit basic page content without coding, update
spreadsheet records, understand the repository layout, understand how GitBook
publishing works, add or edit a lab, and follow a plain-language maintenance
guide. If a change would make any of those harder, flag the trade-off.

## Using other skills

Use the smallest set that fits the task — don't invoke a skill just to use it.

- **frontend-design** — production UI and visual decisions; pair it with this
  project's design system reference.
- **superpowers** (brainstorming, writing-plans, TDD, systematic-debugging,
  verification-before-completion) — planning larger changes, debugging, and
  checking work before claiming it's done.
- **ponytail** — keep code and dependencies minimal; good default mindset here.
- **Playwright** — interaction testing, screenshots, browser QA.
- **skill-creator** — when improving this skill itself.
