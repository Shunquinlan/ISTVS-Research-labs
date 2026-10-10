---
description: >-
  Researched pricing and platform-comparison findings for the ISTVS Research
  Labs website decision (GitBook+GitHub vs. Squarespace/Wix/WordPress.com/
  Webflow/Google Sites). Read this before re-researching pricing for the same
  decision — it saves re-doing the September 2026 research pass.
---

# Platform pricing reference — checked September 2026

Source: research done for the "Platform Evaluation & Recommendation" deck
delivered to Dr. Tekeste, 2026-09-03. Official vendor pricing pages where
fetchable; cross-checked against a secondary source where a page rendered
client-side with no numeric figures (noted below). **Re-verify before ISTVS
signs up for anything — vendor pricing changes.**

## GitBook (the one that matters most for this project)

- **Free:** $0. 1 user. GitHub/GitLab sync included. No custom domain, no team
  collaboration, no advanced branding/analytics.
- **Premium:** $65/site/month (billed annually). Additional team members are
  **$12/user/month on top** — the base price does not appear to bundle extra
  seats. Adds: custom domain, team collaboration, analytics, feedback,
  redirects.
- **Nonprofit / Open Source:** a free Community plan exists — application
  required, eligibility to confirm. **This is the single biggest cost lever
  for this project** — if ISTVS qualifies, the Premium estimate below drops
  to $0/yr. Apply before relying on a paid-plan budget number.
- Illustrative production cost for ~4 named editors (Shun, Dr. Tekeste, John
  Sheriff, Jaush Tai): $65 + 4×$12 = **$113/mo ≈ $1,356/yr** — this assumes
  all 4 need individual paid seats, which has not been confirmed with
  GitBook. Verify seat count before budgeting.
- Correction: `docs/questions-for-istvs.md` (written 2026-09-01) estimated
  the sync feature at "~$8/user/month" — that was a rough guess before this
  research pass. The real Premium pricing is the $65/site + $12/user
  structure above.

## GitHub

- **Free** already covers this project: unlimited private repositories,
  unlimited collaborators. No reason to pay for Team ($4/user/mo) — its
  extra features (Codespaces, more CI minutes) aren't needed here.

## The five alternatives (production-scale estimate, ~4 editors, custom domain)

| Platform | Recommended tier | Est. / year | Note |
|---|---|---|---|
| Squarespace | Core | $348 | Best ease-of-use; no built-in spreadsheet→page automation |
| Wix | Core/Business | $348–468 | Has real CMS Collections (CSV import) — closer to our model than expected |
| WordPress.com | Business | $300 | Business tier needed for plugin access (automation) |
| Webflow | Premium site + seats | $528–1,068 | Native CMS is the closest built-in automation match; seat math needs verifying with Webflow directly |
| Google Sites | Free + Workspace Business Starter (~$7/user/mo) | $336 | Google Sites itself is free, but a **custom domain requires paid Workspace** — not actually free once that requirement applies |

## Fairness note for future re-use

When this reference is reused for a follow-up decision (e.g. re-pitching
after the 2026-09-15 GitBook trial deadline, or a scope change), don't just
copy these numbers forward without re-checking — pricing pages change
often, and this table was deliberately non-biased: the brief specifically
asked not to skew the comparison toward GitBook+GitHub, and the honest
finding was that GitBook Premium is *not* the cheapest option here unless
the nonprofit plan comes through.
