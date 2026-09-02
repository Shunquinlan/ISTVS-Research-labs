# Work Log — ISTVS Research Labs website

Running log of work sessions. Times are recorded from real clock times, never estimated.

**Current phase:** Week 1 — project setup (GitHub repository, GitBook space, requirements)

---

## 2026-09-01

- **Time:** 18:00 – _(end time to be filled)_
- **Done:**
  - Reviewed the current project folder and identified what Week 1 still needs
  - Created the `istvs-research-labs-web` project skill under `.claude/skills/`
  - Initialized the git repository (branch `main`); set commit identity for this repo
  - Added baseline files: `README.md`, `WORK_LOG.md`, `docs/requirements.md`,
    `.gitignore`, `.gitattributes`
  - Wrote `docs/requirements.md` — a plain-language summary of the two source
    documents (ISTVS General Secretary's proposal + ISU chapter brief)
  - Deleted the empty `index.html` / `script.js` / `style.css` stubs
  - Created the private GitHub repository
    <https://github.com/Shunquinlan/ISTVS-Research-labs> and pushed `main`
  - Created the GitBook space, installed the GitBook app on GitHub, and connected
    two-way **Git Sync** (GitHub `main` <-> GitBook)
  - Added `gitbook-docs.yaml` (site structure) and a `site/` folder with a
    holding landing page; the published website is built only from `site/`
  - Published a preview: **<https://istvs-1.gitbook.io/istvs-docs/>**
  - Commits: `c97fdfe`, `9aad4fd`, `2dec94e`
- **Decisions:**
  - Site is published through GitBook from Markdown files in a GitHub repository
    (per the ISTVS General Secretary's proposal). No static-site framework.
  - GitHub repo is private for now; the published GitBook site is public. Repo can
    be made public later if ISTVS wants the source open.
  - Website content is kept in its own `site/` folder, separate from project
    material (`docs/`, `WORK_LOG.md`, `.claude/`, `Context/`, source PDFs), so the
    published site never accidentally includes internal files.
  - GitBook space is a single space named "Research Labs" at path `research-labs`
    (the URL path is a placeholder; revisit when the real structure is designed).
- **Blockers / open items:**
  - **GitBook plan:** currently on a 14-day trial of a paid plan. Git Sync is a
    paid feature. Before ~2026-09-15, move to GitBook's nonprofit/education plan
    (ISTVS is a nonprofit; likely eligible) or a paid plan. Raise with the
    advisor / ISTVS Secretariat.
  - **Account ownership:** the GitBook space and GitHub repo are under a student
    personal account. Before launch, transfer ownership to an ISTVS-controlled
    account so the site outlives student turnover.
- **Next (Week 2):**
  - Design the lab-data spreadsheet structure (columns, category list)
  - Confirm the lab data fields with the ISTVS Secretariat (Massimo Martelli),
    who holds the existing Knack database
  - Review `docs/requirements.md` together

---

### Progress update — Week 1 (shareable with the project advisor)

Dr. Tekeste,

Here is where the ISTVS Research Labs website stands after the first work session.

**Live preview:** https://istvs-1.gitbook.io/istvs-docs/
(This is a temporary GitBook address and only a placeholder page so far — the
real landing page and lab directory come in weeks 3–5.)

**What is set up**

- A GitHub repository now holds the project's source files, with version history:
  https://github.com/Shunquinlan/ISTVS-Research-labs (private for now).
- A GitBook space is connected to that repository with two-way sync, exactly as
  Mr. Martelli's proposal described: pages can be edited either visually in
  GitBook or as Markdown files in GitHub, and the two stay in sync automatically.
- The repository has a clear starting structure: a `README`, a plain-language
  `requirements` document summarising the ISTVS proposal and the ISU chapter
  brief, a work log, and a separate `site/` folder that is the only thing the
  public website is built from.
- Anyone with a GitHub account can be given edit access, so the team members
  named in the brief can be added when we are ready.

**Two items that need a decision soon**

1. *GitBook plan.* The GitHub sync feature GitBook charges for; we are on a
   14-day free trial. ISTVS is a nonprofit, so we should qualify for GitBook's
   nonprofit/education plan. It would help to know whether ISTVS already has a
   GitBook account or a preferred way to cover this before about 15 September.
2. *Ownership.* The repository and GitBook space are currently under my personal
   accounts. Before launch we should move them to an ISTVS-owned account so the
   site is not tied to one student.

**Next week (Week 2):** design the spreadsheet that will hold the lab records —
its columns and the list of research categories — and confirm those fields with
the ISTVS General Secretariat, who has the current lab database.

Best regards,
Shun
