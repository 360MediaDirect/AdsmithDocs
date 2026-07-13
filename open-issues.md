# Open Issues — Plain-Language Overview

_Last updated 2026-07-13 05:09:08 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels set up on offers currently never fire because of a mismatch in how they're saved versus read. Once fixed, the pixels you configure will fire on a successful conversion, so your attribution and revenue tracking stay accurate. This is a high-priority fix. (#297)
- **[Task]** **Auto-register offers ignore audience targeting** — Auto-register offers are firing for every visitor, even ones outside their intended age, gender, state, ZIP, or device targeting. This fix will make them respect the same targeting rules as regular offers (or clearly document any intentional difference). A high-priority correction. (#333)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several offer options you can fill in today (including Modal-tab fields, Display URL, and certain data-client flags) are being dropped before they reach visitors. Each will be either properly wired through or removed from the form so there are no misleading, do-nothing fields. (#295)
- **[Feature]** **Preview unsaved edits on placements and offers** — Today the Preview button shows the last saved version, so you have to save before you can see a change. This update lets Preview reflect your current in-progress edits without saving first. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory feature that estimates how a new offer is likely to perform based on your historical offer data, replacing an informal manual review. It would give you a data-grounded read on a new offer right at intake. (#322)

## Admin, Users & Auditing

- **[Feature]** **Protection against two people overwriting the same record** — A new safeguard so that when two admins edit the same record, one can't silently erase the other's changes. You'll see a clear "locked by someone else" notice or a prompt to reload if a record changed while you had it open. (#267)
- **[Feature]** **Searchable history of who changed what** — A new Audit Log that records every manual and automated change across the platform, with who made it and when. Administrators will be able to search and filter this history and view a change trail on each record's detail page. (#276)
- **[Feature]** **Clean up admin controls that don't do anything** — Several settings across Advertisers (Web Presence), user permissions, Data Clients, and Pre-Pings currently save but have no effect. These will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Users screen gap review versus the old system** — A documentation review comparing the Users area in New Adsmith Frontend against the legacy system to identify missing pieces (like bulk actions, last-login, and 2FA status) and prioritize what to add. (#80)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent yet. This is a keep-or-retire decision to confirm whether anyone still needs it before dropping or rebuilding it. (#328)

## Data Clients & Pre-Pings

- **[Feature]** **Restore custom pre-ping checks for data clients** — Custom serve-time validation checks that hundreds of data clients relied on in the old system aren't running on the new platform yet. This work brings those checks back so leads are validated correctly. A high-priority item. (#338)
- **[Feature]** **Restore after-success delivery steps** — Post-conversion delivery and redirect steps used by certain clients weren't carried over. This adds a flexible, configurable version so those after-success behaviors work again. (#327)

## Surveys

- **[Feature]** **Make every Design-tab setting actually take effect** — A thorough check across all entities to ensure every customization option on the Design tab is reflected in the live survey view, with no settings that silently do nothing. (#288)
- **[Feature]** **Finish connecting Placement Design settings to the survey widget** — A handful of Placement Design-tab settings (such as iFrame height and display format) either don't apply yet or aren't read by the live widget. Each will be fully wired up or removed. (#293)

## Reports & Dashboard

- **[Task]** **Confirm dashboard numbers match the legacy system** — An investigation into why some dashboard report figures didn't line up with the old system during testing, so we can pinpoint the cause and confirm the reports are trustworthy. (#271)
- **[Bug]** **Testing an invalid link should show an error, not the dashboard** — Right now, entering an invalid link during link testing sends you to the dashboard instead of telling you the link failed. This fix gives a clear error result. Nearly complete. (#239)

## Modals

- **[Feature]** **Make the Modal Design tab work — or remove it** — Every field on the Modal Design tab currently saves but has no visible effect on the visitor modal. These will either be built to display (header text, colors, progress bar) or removed so the tab isn't misleading. (#294)

## Flows

- **[Task]** **Fix the styling on the Flow form** — Parts of the Flow form don't look right — plain textareas, unstyled color pickers and checkboxes, and paired fields stacking instead of sitting side by side. This tidies up the form to match the polished look of the other screens. Partly done. (#152)

## Campaigns

- **[Feature]** **Bring back the Campaigns module** — The Campaigns area from the old system isn't in New Adsmith Frontend yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups. A critical, high-priority feature. (#200)

## Behind the Scenes

- **[Task]** **Read-only staging environment for safe testing** — Setting up a staging version of the product connected to a copy of real data, locked to read-only, so the team can verify behavior against realistic data without any risk of changing it. (#270)
- **[Feature]** **Turn Slack conversations into tracked work items automatically** — An internal helper that reads designated Slack conversations and files action items as tracked issues, cutting out manual copy-and-paste when capturing follow-ups. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
