# Open Issues — Plain-Language Overview

_Last updated 2026-07-08 13:34:24 UTC · 22 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App
- **[Task]** **Comparing the old and new Users screens** — A review of the legacy Users management against the new one to spot missing capabilities (like bulk role changes, last-login, and two-factor status) so the new Users area can catch up. (#80)
- **[Feature]** **A heads-up when two people edit the same record** — Stops one person's changes from silently overwriting another's; if a record is already open by someone else, you'll see who has it and be prompted to reload instead of losing work. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log will record every change to offers, placements, and other records — whether made by a person or automatically — with who did it and when, all searchable by administrators. (#276)
- **[Feature]** **Removing settings that don't actually do anything** — Cleaning up admin controls that look editable but have no effect (such as Advertiser Web Presence fields, certain user permissions, and some Data Client and Pre-Ping options) to avoid confusion. (#296)
- **[Bug]** **Invalid links no longer dump you on the Dashboard** — When you test a bad link, you'll get a clear error in the Link Testing screen instead of being unexpectedly sent to the Dashboard. (#239)
- **[Task]** **Deciding the future of the file-share page** — Determining whether the old file-share page is still used and either bringing it into the new platform or formally retiring it. (#328)

## Survey
- **[Bug]** **Survey styling settings that were being ignored** — Many Design-tab options (colors, buttons, header text, legal text, progress bar) were saved but never appeared to visitors; this makes them actually take effect, so what you set is what visitors see. (#290)
- **[Bug]** **Voucher code and info links missing on live surveys** — Custom voucher-code questions and the privacy/terms/details links configured for a Data Client will show on the survey page again, matching the old system. (#291)
- **[Feature]** **Making every Design-tab option truly work** — An end-to-end check so each customization you set on the Design tab genuinely shows up in the live survey, with no dead options left behind. (#288)
- **[Feature]** **Finishing the remaining survey Design settings** — Wraps up the last few Placement Design-tab settings (like survey height and display format) so they either work in the live survey or are removed if unused. (#293)

## Offers
- **[Bug]** **Saved offer options that never reached the live widget** — Several offer settings (including Modal-tab fields and "force more info visible") were saved but dropped before display; each will be made to work or removed. (#295)
- **[Task]** **Auto-register offers should respect visitor targeting** — Ensures auto-register offers honor age, gender, state, zip, and device targeting so they don't fire for visitors who should be excluded. (#333)
- **[Feature]** **Preview offers and placements with unsaved changes** — The Preview button will reflect your current edits before you save, so you can check a change without having to save it first. (#292)
- **[Feature]** **Automatic performance estimate for new offers** — Explores predicting how a new offer is likely to perform based on past offers and their results, as a data-driven replacement for the manual gut-check review. (#322)

## Behind the Scenes
- **[Task]** **A read-only staging environment for testing** — Setting up a safe, look-but-don't-touch copy of the platform using production-like data, so testing can be done without risk to live records. (#270)
- **[Feature]** **Turning Slack conversations into tracked tasks** — A helper that reads designated Slack channels and files action items automatically, reducing manual note-taking and follow-up. (#272)

## Campaigns
- **[Feature]** **Bringing back the Campaigns module** — The Campaigns area from the old admin (create and edit campaigns, offer groups, CTA text, and offer settings) will be added to the new platform, which currently has no way to manage campaigns. High priority. (#200)

## Flows
- **[Task]** **Fixing the look of the Flow form** — Addresses unstyled and misaligned parts of the Flow form (text boxes, color pickers, checkboxes, and side-by-side fields) so it matches the polish of the other forms. (#152)

## Data Clients
- **[Feature]** **Porting post-conversion delivery steps** — Brings over the legacy "after-success" behaviors that run after a conversion (delivery and redirect steps) for the clients that need them, or documents them as retired. (#327)

## Modals
- **[Feature]** **Making the Modal Design tab work or removing it** — All six Modal Design-tab fields currently have no effect on the visitor modal; each will be wired up to display properly or removed from the form. (#294)

## Pre-Pings
- **[Feature]** **Restoring legacy pre-ping coverage** — Ports the older per-client pre-ping behavior so any offer that still relies on it keeps working in the new platform. High priority. (#330)

## Reports & Dashboard
- **[Task]** **Investigating mismatched dashboard report numbers** — Looking into why dashboard report figures differ from the legacy system, to find the cause and confirm the numbers can be trusted. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: db2e2e32afdf249c2931b9305c5b4e9f6e133e4b3e0fdf0fc98b37cd3f75c917 -->
