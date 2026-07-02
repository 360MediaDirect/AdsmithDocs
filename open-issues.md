# Open Issues — Plain-Language Overview

_Last updated 2026-07-02 13:33:46 UTC · 21 open issues._

This page summarizes everything currently open and being worked on in New Adsmith
Frontend, written for the people who use it day to day. Each item ends with its
internal tracking number in parentheses, e.g. (#244).

## Dashboard

- **[Task]** **Custom date range on the Dashboard filter** — Choosing "Custom" in the date filter will open a real start-and-end date picker, so you can view Dashboard data for any range you like instead of only the preset options. (#58)
- **[Feature]** **Pick report dates right from the Dashboard** — You'll be able to change the reporting day or range using controls in the Dashboard toolbar instead of editing the web address by hand. Shareable links will still update automatically. (#268)
- **[Feature]** **Export the day-by-day breakdown** — A new export button on the breakdown-by-day view will let you download that data (for example to a spreadsheet). This is a high-priority addition. (#286)
- **[Task]** **Cleaner Dashboard header and tables** — The header will show the logo instead of the "Adsmith" text, long offer names will no longer be cut off, and table rows will get tidier alternating shading. (#283)
- **[Task]** **Update notes get their own table** — Update notes will be split out from optimizations and general notes so they're easy to spot and don't get lost among other note types. (#284)
- **[Task]** **Tidier offer names** — When an offer name has a colon, the Dashboard will show only the meaningful part after it, trimming redundant text at the front. Names without a colon are unchanged. (#285)

## Surveys

- **[Bug]** **Design settings that actually change the survey** — Many of the styling and behavior options on a placement's Design tab (colors, continue button, question text, header, legal text and more) currently have no effect on what visitors see. This work connects them so the survey widget reflects what you set. (#290)
- **[Feature]** **Design options that match the live survey** — Every customization on the Design tab will be reflected in the survey view, and all entity forms will be checked to confirm each option is fully wired up rather than doing nothing. (#288)
- **[Task]** **Survey images shown in full** — Survey images will fit within their space and display completely instead of being cropped. (#287)

## Placements

- **[Feature]** **Preview a placement or offer before saving** — A preview button on the add and edit pages will show how a placement or offer will look based on your current (unsaved) entries. (#289)
- **[Feature]** **Better control over the offer list on placements** — Follow-up work will let new placements default to your manual offer order (so drag-to-reorder is respected) and add a way to filter the available offers by category. (#275)

## General / Across the App

- **[Feature]** **No more accidentally overwriting each other's edits** — When two people open the same record, the app will show who's currently editing it and warn before anyone's changes could be lost, keeping edits safe across all entity screens. (#267)
- **[Feature]** **A searchable history of changes** — A new Audit Log will record who changed what and when across offers, placements, advertisers, modals, flows and more (including automated changes), so you can always trace how a record got to its current state. (#276)

## Reports

- **[Task]** **Sortable Offer Audit results** — You'll be able to click column headers in the Offer Performance Audit tables (Sources, Gender, Age, States, Email Domains) to re-sort by any column, making it easier to spot outliers. (#281)

## Flows

- **[Task]** **Consistent styling on the Flow form** — Fixes to the Flow form's appearance so text boxes, color pickers, checkboxes and paired fields look and lay out properly, matching the Placement and Modal forms. Partly done, with the remaining polish handled carefully to avoid affecting other tabs. (#152)

## Campaigns

- **[Feature]** **Bring back Campaign management** — The Campaigns area from the legacy admin isn't in New Adsmith Frontend yet. This adds it back so you can view, create, edit and configure campaigns and their offer groups. This is a critical, high-priority item. (#200)

## Users

- **[Task]** **Review of the Users area vs. the old system** — A documented comparison of the old and new Users screens to identify what's missing (such as bulk actions and extra columns) and guide what to build next. (#80)

## Behind the Scenes

- **[Task]** **A safe testing environment with recent data** — Setting up a separate staging area loaded with May and June data so reports and features can be validated without touching live information. (#270)
- **[Task]** **Checking report numbers against the old system** — An investigation into why some Dashboard report figures differed from the legacy system, to pinpoint the cause and confirm the numbers line up. (#271)
- **[Feature]** **Turning conversations into tracked to-dos** — A behind-the-scenes helper that reads team Slack discussions and automatically logs the resulting action items, reducing manual note-keeping. (#272)

---

_This page is generated automatically from open issues and refreshes regularly. Please don't edit it by hand — changes will be overwritten._

<!-- issues-content-hash: 7cf2416479c6a006663477450a87c48f16726c5f92d204cab5941b3f0ca4624c -->
