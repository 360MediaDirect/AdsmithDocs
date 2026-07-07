# Open Issues — Plain-Language Overview

_Last updated 2026-07-07 09:05:37 UTC · 23 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## General / Across the App

- **[Bug]** **Clear error when testing an invalid link** — Testing a link that isn't valid will show a clear error message right on the Link Testing screen instead of unexpectedly dropping you on the Dashboard. This is nearly finished. (#239)
- **[Feature]** **Safe editing when two people open the same record** — If someone else is already editing a record, you'll see a notice saying who has it open, and the app will prevent one person's changes from quietly overwriting another's. (#267)
- **[Feature]** **New searchable Audit Log** — Administrators will get a searchable history of every change made across the app — who changed what, when, including automated changes — making it easy to trace how a record got to its current state. (#276)
- **[Feature]** **Hide controls that don't do anything** — We're removing or hiding settings that look editable but currently have no effect (certain advertiser web-presence fields, some user permission toggles, and a few data-client and pre-ping options), so screens only show controls that actually work. (#296)
- **[Task]** **Decide the future of the file-share page** — We're confirming whether the old file-share page is still used and either bringing it into New Adsmith Frontend or formally retiring it. (#328)

## Surveys

- **[Feature]** **Every survey design option takes effect** — All customization options on the Survey design tab will actually change what visitors see, and we're reviewing every entity form so no setting is a dead end. (#288)
- **[Bug]** **Connect survey styling settings to the live survey** — Many design settings you can set today (colors, continue button, header and legal text) don't yet reach the live survey; this wires them up so your choices show for visitors. This work is well underway. (#290)
- **[Bug]** **Voucher code and info links appear again** — The voucher code line and the privacy/terms/details links configured for a client will display on the live survey page as they did in the old system. (#291)
- **[Feature]** **Finish wiring the remaining Placement design settings** — The last few design settings (such as survey height and display format) will take effect on the live survey, or be removed if unused, so nothing on the tab is misleading. This is largely complete. (#293)

## Offers

- **[Bug]** **Saved offer options reach the live widget** — Several offer settings that are saved today never actually make it to the live experience; this ensures they take effect (or are cleaned up if they're not needed). (#295)
- **[Feature]** **Automatic performance projections for new offers** — A new tool will estimate how a new offer is likely to perform based on your historical offer data, replacing the old manual gut-check review. This is exploratory with no fixed deadline. (#322)
- **[Task]** **Auto-register offers will respect audience targeting** — Auto-register offers currently ignore age, gender, state, zip, and device targeting; this makes sure they only fire for the visitors they're meant for. High priority. (#333)

## Placements

- **[Feature]** **Preview your unsaved changes** — The Preview button on placement and offer edit pages will reflect the changes you've made but not yet saved, so you can check your edits before committing them. (#292)
- **[Feature]** **Bring back the banner placement style** — We're confirming whether the old banner placement template is still in use and adding it to New Adsmith Frontend if it is. (#326)

## Behind the Scenes

- **[Task]** **Safe, read-only test environment** — Behind-the-scenes setup of a testing environment that uses production-like data in read-only mode, so the team can verify the app safely. Nearly done. (#270)
- **[Feature]** **Automatic to-do capture from team chats** — A behind-the-scenes helper that reads team conversations and turns action items into tracked tasks automatically, reducing manual note-taking. (#272)

## Campaigns

- **[Feature]** **Add the Campaigns module** — New Adsmith Frontend will gain a Campaigns area so you can create, edit, and manage campaigns and offer groups just like in the old system. This is a high-priority core feature that's currently missing. (#200)

## Modals

- **[Feature]** **Make the Modal design tab do something** — The Modal design settings (header title and subtitle, colors, progress bar) currently don't change the visitor-facing modal; they'll either be connected so they work or removed so the tab only shows real options. (#294)

## Data Clients

- **[Feature]** **Restore post-conversion delivery behavior** — We're bringing over the old "after success" delivery and redirect steps for certain clients, or confirming they're no longer needed. (#327)

## Pre-Pings

- **[Feature]** **Restore the older per-client pre-ping** — Offers that still rely on the legacy per-client pre-ping check will keep working once this older path is brought over (or confirmed fully covered by the new one). High priority. (#330)

## Users

- **[Task]** **Review of missing Users features** — A comparison of the old and new Users management screens to identify gaps to bring over — such as bulk role changes, last-login and two-factor status, and select-all — so nothing important is lost. (#80)

## Flows

- **[Task]** **Tidy up the Flow form's appearance** — Fixing styling issues on the Flow form so text boxes, color pickers, checkboxes, and paired fields look consistent and line up side by side like the other forms. Partly done. (#152)

## Reports

- **[Task]** **Confirm Dashboard report figures are accurate** — Investigating why some Dashboard report numbers didn't match the old system, so you can trust that the figures you see are correct. (#271)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 0f0dc75345ae083c3f2607503afd91bf3b9663925bf97592fab1f9e589c4ec62 -->
