# Open Issues — Plain-Language Overview

_Last updated 2026-07-01 21:32:05 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Feature]** **Custom date range on the dashboard filter** — Choosing "Custom" in the date filter will open a start/end date picker so you can view dashboard data for any specific range instead of only the preset options. The chosen range shows in the filter and refreshes the data. (#58)
- **[Feature]** **Change report dates without touching the address bar** — Date and day selection controls are moving directly into the dashboard toolbar, so you can pull daily or custom reports right from the screen. Links still update behind the scenes so they stay shareable. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the "breakdown by day" view will let you download that data (for example to a spreadsheet). This is high priority. (#286)
- **[Task]** **Cleaner branding and easier-to-read tables** — The header will show the logo instead of the "Adsmith" text, long offer names will no longer be cut off, and table rows will alternate white and light-gray shading for readability. (#283)
- **[Task]** **Update notes get their own table** — Update notes will be split out from optimizations and general notes so they're easy to spot and don't get lost among other note types. (#284)
- **[Task]** **Tidier offer names** — Offer names will drop the redundant text before the first colon and show only the meaningful part. Names without a colon stay as-is. (#285)

## General / Across the App

- **[Feature]** **Prevent two people from overwriting each other's edits** — When someone opens a record to edit it, others will see it as locked with a note about who has it open, and a warning appears if a record was changed while you had it open. This protects against accidentally wiping out a colleague's changes and works across all entity screens. (#267)
- **[Feature]** **A searchable history of every change** — A new Audit Log will record who changed what and when across offers, placements, advertisers, and more (including automated changes), with a searchable view and per-record history. This makes it easy to answer "who changed this and when." (#276)
- **[Bug]** **Clear error when testing an invalid link** — Testing a bad link currently dumps you back on the dashboard with no explanation. Once fixed, you'll see a proper error message instead. (#239)

## Surveys

- **[Bug]** **Survey design settings that actually take effect** — Many survey styling and layout options (colors, buttons, header text, legal text, and more) are configurable but don't currently change what visitors see. This work wires them through so your choices in the Design tab appear in the live survey. (#290)
- **[Feature]** **Design choices reflected in the survey view** — Every option in the Design tab will be checked to make sure it flows all the way through to the live survey, and the same review will run across all entity forms so no setting is left doing nothing. (#288)
- **[Task]** **Full survey images, no cropping** — Survey images will scale to show the whole picture instead of being cut off at the edges. (#287)

## Placements

- **[Feature]** **Better control over the offer list** — Follow-up improvements to the offer picker: setting new placements to use Manual Order by default (so your drag-to-reorder actually sticks) and adding a category filter to the available offers list to find offers faster. (#275)
- **[Feature]** **Preview before you save** — A preview button on the placement and offer add/edit pages will let you see how your placement or offer will look using your current, unsaved settings. (#289)

## Users

- **[Task]** **Filling the gaps in the Users screen** — A detailed comparison of the old Users area against the new one, identifying missing pieces (like bulk actions, last-login and two-factor details, and password setup) so the new Users screen can catch up to what you had before. (#80)

## Campaigns

- **[Feature]** **Bring back Campaign management** — The Campaigns area from the old system isn't in the new platform yet. This adds it back so you can view, create, edit, and configure campaigns and their offer groups. This is a critical, high-priority gap. (#200)

## Flows

- **[Task]** **Fix the look of the Flow form** — Parts of the Flow form currently appear unstyled or awkwardly stacked. This cleanup restores proper styling and side-by-side field layouts to match the other forms. Some of it is already done, with a careful pass remaining. (#152)

## Behind the Scenes

- **[Task]** **A safe testing environment with real data** — Setting up a separate staging environment loaded with May and June data so testing and report checks can happen without affecting live information. (#270)
- **[Task]** **Confirming report numbers match the old system** — Investigating why some dashboard report figures differed from the legacy system, to pinpoint any discrepancy and confirm the numbers can be trusted. (#271)
- **[Feature]** **Automatic issue capture from team chats** — An internal helper that turns action items from team conversations into tracked to-do items automatically, reducing manual copy-and-paste. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 7cf2416479c6a006663477450a87c48f16726c5f92d204cab5941b3f0ca4624c -->
