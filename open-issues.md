# Open Issues — Plain-Language Overview

_Last updated 2026-07-17 07:39:15 UTC · 16 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Conversion tracking pixels weren't firing** — A high-priority fix: success pixels you set up on offers were silently never firing, so completed conversions weren't being recorded. Once fixed, those pixels will fire reliably and your attribution and revenue signals will be captured. (#297)
- **[Bug]** **Auto-register offers now respect visitor targeting** — A high-priority fix: auto-register offers were skipping your age, gender, state, ZIP, and device targeting and could fire for visitors who should have been excluded. They'll soon honor the same targeting rules as regular offers. (#333)
- **[Bug]** **Some saved offer settings weren't reaching live pages** — Several offer options you configured (including certain modal fields, Display URL, and a number of data-client settings) weren't making it through to what visitors actually see. This work ensures each saved option either takes effect or is cleaned up. (#295)
- **[Feature]** **Preview your unsaved edits on Placements and Offers** — When editing a placement or offer, the Preview will show your current in-progress changes instead of the last saved version, so you can check your work before saving. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature to estimate how a new offer is likely to perform based on your historical offer data, giving Kurt a data-driven gut-check at intake instead of relying on a manual review. (#322)

## Surveys
- **[Feature]** **Every survey design option should actually work** — A thorough check across all entities to confirm that each customization you set on the design tab is reflected in the live survey, with any unused options fixed or removed. (#288)
- **[Feature]** **Finish connecting Placement design settings to the live survey** — Placement design options such as frame height and display format will properly carry through to what visitors see, and any leftover unused settings will be wired up or removed. (#293)

## Data Clients
- **[Feature]** **Bring back the legacy pre-ping checks for data clients** — A high-priority effort to restore the custom, per-client validation that ran when offers were served in the old system (used by hundreds of active clients) so those checks run again on the new platform. (#338)
- **[Feature]** **Restore after-success delivery behaviors** — Post-conversion delivery and redirect steps from the previous system weren't carried over. This work brings those behaviors back as a reusable setting so affected clients keep working as before. (#327)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a staging version of New Adsmith Frontend loaded with production-like data that can be reviewed and verified without any risk of changing real records. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items** — A helper that reads designated Slack channels, spots action items, and files them as tracked issues automatically, replacing today's manual copy-and-paste process. (#272)

## General / Across the App
- **[Feature]** **Clean up settings that don't do anything** — Several admin controls (including the Advertiser Web Presence fields, some user permission toggles, and a few data-client and pre-ping options) currently save but have no effect. They'll be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Users area review against the previous system** — A detailed comparison of the Users management screens with the old system to identify missing capabilities (like bulk role changes and login/2FA details) and prioritize what to add. (#80)

## Modals
- **[Feature]** **Make the Modal Design tab work — or remove it** — The modal header and progress-bar customization fields currently save but never appear to visitors. This work will either make them show up in the visitor modal or remove them so the tab isn't misleading. (#294)

## Flows
- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled and some paired fields stack awkwardly instead of sitting side by side. This cleanup brings the form in line with the polished look of the Placement and Modal forms. (#152)

## Reports & Dashboard
- **[Task]** **Confirm Dashboard report numbers match the old system** — During testing, some dashboard figures didn't line up with the legacy app. This investigation pins down where the difference comes from and confirms the reports can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 6f6b46eb23460d5a4dadb515313ffdc9b368125f6f6ff2fee621d7d1d0c4666e -->
