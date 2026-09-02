# ISTVS Research Labs website

Source for the **Research Labs** directory website of the International Society
for Terrain-Vehicle Systems (ISTVS), built by the Iowa State University ISTVS
student chapter with the ISTVS General Secretariat.

The site replaces the Society's old "Research Facilities" database (previously in
Knack) with a simple, public, browsable directory of terramechanics and
terrain-vehicle research laboratories.

## How the site is published

- **GitBook** turns the Markdown files in this repository into web pages.
  Planned address: `res-labs.istvs.org`.
- **GitHub** (this repository) holds the source. GitBook and GitHub stay in sync,
  so a page can be edited two ways:
  - visually, in GitBook, or
  - by editing the Markdown file here in GitHub.
- Lab data will live in one spreadsheet. Later, a small script will turn each
  spreadsheet row into a lab page. That automation is **not built yet.**

## Repository layout

| Path | What it holds |
|---|---|
| `README.md` | This file |
| `WORK_LOG.md` | Log of work sessions (date, hours, what was done, next steps) |
| `docs/` | Project documentation — requirements, and later the maintenance guide |
| `Context/` | Background material and source documents |
| `.claude/` | Configuration for the Claude Code assistant used on this project |

More folders (site pages, the lab spreadsheet, the automation script) will be
added in later weeks, in the order set out in `docs/requirements.md`.

## Project status

Currently in **Week 1** of an 8-week plan: project setup. See `WORK_LOG.md` for
the current week and `docs/requirements.md` for the full plan.

## Editing this project

If you are new to this repository, start with `docs/requirements.md`. A
plain-language maintenance guide for future officers and students will be added
in Week 6.
