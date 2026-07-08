# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 15:46:15 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Feature Parity with the Legacy System

- **[Feature]** **Bring back the Campaigns module** — Campaign management doesn't exist yet in New Adsmith Frontend. This high‑priority work will let you view, create, edit, and configure campaigns — including offer groups, offers, CTA text, and marketing partners — just like the old system. (#200)
- **[Feature]** **Restore legacy pre‑ping coverage** — Some offers still rely on an older, per‑client pre‑ping check that hasn't been carried over. This high‑priority work confirms which offers need it and makes sure that pre‑ping behavior works in New Adsmith Frontend. (#330)
- **[Feature]** **Bring over "after success" client delivery** — Certain post‑conversion delivery and redirect steps from the legacy system haven't been ported yet. This work identifies which are still needed (per client) and reconnects them so conversions complete as expected. (#327)
- **[Task]** **Compare the old and new Users screens** — A review of the legacy Users area against the new one to catch anything missing (like bulk role changes, last‑login and two‑factor status, and notifications), so nothing important is lost in the move. (#80)
- **[Task]** **Decide the future of the file‑share page** — The old file‑share page has no equivalent yet. This is a keep‑or‑retire decision to confirm whether anyone still needs it before rebuilding or officially dropping it. (#328)

## Surveys

- **[Bug]** **Make the survey's Design settings actually take effect** — Many look‑and‑feel settings on the Placement Design tab (colors, header, continue button, progress bar, legal text, and more) are saved but don't change what visitors see. This fixes that so your customizations show up on the live survey. (#290)
- **[Bug]** **Show voucher codes and info links on the live survey** — Custom questions like a voucher code and the privacy/terms/details links are configured in the admin but aren't appearing on the survey page. This restores them so visitors see the code and compliance links. (#291)
- **[Feature]** **Finish wiring the remaining survey Design settings** — A follow‑up to the fix above, covering the last few Design‑tab options that still don't affect the widget. Each will either be made to work or removed so nothing on screen is misleading. (#293)
- **[Feature]** **Make every Design‑tab option do something across the app** — A full review to confirm each customization option you can set actually shows up where it should, with any "dead" options fixed or cleaned up. (#288)

## Offers

- **[Bug]** **Stop offer settings from getting lost before they go live** — Several saved offer options (including modal fields and "force more info") never make it to what visitors see. This makes sure each option either reaches the live experience or is clearly retired. (#295)
- **[Feature]** **Preview offers and placements with your unsaved edits** — Today the Preview button shows the last saved version, so you must save before you can preview a change. This lets Preview reflect your current, in‑progress edits. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — An exploratory tool to project how a new offer is likely to perform based on your own historical offer data, replacing an informal manual gut‑check with a data‑driven estimate. (#322)
- **[Task]** **Apply visitor targeting to auto‑register offers** — Auto‑register offers currently skip age, gender, state, ZIP, and device targeting, so they can fire for people who should be excluded. This confirms the correct behavior and makes these offers respect targeting. (#333)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record, one can unknowingly wipe out the other's changes on save. This adds an editing lock and a warning so you're told when a record is being edited by someone else or has changed since you opened it. (#276)
- **[Feature]** **A searchable history of who changed what** — Records every manual and automated change to entities like offers, placements, and advertisers, with who did it and when, viewable in a searchable Audit Log and on each record's history. Makes troubleshooting "who changed this?" easy. (#276-related) (#276)
- **[Feature]** **Remove admin controls that don't do anything** — Some settings (an advertiser Web Presence tab, certain user‑permission toggles, and a few data‑client and pre‑ping fields) are saved but have no effect, which is confusing. These will be hidden or removed — or scheduled to be made functional. (#296)
- **[Bug]** **Show a clear error for invalid link tests** — Testing an invalid link currently dumps you on the Dashboard with no explanation. This will show a proper failure message right in the Link Testing screen. (#239)

## Behind the Scenes

- **[Task]** **A safe, look‑only staging environment** — Setting up a test environment loaded with production‑like data that can only be read, never changed, so the team can validate the product against realistic data without any risk. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — An internal helper that reads designated Slack channels and files action items as tracked issues automatically, cutting out manual copy‑and‑paste. (#272)

## Reports

- **[Task]** **Confirm report numbers match the legacy system** — Reviewers noticed Dashboard report figures didn't line up with the old system. This investigates where the difference comes from, measures it, and either fixes it or confirms the numbers are correct. (#271)

## Flows

- **[Task]** **Tidy up the look of the Flow form** — Parts of the Flow form appear unstyled or stack awkwardly compared to other forms. This is a careful clean‑up pass so fields line up and look consistent without disturbing the rest of the form. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — Every setting on the Modal Design tab is currently saved but has no effect on the visitor modal. This will either connect those settings so they display, or remove the tab if the modal is meant to be header‑less. (#294)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
