# Open Issues — Plain-Language Overview

_Last updated 2026-07-15 03:01:40 UTC · 20 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Bug]** **Success pixels aren't firing** — Conversion tracking pixels set up on an offer currently never fire, which means completed conversions may go unrecorded. This fix ensures a configured success pixel actually fires when a conversion happens, so attribution and revenue tracking are accurate. This is a high-priority bug fix. (#297)
- **[Bug]** **Some saved offer settings never reach the live experience** — Several options you can set on an offer (including its Modal-tab settings, Display URL, and certain data-client flags) are being dropped before they get to visitors. Once fixed, the settings you save will actually take effect — or be clearly removed if they're no longer needed. (#295)
- **[Task]** **Auto-register offers will respect visitor targeting** — Auto-register offers currently ignore age, gender, state, ZIP, and device targeting, so they can show to people who should be excluded. This work makes them honor the same targeting rules as regular offers (or confirms the difference is intentional). This is a high-priority fix. (#333)
- **[Feature]** **Preview unsaved changes on Placements and Offers** — Today the Preview button shows the last saved version of a placement or offer, so you have to save before you can check a change. This upgrade lets Preview reflect your current, unsaved edits. (#292)
- **[Feature]** **Automatic performance projections for new offers** — An exploratory tool that estimates how a new offer is likely to perform based on your historical offer data, replacing the informal manual gut-check. It would give the team a quick, data-grounded read at intake time. (#322)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When two admins open the same record at once, one person's changes can silently wipe out the other's. This adds an editing lock and a warning so you'll see when someone else is editing a record and won't lose your work. (#267)
- **[Bug]** **Clearer result when testing an invalid link** — Testing an invalid link currently just dumps you back on the dashboard with no explanation. After this fix, you'll get a clear error message telling you the link failed. This is a nearly-finished bug fix. (#239)
- **[Feature]** **Clean up settings that don't do anything** — Several admin controls (an Advertiser "Web Presence" tab, some user permission toggles, and a couple of Data-Client and Pre-Ping options) are saved but never actually used, which is misleading. They'll be hidden or removed — or properly built out — so what you see reflects what really happens. (#296)
- **[Task]** **Decide the future of the file-share page** — The old file-share page has no equivalent in New Adsmith Frontend. This is a quick review to confirm whether anyone still needs it, then either add it back or retire it for good. (#328)

## Surveys

- **[Feature]** **Make sure every design option shows up in the survey** — A review to confirm that every customization you set on the Design tab actually appears in the live survey, across all entity screens, with no dead or disconnected options. You'll be able to trust that the settings you choose take effect. (#288)
- **[Feature]** **Finish connecting Placement design settings to the survey widget** — A handful of Placement Design-tab settings (like iFrame height and display format) are saved but not yet reflected in the live widget. This wires them up so your choices show through — or removes any that aren't needed. (#293)

## Data Clients & Pre-Pings

- **[Feature]** **Bring back post-conversion delivery scripts** — The old platform's "after-success" client behaviors (post-conversion delivery and redirects) haven't been carried over yet. This ports them so those clients keep working as before. This work is nearly complete. (#327)
- **[Feature]** **Restore custom pre-ping checks for hundreds of data clients** — Legacy custom validation that runs when an offer is served hasn't been carried into New Adsmith Frontend, affecting 448 data clients whose checks silently aren't running today. This work reconnects that validation so those clients behave as expected. This is a large, high-priority effort. (#338)

## Behind the Scenes

- **[Task]** **A safe, read-only test environment** — Setting up a staging copy of New Adsmith Frontend against production-like data for verification, locked to read-only so testing can't change real records. This work is well underway. (#270)
- **[Feature]** **Turn team conversations into tracked work automatically** — A helper that reads designated chat channels, spots action items, and files them as tracked issues, cutting out manual copy-and-paste. (#272)

## Flows

- **[Task]** **Fix unstyled areas of the Flow form** — Parts of the Flow form currently look broken or unstyled — plain text boxes, unstyled color pickers, and paired fields that stack awkwardly instead of sitting side by side. This tidies up the form so it matches the polished look of other screens. Partially done, with a careful final pass remaining. (#152)

## Modals

- **[Feature]** **Make the Modal Design tab actually work** — Every field on the Modal Design tab is currently saved but has no effect on what visitors see. This will either wire those fields up so they change the modal's header and progress bar, or remove them if the modal is meant to be simple. (#294)

## Campaigns

- **[Feature]** **Bring the Campaigns module to New Adsmith Frontend** — The Campaigns feature from the old admin — for creating and managing campaigns and offer groups — isn't in the new platform yet. This adds it back so you can view, create, and configure campaigns as before. This is a critical, high-priority addition. (#200)

## Users

- **[Task]** **Close the gaps between the old and new Users screens** — A detailed review comparing the old Users area to the new one, identifying missing pieces (like bulk actions, last-login and two-factor status, and a password field on new users) so the new screen reaches full parity. This review is largely complete. (#80)

## Dashboard

- **[Task]** **Confirm dashboard report numbers match the old system** — During testing, some dashboard figures didn't line up with the legacy system, making it hard to trust the numbers. This investigation pins down where any differences come from and either fixes them or confirms the figures are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: f12be1691f4d05be7a51684fc6fe5ab6d4c4751d5a9de6a600395df673d554b3 -->
