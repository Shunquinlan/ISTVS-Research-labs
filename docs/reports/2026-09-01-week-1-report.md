# ISTVS Research Labs Website — Week 1 Progress Report

**Prepared by:** Shun Quinlan, Iowa State University ISTVS Student Chapter
**For:** Dr. Tekeste — ISTVS US Secretary; Advisor, ISU ISTVS Student Chapter
**Date:** September 1, 2026
**Project week:** 1 of 8 — Project setup

---

## 1. Summary

Week 1 established the technical foundation for the new ISTVS Research Labs
website. The publishing platform (GitBook), the source repository (GitHub), and
the automatic two-way sync between them are set up and working, and a placeholder
site is live at a temporary address. The project is on schedule.

A short list of questions for ISTVS is included at the end of this report. The
answers shape Week 2, which is about designing the spreadsheet that will hold the
lab records.

## 2. What was set up this week

- **Project plan and ground rules.** Agreed an eight-week plan, a method of taking
  the smallest appropriate step at each stage, and beginner-friendly
  documentation standards. All of it is written down in the project repository.
- **GitHub repository** (private): the address is
  https://github.com/Shunquinlan/ISTVS-Research-labs . It holds every project
  file with a full history of changes.
- **GitBook space**, connected to the repository with two-way sync, exactly as
  the General Secretary's proposal described. Pages can be edited visually in
  GitBook or as text files in GitHub, and the two stay synchronized
  automatically.
- **Repository structure**, organized so that someone with little coding
  experience can follow it:
  - a README explaining what the project is;
  - a plain-language requirements document summarizing the ISTVS proposal and the
    ISU chapter brief;
  - a questions document (the list at the end of this report);
  - a work log recording each work session and its hours;
  - a `site` folder that is the only part of the repository the public website is
    built from, kept separate from internal project files.
- **Live preview:** https://istvs-1.gitbook.io/istvs-docs/ . This is a temporary
  GitBook address with a single placeholder page. The real landing page and lab
  directory are built in Weeks 3 to 5.

## 3. Decisions made

| Decision | Reason |
| --- | --- |
| GitBook plus GitHub, with no website framework | Matches the General Secretary's proposal; keeps the site editable by non-coders |
| Repository private for now; the published site is public | Standard practice; the source can be opened later if ISTVS wants |
| Website content isolated in its own `site` folder | Prevents internal project files from appearing on the public site |
| Lab data lives in one spreadsheet for now | The number of labs is small; a full database can be added later |
| A page template is designed and approved before any automation is written | Required by the General Secretary's proposal |

## 4. Items that need an ISTVS decision soon

1. **GitBook plan.** GitBook's GitHub-sync feature is a paid feature. The project
   is on a 14-day free trial that ends around **September 15, 2026**. ISTVS is a
   non-profit and should qualify for GitBook's non-profit or education plan, which
   is free or discounted. A decision is needed before the trial ends.
2. **Account ownership.** The repository and the GitBook space are currently under
   a student personal account. Before launch they should be moved to an
   ISTVS-owned account so the site is not tied to one student.

## 5. Next week (Week 2)

- Design the spreadsheet that will hold the lab records — its columns and the list
  of research categories.
- Confirm those fields against the existing lab database, which the ISTVS General
  Secretariat holds.

## 6. Questions for ISTVS

### The current lab data (highest priority)

1. Can the Secretariat provide an export of the current Research Facilities
   database from Knack (Excel, CSV, or JSON)? It is needed to design the
   spreadsheet in Week 2.
2. How many research labs are currently in the database?
3. What fields does each record have today? We are assuming: lab name,
   institution, location, research category, principal investigator, description,
   capabilities or research areas, website, and contact.
4. The Knack database also stores images and PDF documents for each lab. Should
   the new site display lab photos and link those documents?
5. Is there an agreed list of research categories, or do we define one?
6. Is there any data that should not be published publicly?

### People and access (setup is Week 6 — confirming the list now)

7. Please confirm the full name, role, email, and GitHub username for each person
   who should have edit access:
   - Dr. Tekeste — is the role "ISTVS US Secretary" and "advisor to the ISU
     student chapter"?
   - John Sheriff — President, Iowa ISTVS student chapter — is the spelling
     correct?
   - "Jaush Tai" — correct spelling, and Secretary of which body?
   - Anyone else who should be on the list?
8. Does everyone on that list already have a GitHub account?

### Domain and hosting

9. The proposal suggests `res-labs.istvs.org`. Is that the final address, or an
   example?
10. Who controls DNS for `istvs.org`? The main ISTVS site is on Squarespace.
    Setting up the custom address is an ISTVS action, likely in Week 6 to 8.
11. Does ISTVS already have a GitBook account or organization the site should live
    under?

### Site scope

12. Is category filtering enough, or do users also need a free-text search box?
13. After launch, how should a new lab be submitted or an existing one updated — a
    public submission form, email to the Secretariat, or a direct edit by an
    authorized editor?
14. What calls to action does ISTVS want on the site (for example "Submit your
    lab", "Join ISTVS", "Contact the Secretariat")?
15. Is the site English only, or should it plan to support other languages later?
16. Does ISTVS want visitor analytics? GitBook provides this built in.

### Ownership and handoff

17. When and how should ownership of the repository and GitBook space transfer to
    ISTVS?
18. Who is the long-term maintainer of the site after this eight-week project?

### Review checkpoints

19. Does ISTVS want to review and approve the landing-page and lab-profile design
    in Week 3, before pages are generated?
20. Is there a target launch date or event for the Week 8 presentation?
