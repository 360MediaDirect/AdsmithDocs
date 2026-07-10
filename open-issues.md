# Open Issues — Plain-Language Overview

_Last updated 2026-07-10 07:09:19 UTC · 25 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Offers

- **[Feature]** **Live preview of unsaved offer and placement edits** — When editing an offer or placement, the Preview will show your current in-progress changes instead of only the last saved version, so you can check your work before saving. (#292)
- **[Bug]** **Some saved offer settings never reach the live page** — Several offer options you fill in (including modal settings, "Force More Info Visible," Display URL, and certain data-client flags) are being dropped and never applied to what visitors see; this fix ensures each saved option is either used or clearly retired. (#295)
- **[Bug]** **Success pixels not firing** — Conversion tracking pixels set up on an offer currently never fire, meaning credit for conversions can be lost silently; this fix makes configured success pixels fire reliably. This is a high-priority fix. (#297)
- **[Bug]** **Auto-register offers ignore visitor targeting** — Auto-register offers are firing for everyone regardless of the age, gender, state, zip, or device targeting you set; this fix makes them respect those rules (or documents the difference if intended). A high-priority fix. (#333)
- **[Bug]** **bPerx voucher code missing from offer preview** — The bPerx voucher code line isn't showing in the offer preview on the dev site; this work tracks down why the code lookup fails and restores the voucher display in both preview and the live survey. (#344)
- **[Feature]** **Predict new-offer performance automatically** — Instead of relying on a manual gut-check, new offers could be scored against your historical offer data to estimate how they're likely to perform, giving a helpful projection at intake time. (#322)

## General / Across the App

- **[Feature]** **Protection against two people overwriting each other's edits** — When someone opens a record for editing, others will see it's locked and by whom, and saves will warn you if the record changed since you opened it — preventing accidental lost changes across every entity screen. (#267)
- **[Feature]** **Searchable activity/audit log** — A new admin page will record who changed what and when (including automated changes) across offers, placements, advertisers, and more, so you can trace history and troubleshoot with confidence. (#276)
- **[Feature]** **Clean up controls that don't do anything** — Several admin settings that currently save but have no effect (Advertiser Web Presence fields, some user permission toggles, a couple of Data-Client and Pre-Ping options) will be removed or hidden so the screens only show controls that actually work. (#296)
- **[Task]** **Decide the future of the old file-share page** — The legacy file-share page has no equivalent in New Adsmith Frontend; this task confirms whether anyone still needs it and either rebuilds or formally retires it. (#328)
- **[Bug]** **Invalid link test should show an error, not the dashboard** — When you test an invalid link, you're currently sent to the dashboard with no explanation; this fix shows a clear failure message instead. (#239)
- **[Task]** **Review remaining user-management features to build** — A comparison of the old Users area against New Adsmith Frontend to confirm which features (like bulk actions and login/2FA details) still need to be carried over. (#80)

## Surveys

- **[Feature]** **Make sure every design option actually shows on the survey** — A full check that each customization option in the design tabs is reflected on the live survey view, with any settings that lead nowhere either wired up or removed. (#288)
- **[Bug]** **Voucher code and info links missing on live survey** — For affected data clients, the voucher code line and the privacy/terms/details links show in the old app but not the new one; this fix restores them since they're needed for compliance and passing leads. A high-priority fix. (#291)
- **[Feature]** **Finish connecting Placement design settings to the survey** — A few Placement design-tab settings (like survey height and display format) are saved but not yet applied to the survey; this work connects them or removes any that aren't needed. (#293)

## Pre-Pings

- **[Feature]** **Run display-trigger pre-ping checks at the right moment** — Certain pre-ping validations currently only check that a field exists rather than performing the real-time check like the old system; this restores the live check so offers that should be hidden actually are. A high-priority fix. (#337)
- **[Feature]** **Bring over the older per-client pre-ping checks** — Hundreds of data clients relied on custom pre-ping validation in the old system that isn't running in New Adsmith Frontend yet; this work maps and restores that behavior so those checks apply again. A high-priority item. (#338)

## Placements

- **[Feature]** **Fix historical placement reports showing zero offer impressions** — Offer impressions weren't being recorded in hourly stats, so past placement reports showed zero; this update captures that number so historical reports are accurate. (#339)

## Modals

- **[Feature]** **Make the Modal Design tab actually work (or remove it)** — All six fields on the Modal design tab currently save but have no effect on the visitor modal; this work either builds the header and progress-bar display they control or removes the tab if it's not needed. (#294)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Parts of the Flow form look unstyled or awkwardly stacked; this fixes the layout so fields, text boxes, color pickers, and checkboxes match the polished look of the other forms. (#152)

## Campaigns

- **[Feature]** **Bring the Campaigns area to New Adsmith Frontend** — The Campaigns module from the old admin isn't in the new platform yet; this adds the ability to view, create, edit, and configure campaigns and their offer groups. This is a critical, high-priority build. (#200)

## Reports

- **[Task]** **Confirm new report numbers match the old system** — Dashboard report figures didn't line up with the legacy app during testing; this investigation pins down where the difference comes from and either fixes it or confirms the numbers are correct. (#271)

## Data Clients

- **[Feature]** **Restore after-success delivery behavior** — Post-conversion delivery and redirect steps from the old system weren't carried over; this brings them back as a configurable option so affected clients behave as they did before. (#327)

## Behind the Scenes

- **[Task]** **Set up a read-only staging environment** — A safe, prod-like environment for testing and verification that can't accidentally change real data. (#270)
- **[Feature]** **Assistant that turns meeting notes into tracked tasks** — An internal helper to capture action items from team conversations and log them automatically, reducing manual copy-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 20c05265760e30b087db164aa9ffb7701fea9cb19d23bb2497ef9c503a36041b -->
