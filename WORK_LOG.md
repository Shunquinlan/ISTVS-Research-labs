# Work Log — ISTVS Research Labs website

Running log of work sessions. Times are recorded from real clock times, never estimated.

**Current phase:** Week 2 — lab data structure and template planning (resumed 2026-10-10 after a ~2-week break)

---

## 2026-09-01

- **Time:** 18:00 – 23:00 (5.0 h)
- **Done:**
  - Planned the project approach: agreed the 8-week phasing, the
    "smallest-appropriate-step" workflow, and the beginner-friendly ground rules;
    captured all of it in the project skill and `docs/requirements.md`
  - Reviewed the current project folder and identified what Week 1 still needs
  - Created the `istvs-research-labs-web` project skill under `.claude/skills/`
    (project purpose, tech direction, design system, data model, QA checklist)
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
  - Reviewed `docs/requirements.md` and compiled `docs/questions-for-istvs.md`
    for the advisor / Secretariat
  - Wrote a Week 1 progress report (`docs/reports/2026-09-01-week-1-report.*`)
  - Commits: `c97fdfe`, `9aad4fd`, `2dec94e`, `ffd7c9c`, `bb84b4f`
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
  - ~~**GitBook plan:** currently on a 14-day trial of a paid plan...~~
    **Resolved 2026-09-04** — see below. ISTVS is already on GitBook's
    nonprofit Community plan; the site should be built inside the existing
    ISTVS GitBook org, not a paid personal-account plan.
  - ~~**Account ownership:** ... transfer ownership to an ISTVS-controlled
    account...~~ **Resolved 2026-09-04** — see below. Massimo Martelli will
    create the space directly inside the ISTVS GitBook org and add
    collaborators to the ISTVS GitHub org, so there is no separate transfer
    step later.
- **Next (Week 2):**
  - Design the lab-data spreadsheet structure (columns, category list)
  - Confirm the lab data fields with the ISTVS Secretariat (Massimo Martelli),
    who holds the existing Knack database
  - Review `docs/requirements.md` together

## 2026-09-04

- **Platform review meeting held** with Dr. Tekeste, Massimo Martelli (ISTVS
  General Secretariat), and Lutz Richter — Shun presented the six-platform
  comparison and the GitBook + GitHub recommendation.
- **Outcome: recommendation approved.** Key facts confirmed live by Massimo
  Martelli, which change two things this project assumed:
  - **Cost: $0, not ~$1,356/yr.** ISTVS is already on GitBook's **nonprofit
    Community plan** (multiple admins/editors, custom domain, all advanced
    features) at no cost — this is the exact plan ISTVS already uses for its
    year.istvs.org conference sites. No new subscription is needed.
  - **Hosting: build inside the existing ISTVS org, not a student account.**
    Massimo will create the new GitBook space directly inside the ISTVS
    GitBook organization and add the project's collaborators to the ISTVS
    GitHub org. This removes the "transfer ownership before launch" blocker
    entirely — there's nothing to transfer.
  - **Domain pattern confirmed.** ISTVS already uses `<year>.istvs.org` for
    conference sites on this same GitBook+GitHub workflow; `res-labs.istvs.org`
    (or `lab.istvs.org`) follows that existing pattern.
  - **Knack correction:** ISTVS is **not** retiring Knack entirely — it stays
    as the members database. Only the public Research Facilities directory is
    moving off Knack onto the new site.
  - Massimo has an existing Python automation (built for generating conference
    proceedings/pages) that generates Markdown files from structured data and
    syncs them to GitBook — a possible reference or reuse point for the
    labs-from-spreadsheet automation planned for Week 2.
- **Action item (Shun):** send Massimo a list of everyone who needs access —
  full name, email, and GitHub username — for two things: (1) GitHub
  collaborator access on the repo, (2) GitBook admin/editor access on the new
  space. Include Dr. Tekeste (wants visibility, not necessarily an editor
  role). Massimo will do the invites in the first days of the following week.
- **Still open:** the actual email/GitHub-username list for John Sheriff and
  Jaush Tai (see `docs/questions-for-istvs.md`).

## 2026-09-10

