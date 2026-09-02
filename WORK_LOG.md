# Work Log — ISTVS Research Labs website

Running log of work sessions. Times are recorded from real clock times, never estimated.

**Current phase:** Week 1 — project setup (GitHub repository, GitBook space, requirements)

---

## 2026-09-01

- **Time:** 18:00 – in progress (session expected to run to ~00:00)
- **Done so far:**
  - Reviewed the current project folder and identified what Week 1 still needs
  - Created the `istvs-research-labs-web` project skill under `.claude/skills/`
- **Decisions:**
  - Site is published through GitBook from Markdown files in a GitHub repository
    (per the ISTVS General Secretary's proposal). No static-site framework; the
    empty `index.html` / `script.js` / `style.css` stubs do not fit this plan and
    are pending removal.
- **Blockers:**
  - GitHub account is not logged in on this machine yet
- **Next:**
  - `git init` and add baseline files (README, .gitignore, docs/requirements.md)
  - Create the GitHub repository and push
  - Create the GitBook space and connect it to the repository
