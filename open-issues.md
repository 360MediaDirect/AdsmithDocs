# Open Issues — Plain-Language Overview

_Last updated 2026-07-21 13:32:15 UTC · 18 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success conversion pixels aren't firing** — When an offer converts, the tracking pixels an admin set up to record that success currently never fire, so conversions can go uncounted. This high-priority fix makes those pixels fire reliably so you don't lose credit for results. (#297)
- **[Task]** **Auto-register offers ignore visitor targeting** — Offers that register a visitor automatically are currently shown to everyone, even when age, gender, state, ZIP, or device targeting says they shouldn't be. This fix makes those offers respect the same targeting rules as regular offers. (#333)
- **[Bug]** **Some saved offer settings never reach live pages** — Several offer options you can fill in today (including offer-level Modal settings and a few delivery flags) quietly get dropped before they take effect. This work makes each saved option either actually work or be removed so the form only shows settings that do something. (#295)
- **[Bug]** **"Conflicting Referrals" field currently does nothing** — The Conflicting Referrals box on an offer's Delivery tab is saved but has no effect at serve time. Once the intended rule is confirmed, this field will either start working as expected or be cleared up so it isn't misleading. (#351)
- **[Feature]** **Preview shows your unsaved edits on Placements and Offers** — Today the Preview button shows the last saved version, so you have to save before you can see a change. After this, Preview will reflect your current in-progress edits without forcing a save first. (#292)
- **[Feature]** **Automatic performance projection for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your own historical offer data, replacing an informal manual gut-check. It would give a data-driven read at intake to help decide whether an offer is worth running. (#322)

## Surveys

- **[Feature]** **Design tab options fully connected across every entity** — A thorough sweep to make sure every design/customization option you set is actually reflected in the live survey, with any options that don't do anything getting fixed or removed. You'll be able to trust that what you configure is what visitors see. (#288)
- **[Feature]** **Remaining Placement design settings applied to the live widget** — A handful of Placement Design-tab settings (like iframe height and display format) are saved but not yet shown in the widget. This finishes wiring them up so those choices take effect for visitors. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring over the file-based pre-ping checks** — A large group of data clients (hundreds) rely on custom pre-delivery validation from the old system that doesn't yet run in New Adsmith Frontend. This high-priority work restores those checks so leads are validated the same way before delivery. (#338)
- **[Feature]** **Restore after-success delivery steps for data clients** — Certain post-conversion delivery/redirect behaviors from the legacy system weren't carried over. This work adds them back as a configurable option so those clients keep working as before. (#327)

## Behind the Scenes

- **[Task]** **Read-only staging environment for safe testing** — Setting up a testing copy of the app connected to production-like data that can't be changed, so the team can verify behavior against realistic numbers without any risk to live data. (#270)
- **[Feature]** **Automatic issue capture from team chat** — A helper that turns action items discussed in chat into tracked work items automatically, so requests get logged without manual copy-paste. (#272)

## Reports

- **[Task]** **Confirm dashboard report numbers match the legacy system** — Reviewers noticed dashboard figures didn't line up with the old app. This investigation pins down where any differences come from and either corrects them or confirms the numbers are trustworthy. (#271)

## Users

- **[Task]** **Compare the new Users area against the legacy version** — A detailed review of what the old Users screen offered versus the new one, highlighting gaps like bulk role changes, last-login and two-factor status, and pagination controls. It sets the roadmap for bringing the Users area up to full parity. (#80)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned compared to other forms, with fields stacking awkwardly. This clean-up makes the Flow form look consistent and polished like the Placement and Modal forms. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — Every field on the Modal Design tab is currently saved but has no effect on what visitors see. This work either makes those header and progress-bar settings appear in the visitor modal or removes the tab so it isn't misleading. (#294)

## Properties

- **[Bug]** **Enforce the domain allowlist on properties** — The allowed-domains list on a property is saved but not actually enforced, so ads can currently be served on any website. This fix makes the app honor the list so offers only serve on approved domains, while properties without a list stay unaffected. (#350)

## General / Across the App

- **[Feature]** **Remove admin controls that don't do anything** — Several settings across the app (like the Advertiser Web Presence fields, certain user-permission toggles, and a few data-client and pre-ping options) are saved but currently have no effect, which can be misleading. This work hides or removes them, or schedules real functionality, so every control you see actually does something. (#296)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 10b1596502d69ac6fd2aad6156b921186ddd497739fcbc9cd0b49d4592839d20 -->