- **Access confirmed.** Shun was added as a collaborator on the real
  `res-labs` GitHub repo, under the ISTVS org
  (https://github.com/istvs/res-labs) — not a student personal account,
  matching what Massimo described on the call. GitBook<->GitHub sync is
  already tested and working (the test sync commits/log entries currently in
  the repo are Massimo's placeholders, not real content — clear them out
  when real work starts).
- **Blocker from the platform-review meeting is now fully closed:** cost
  ($0, nonprofit plan), hosting (inside the ISTVS org), and access are all
  resolved as of this entry.
- **Next:** start Week 2 — design the lab-data spreadsheet structure, get the
  Knack export from Massimo, and replace the placeholder README/SUMMARY with
  real project content.


## 2026-10-10

- **Time:** __:__ – __:__ (Shun to fill in)
- **Done:**
  - Resumed the project after a ~2-week break (illness + exam preparation)
  - Committed leftover Week 1 files (platform deck, executive summary, pricing
    notes) — commit `3def511`
  - Cloned the real ISTVS repository `istvs/res-labs` to
    `C:\Users\quinl\GitHub\res-labs` (outside OneDrive). It contains only
    README.md, SUMMARY.md and LICENSE; README has two sync-test lines from Massimo
  - **Received the Knack export from Massimo** (`ISTVS_Research_facilities_DB.zip`:
    .xlsx/.csv/.json/.txt)
  - Reviewed every record and built `docs/data/knack-review-2026-10-10.xlsx`
- **Findings:**
  - 38 records (39 in the .csv/.json — the extra one is a test entry) but only
    **13 distinct labs**; **6 have complete profiles**
  - The rest are test entries, duplicates, or soil-data form "fragments"
  - The current public page shows Iowa State twice (two records set to Display = Yes)
  - 75 export columns (43 Knack fields split into sub-columns); location data has errors
  - 21 logos/photos/PDFs are stored on Knack's servers
- **Decisions:** none final — all proposals in the review workbook await confirmation
- **Blockers:** none
- **Next:** confirm field decisions, pick the representative lab, draft the lab page template

## 2026-10-19

- **Time:** __:__ – __:__ (Shun to fill in)
- **Done:**
  - Re-checked the Knack review: confirmed .xlsx = .csv minus one test record;
    fixed a drop-down list bug
  - Drafted 8 research-area browse tags from the labs' own descriptions
    ("Draft Tags" tab) and tagged the 8 labs that have descriptions
  - Drafted the reusable lab page template (`docs/template/lab-template.md`) and
    one filled-in example for the ISU Soil Machine Dynamics Laboratory
    (`docs/template/isu-smd-lab.md`) plus a browser preview
  - Listed all 21 Knack files to archive (`docs/data/knack-assets-list.csv`);
    downloading them was blocked from the assistant's side, so Shun runs one
    PowerShell command
  - Added the open questions from the review to `docs/questions-for-istvs.md`
- **Decisions (pending Shun's confirmation):** representative lab = ISU SMD Lab;
  32-column master structure; 8 draft tags
- **Found:** the GitBook site is already live at res-labs.istvs.org (Community
  plan), showing the "WORK IN PROGRESS" test page. The content space is
  "ISTVS Resouce Laboratories" (typo).
- **Blockers:** (1) GitBook: can't create a change request; all spaces are greyed
  out in the "New change request" menu, so editor access is needed from Massimo.
  (2) Stakeholder answers to the open questions (email not sent yet; on hold)
- **Next:** try the example page in a GitBook change request (not published);
  send the review + questions; Week 3 = stakeholder review of the one page

---

### Week 1 — Summary (for hours log)

- **Planning:** spent the week planning the project approach and drafting the
  rough 8-week phase plan (setup -> data model -> design -> build -> handoff),
  captured in `docs/requirements.md` and the project skill.
- **Platform pitch:** researched and built a presentation comparing six
  website platforms (GitBook+GitHub, Squarespace, Wix, WordPress, Webflow,
  Google Sites) across 20 criteria, and presented it to Dr. Tekeste, Massimo
  Martelli, and Lutz Richter.
- **Key thing learned in that meeting:** ISTVS's own conference sites
  (`<year>.istvs.org`) already run on the exact platform combo recommended —
  GitBook + GitHub — and it's free, because ISTVS's nonprofit status already
  qualifies it for GitBook's Community plan.
- **Side note:** retiring Knack outright is not happening — only the Research
  Facilities / lab directory section is migrating off it onto the new site;
  Knack stays in place as the members database.
- **Outcome:** got a go-ahead in that meeting to start Week 2.
- **Hours:** 13 hours of Week 1 work logged in Workday under Week 2 (Workday
  wouldn't accept entries dated before the official student-worker hire date).

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
