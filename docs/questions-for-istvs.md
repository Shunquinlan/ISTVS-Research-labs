# Questions for ISTVS — Research Labs website

Questions to resolve with Dr. Tekeste and, where noted, the ISTVS General
Secretariat (Massimo Martelli). Answers get folded back into
`docs/requirements.md`.

Status: **open** — raised 2026-09-01, Week 1. Updated 2026-10-19 (Week 2) after the Knack export review.

---

## New questions from the Knack review — 2026-10-19

Full details: `docs/data/knack-review-2026-10-10.xlsx` ("Read Me" tab).

1. May **contact emails** be shown publicly on the site? (The current public
   directory already shows a Contact column.)
2. Should the **soil-data submissions** (soil parameters, test apparatus, soil
   test methods, soil models, reports — Knack fields 1–5) appear on the site,
   now or later, or stay archived?
3. **MRTC** is complete but named "DRAFT" and hidden. Publish it or not?
4. Who is **Gedalyahu Manor**, and is **Iguana Technology LLC** (a company)
   meant to be listed?
5. Contact the **7 incomplete labs** for updated info before launch, or launch
   with the **6 complete** ones first?
6. Is the **Iowa State Soil Machine Dynamics Laboratory** OK as the one
   representative lab page for the template review?

## The existing lab data (Knack) — ANSWERED 2026-10-10

Massimo sent the full export (`ISTVS_Research_facilities_DB.zip`) on 2026-10-10:
38 records / 43 fields (75 columns in the export). Lab images and PDFs are
Knack assets linked from the `… : URL` columns and are still publicly
downloadable. Original questions kept below for reference.

- Can the Secretariat provide an **export of the current Research Facilities
  database** from Knack (Excel, CSV, or JSON)? This is needed to design the
  spreadsheet in Week 2.
- **How many research labs** are currently in the database?
- What **fields / columns** does the current record have? (We are assuming: lab
  name, institution, location, research category, principal investigator,
  description, capabilities / research areas, website, contact.)
- The Knack database stores **assets** — lab images and PDF documents. Should the
  new site display lab photos and/or link attached documents? If so, roughly how
  many labs have images today?
- Is there an agreed **list of research categories**, or do we define one?
- Any data that should **not** be published publicly (e.g. personal emails,
  internal notes)?

**Correction 2026-09-04:** Massimo clarified ISTVS is **not** retiring Knack
entirely — it stays as the members database. Only the public Research
Facilities directory is moving off Knack onto the new site.

## People and access

(Access is set up in Week 6 — this is just to confirm the list now.)

**Action item (open):** Massimo asked Shun to email him the full name, email,
and GitHub username for everyone who needs access, so he can add them as
GitHub collaborators and GitBook admins/editors. Include Dr. Tekeste
(wants visibility/watch access). Still need real emails + GitHub usernames for
John Sheriff and Jaush Tai below before that email can go out.

- Please confirm **full name, role, email, and GitHub username** for each person
  who should have edit access:
  - Dr. Tekeste — is the role "ISTVS US Secretary" and "advisor to the ISU
    student chapter"?
  - John Sheriff (President, Iowa ISTVS student chapter) — spelling correct?
  - "Jaush Tai" — full name spelling, and Secretary of which body (ISU student
    chapter)?
  - Anyone else who should be on the list?
- Does everyone on that list already have a **GitHub account**? (Free to create;
  needed for edit access.)

## Domain and hosting — ANSWERED 2026-09-04

- **Pattern confirmed.** ISTVS already uses `<year>.istvs.org` for its
  conference sites on this same GitBook+GitHub workflow, so `res-labs.istvs.org`
  (or `lab.istvs.org`) follows an existing, working pattern rather than being a
  new one-off. Exact subdomain still to be finalized with Massimo.
- **GitBook org confirmed.** ISTVS already has a GitBook organization (used for
  the conference sites). Massimo will create the new space directly inside it —
  no separate student-account site to migrate later.
- DNS control for `istvs.org` — not explicitly confirmed, but Massimo clearly
  administers the existing `<year>.istvs.org` subdomains, so this is his/the
  Secretariat's action when we're ready to point the domain.

## GitBook plan / cost — ANSWERED 2026-09-04

- **Resolved in the platform review meeting.** ISTVS is already on GitBook's
  **nonprofit Community plan** (confirmed live by Massimo Martelli) — the same
  plan already running the `<year>.istvs.org` conference sites. It includes
  multiple admins/editors, a custom domain, and Git Sync, at **$0 cost**. The
  new Research Labs space should be created inside that existing ISTVS org,
  not a new paid plan or a student trial account.
  (Prior estimate for reference — not what will actually happen — is in
  [../.claude/skills/istvs-research-labs-web/references/platform-pricing-2026-09.md](../.claude/skills/istvs-research-labs-web/references/platform-pricing-2026-09.md).)

## Site scope and features

- Is **category filtering** enough, or do users also need a **free-text search
  box**?
- After launch, how should a **new lab get added or an existing one updated**?
  Options: a public submission form, email to the Secretariat, or a direct
  edit by an authorized editor.
- Are there **calls to action** ISTVS wants on the site (e.g. "Submit your lab",
  "Join ISTVS", "Contact the Secretariat")?
- Is the site **English only**, or should it support other languages later?
- Does ISTVS want **visitor analytics** (GitBook has this built in)?

## Ownership and handoff

- **Resolved 2026-09-04 (partially):** no transfer needed. Massimo will create
  the GitBook space directly inside the ISTVS org and add collaborators to an
  ISTVS-side GitHub setup, so the site is never tied to a student personal
  account in the first place.
- Still open: who is the **long-term maintainer** after this 8-week project —
  a rotating student officer, the Secretariat, or the advisor? Dr. Tekeste
  asked to be added as a watcher/admin so he has visibility even though he
  described himself as not a GitHub developer.

## Review checkpoints

- Does ISTVS (Dr. Tekeste and/or the Secretariat) want to **review and approve**
  the landing-page and lab-profile design in Week 3 before pages are generated?
- Any **launch date** or event the Week 8 presentation should target?
