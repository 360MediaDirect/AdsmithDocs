# Open Issues — Plain-Language Overview

_Last updated 2026-07-11 11:22:35 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers
- **[Bug]** **Success tracking pixels aren't firing** — Conversion pixels you set up under "Pixels to Fire on Success" currently never fire because of a formatting mismatch, so successful conversions go unrecorded. This fix makes those pixels fire reliably again so your attribution and reporting stay accurate. This is a high-priority fix. (#297)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers are currently shown to everyone, ignoring the age, gender, state, ZIP, and device rules you've set, so they can reach people who should be excluded. Once resolved, these offers will honor the same targeting as regular offers (or the exception will be clearly documented). This is a high-priority fix. (#333)
- **[Bug]** **Saved offer options that don't reach the live experience** — Several offer settings you can fill in today (like certain modal fields, Display URL, and some data-client flags) never actually make it to the live visitor experience. We're making sure each option either works end-to-end or is removed so what you configure is what visitors see. (#295)
- **[Feature]** **Preview reflects your unsaved changes** — On placement and offer edit screens, Preview currently shows the last-saved version, so you have to save before you can check a change. Soon Preview will show your current, in-progress edits without forcing a save first. (#292)
- **[Feature]** **Automated performance projection for new offers** — Instead of relying on a manual gut-check, this would estimate how a new offer is likely to perform based on your existing offers and historical results. It gives you a data-grounded read at intake time. This is an exploratory, medium-priority idea. (#322)

## General / Across the App
- **[Feature]** **Protection against two people overwriting each other's edits** — Today, if two admins open the same record at once, one person's changes can silently wipe out the other's. This adds a clear "someone else is editing / this record just changed" warning across all entity screens so nothing gets lost. (#267)
- **[Feature]** **Searchable history of who changed what and when** — There's currently no reliable way to see who paused an offer, changed a cap, or edited a record. This adds an Audit Log you can search and filter by entity, person, action, and date, plus a history view on each record. (#276)
- **[Feature]** **Removing settings that don't actually do anything** — A handful of admin controls (an Advertiser Web Presence tab, some user-permission toggles, and a few Data-Client and Pre-Ping options) currently save but have no effect, which is misleading. We'll hide or remove them, or wire them up properly. (#296)
- **[Task]** **Decision on the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend. We're confirming whether anyone still needs it and either rebuilding it or formally retiring it. (#328)

## Surveys & Modals
- **[Feature]** **Design-tab settings will actually show in the survey** — We're making sure every customization option on the Design tab is reflected in the live survey view, and auditing all entity forms so no setting is left doing nothing. (#288)
- **[Feature]** **Finishing Placement Design settings that don't yet apply** — A few Placement Design-tab options (like iFrame height and display format) are saved but never shown to visitors. Each will either be wired through to the live widget or removed from the form. (#293)
- **[Feature]** **Fixing the Modal Design tab** — The entire Modal Design tab (header text, colors, progress bar, and more) currently saves but never appears in the visitor modal. We'll either build these into the modal or remove the tab if the modal is meant to be header-less. (#294)

## Data Clients & Pre-Pings
- **[Feature]** **Bringing back post-conversion delivery behaviors** — Certain after-success actions from the legacy system (post-conversion delivery and redirects for specific clients) weren't carried over. This restores them as a configurable option so those clients keep working. This is nearly complete. (#327)
- **[Feature]** **Restoring custom serve-time checks for data clients** — Hundreds of data clients relied on custom validation checks that don't currently run on the new platform. This ports that logic over so those checks run again at the right moment (safely failing open on errors and skipped in demo mode). This is a high-priority item. (#338)

## Behind the Scenes
- **[Task]** **A safe, read-only test environment** — Setting up a test environment loaded with production-like data for verification, locked to read-only so testing can never change real records. (#270)
- **[Feature]** **Automatically turning conversations into tracked work items** — A helper that reads designated team conversations and files or updates work items automatically, cutting out manual copy-and-paste. (#272)

## Dashboard & Reports
- **[Task]** **Confirming report numbers match the old system** — During testing, some dashboard report totals didn't line up with the legacy system. We're comparing the two over a fixed date range to find any differences, explain them, and confirm the numbers can be trusted. (#271)

## Campaigns
- **[Feature]** **Bringing the Campaigns module to New Adsmith Frontend** — Campaigns and offer groups can't currently be managed in the new platform. This rebuilds the full workflow — viewing, creating, editing, and configuring campaigns and their offers — to match what's available today. This is a critical, high-priority feature. (#200)

## Flows
- **[Task]** **Cleaning up the look of the Flow form** — Parts of the Flow form currently appear unstyled or misaligned compared to other forms. This tidies up the layout and styling so paired fields, text boxes, and color pickers look consistent. Some of this is already done, with the rest being handled carefully to avoid affecting other tabs. (#152)

## Users
- **[Task]** **Reviewing what's still missing in Users** — A detailed comparison of the old Users area against the new one, listing features not yet carried over (like bulk actions, last-login and two-factor status, and password setup) so we can prioritize what to add. This is a documentation and planning effort. (#80)

## Link Testing
- **[Bug]** **Clear error when a link fails testing** — Right now, testing an invalid link quietly sends you to the dashboard with no explanation. After this fix, you'll get a clear failure message so you know the link didn't pass. This fix is nearly complete. (#239)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: cd6568ac8a6e878837700846282082d0575aaaa68d6d2ab17fcf8602934c2eeb -->
